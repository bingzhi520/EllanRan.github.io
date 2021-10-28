# 断言
## 1. check 
check 宏在 Debug Development Test 和 Shipping Editor 版本中运行；<br>
以 “Slow” 结尾的宏仅在 Debug 版本中运行；<br>
定义 USE_CHECKS_IN_SHIPPING 为1，使 check 宏可在所有版本中运行。 <br>
当check宏不运行时候，里面的表达式不执行
~~~
// 若expr为false，停止执行
check(expr) 
checkSlow(expr);
// 若expr为false，停止执行并输出format到日志
checkf(expr,format,...) 
checkfSlow(expr,format,...)；
// 执行一次的do-while循环语句，如checkCode( if(expr) {UE_LOG(LogTemp, Fatal, TEXT("xxx"));} );
checkCode(Code)；
// 此行被hit，则中断程序，类似check(false)，主要用于不可到达的代码块
checkNoEntry();
// 此行被hit超过一次，则中断程序，有且仅有一次执行的机会
checkNoReentry();
// 检测函数是否递归，若为递归则中断程序
checkNoRecursion();
// 类似于checkNoEntry()，主要用于应该被重写的虚函数
unimplemented(); 
~~~
## 2. Verify
verify 宏在 Debug、Development、Test 和 Shipping Editor 版本中完整运行。<br>
当Verify宏不运行时候，里面的表达式依旧执行<br>
~~~
// 若expr为false，停止执行
verify(expr) 
verifySlow(expr);
// 若expr为false，停止执行
verify(expr,format,...) 
verifySlow(expr,format,...); 
~~~
## 3. Ensure
Ensure 宏在所有版本中计算表达式的值，但仅在 Debug、Development、Test 和 Shipping Editor 版本通知 crash reporter。<br>
默认情况下，ensure 宏仅报告一次，需要每次都报告时使用 ensureAlways 宏。 <br>
~~~
// 若expr为false，上报给crash reporter
ensure(expr) 
ensureAlways(expr);
// 若expr为false，上报给crash reporter并将format输出到output日志
ensureMsgf(expr,format,...) 
ensureAlwaysMsgf(expr,format,...);
~~~
https://docs.unrealengine.com/en-US/ProgrammingAndScripting/ProgrammingWithCPP/Assertions/index.html
