# asyncexperts-materials

## Introduction

Diagnostics Concurrency Visualizer for Visual Studio 2019
https://marketplace.visualstudio.com/items?itemName=Diagnostics.DiagnosticsConcurrencyVisualizer2019

About Concurrency Visualizer
https://docs.microsoft.com/pl-pl/visualstudio/profiling/concurrency-visualizer?view=vs-2019

Concurrency Visualizer videos on Channel 9
https://channel9.msdn.com/Search?term=Concurrency%20Visualizer&lang-en=true

Concurrency Visualizer Profiler - Adam Sitnik's article
https://adamsitnik.com/ConcurrencyVisualizer-Profiler

## Threading

Additional resources:

"Optimizing Concurrency Levels in the .NET ThreadPool"- hill-climbing described in the paper published by Microsoft:
https://www.researchgate.net/publication/228977836_Optimizing_concurrency_levels_in_the_net_threadpool_A_case_study_of_controller_design_and_implementation

".NET Threadpool starvation, and how queuing makes it worse" - great article about example deadlock scenario by Criteo:
https://labs.criteo.com/2018/10/net-threadpool-starvation-and-how-queuing-makes-it-worse

https://dschenkelman.github.io/2013/10/29/asynchronous-io-in-c-io-completion-ports

Understanding the Windows I/O System:
https://www.microsoftpressstore.com/articles/article.aspx?p=2201309&seqNum=3


Multithreaded Asynchronous I/O & I/O Completion Ports:
https://www.drdobbs.com/cpp/multithreaded-asynchronous-io-io-comple/201202921


The CLR Thread Pool 'Thread Injection' Algorithm:
https://mattwarren.org/2017/04/13/The-CLR-Thread-Pool-Thread-Injection-Algorithm

Concurrency - Throttling Concurrency in the CLR 4.0 ThreadPool:
https://docs.microsoft.com/en-us/archive/msdn-magazine/2010/september/concurrency-throttling-concurrency-in-the-clr-4-0-threadpool

New and Improved CLR 4 Thread Pool Engine:
http://www.danielmoth.com/Blog/New-And-Improved-CLR-4-Thread-Pool-Engine.aspx

Diagnosing .NET Core ThreadPool Starvation with PerfView:
https://docs.microsoft.com/en-us/archive/blogs/vancem/diagnosing-net-core-threadpool-starvation-with-perfview-why-my-service-is-not-saturating-all-cores-or-seems-to-stall

## Async Basics

Additional resources:

StartNew is Dangerous
https://blog.stephencleary.com/2013/08/startnew-is-dangerous.html

Dynamic Task Parallelism
https://docs.microsoft.com/en-us/previous-versions/msp-n-p/ff963551(v=pandp.10)

Async/Await FAQ
https://devblogs.microsoft.com/pfxteam/asyncawait-faq/

Understanding the Costs of Async and Await
https://docs.microsoft.com/en-us/archive/msdn-magazine/2011/october/asynchronous-programming-async-performance-understanding-the-costs-of-async-and-await

Eliding async await
https://blog.stephencleary.com/2016/12/eliding-async-await.html

Understanding the Whys, Whats, and Whens of ValueTask
https://devblogs.microsoft.com/dotnet/understanding-the-whys-whats-and-whens-of-valuetask/

Prefer ValueTask to Task, always; and don't await twice
https://blog.marcgravell.com/2019/08/prefer-valuetask-to-task-always-and.html

Async ValueTask Pooling in .NET 5
https://devblogs.microsoft.com/dotnet/async-valuetask-pooling-in-net-5/

.NET 5 and pooling for ValueTasks
https://blog.scooletz.com/2020/06/01/pooling-for-value-tasks-in-net5

Proposal: ValueTask.WhenAll #23625
https://github.com/dotnet/runtime/issues/23625

"Determine what to do with "async ValueTask" caching" #13633
https://github.com/dotnet/runtime/issues/13633

Miscellaneous C# Async Tips
https://stu.dev/miscellaneous-csharp-async-tips/

The Dangers of Task.Factory.StartNew
https://sergeyteplyakov.github.io/Blog/async/2019/05/21/The-Dangers-of-Task.Factory.StartNew.html

LongRunning Is Useless For Task.Run With Async/Await
http://blog.i3arnon.com/2015/07/02/task-run-long-running/

Task.Unwrap() - A useful proxy to avoid inner Task inside a Task
http://vunvulearadu.blogspot.com/2015/09/taskunwrap-usefull-proxy-to-avoid-inner.html

Task.Run vs Task.Factory.StartNew
https://devblogs.microsoft.com/pfxteam/task-run-vs-task-factory-startnew/

StartNew is Dangerous
https://blog.stephencleary.com/2013/08/startnew-is-dangerous.html

## Async II
ConfigureAwait.Fody
https://github.com/Fody/ConfigureAwait

VM775:1 Fody licensing
VM775:1 https://github.com/Fody/Home/blob/master/pages/licensing-patron-faq.md
VM775:1 ConfigureAwait FAQ
VM775:1 https://devblogs.microsoft.com/dotnet/configureawait-faq/
VM775:1 Await, SynchronizationContext, and Console Apps
VM775:1 https://devblogs.microsoft.com/pfxteam/await-synchronizationcontext-and-console-apps/
VM775:1 Await, SynchronizationContext, and Console Apps: Part 2
VM775:1 https://devblogs.microsoft.com/pfxteam/await-synchronizationcontext-and-console-apps-part-2/
VM775:1 Await, SynchronizationContext, and Console Apps: Part 3
VM775:1 https://devblogs.microsoft.com/pfxteam/await-synchronizationcontext-and-console-apps-part-3/
VM775:1 Implementing a SynchronizationContext.SendAsync method
VM775:1 https://devblogs.microsoft.com/pfxteam/implementing-a-synchronizationcontext-sendasync-method/
VM775:1 ExecutionContext vs SynchronizationContext
VM775:1 https://devblogs.microsoft.com/pfxteam/executioncontext-vs-synchronizationcontext/
VM775:1 Parallel Computing - It's All About the SynchronizationContext
VM775:1 https://docs.microsoft.com/en-us/archive/msdn-magazine/2011/february/msdn-magazine-parallel-computing-it-s-all-about-the-synchronizationcontext
VM775:1 QueueSynchronizationContext.cs
VM775:1 https://github.com/kekyo/SynchContextSample/blob/master/SynchContextSample/QueueSynchronizationContext.cs
VM775:1 AsyncContext from AsyncEx
VM775:1 https://github.com/StephenCleary/AsyncEx/blob/master/doc/AsyncContext.md

What Color is Your Function?
VM1143:1 http://journal.stuffwithstuff.com/2015/02/01/what-color-is-your-function/
VM1143:1 Project Loom
VM1143:1 https://wiki.openjdk.java.net/display/loom/Main
VM1143:1 Dependency injection in ASP.NET Core
VM1143:1 https://docs.microsoft.com/en-us/aspnet/core/fundamentals/dependency-injection?view=aspnetcore-3.1
VM1143:1 Injection Constructors should be simple
VM1143:1 https://blog.ploeh.dk/2011/03/03/InjectionConstructorsshouldbesimple/
VM1143:1 Stephen Cleary's blog post
VM1143:1 https://blog.stephencleary.com/2013/01/async-oop-2-constructors.html
VM1143:1 null-conditional await proposal
VM1143:1 https://github.com/dotnet/csharplang/issues/35
VM1143:1 Task Exception Handling in .NET 4.5
VM1143:1 https://devblogs.microsoft.com/pfxteam/task-exception-handling-in-net-4-5/
VM1143:1 Await, and UI, and deadlocks! Oh my!
VM1143:1 https://devblogs.microsoft.com/pfxteam/await-and-ui-and-deadlocks-oh-my/
VM1143:1 Should I expose asynchronous wrappers for synchronous methods?
VM1143:1 https://devblogs.microsoft.com/pfxteam/should-i-expose-asynchronous-wrappers-for-synchronous-methods/
VM1143:1 ASP.NET Core Diagnostic Scenarios
VM1143:1 https://github.com/davidfowl/AspNetCoreDiagnosticScenarios/blob/master/AsyncGuidance.md
VM1143:1 Discussion: async constructors #419
VM1143:1 https://github.com/dotnet/csharplang/issues/419

if an exception is thrown
VM1292:1 https://stackoverflow.com/questions/53215577/why-does-exception-from-async-void-crash-the-app-but-from-async-task-is-swallowe
VM1292:1 AsyncContext
VM1292:1 https://github.com/StephenCleary/AsyncEx/blob/e637035c775f99b50c458d4a90e330563ecfd07b/src/Nito.AsyncEx.Context/AsyncContext.cs
VM1292:1 AsyncAwaitBestPractices
VM1292:1 https://github.com/brminnick/AsyncAwaitBestPractices
VM1292:1 Removing async void
VM1292:1 https://johnthiriet.com/removing-async-void/
VM1292:1 AsyncAwaitBestPractices
VM1292:1 https://github.com/brminnick/AsyncAwaitBestPractices
VM1292:1 Great Twitter discussion about ContinueWith and async
VM1292:1 https://twitter.com/ben_a_adams/status/1045096041266249728

Performance best practices in C#
VM1429:1 https://medium.com/@kevingosse/performance-best-practices-in-c-b85a47bdd93a
VM1429:1 Issue Add non-generic TaskCompletionSource 37452
VM1429:1 https://github.com/dotnet/runtime/pull/37452
VM1429:1 Performance best practices in C#
VM1429:1 https://medium.com/@kevingosse/performance-best-practices-in-c-b85a47bdd93a
VM1429:1 The danger of TaskCompletionSource class
VM1429:1 https://devblogs.microsoft.com/premier-developer/the-danger-of-taskcompletionsourcet-class/

System.Private.CoreLib
VM1601:1 https://github.com/dotnet/runtime/blob/4f9ae42d861fcb4be2fcd5d3d55d5f227d30e723/src/libraries/System.Private.CoreLib/src/System/Runtime/CompilerServices/TaskAwaiter.cs
VM1601:1 await anything
VM1601:1 https://devblogs.microsoft.com/pfxteam/await-anything/
VM1601:1 Dispatcher.Yield in WPF
VM1601:1 https://docs.microsoft.com/en-us/dotnet/api/system.windows.threading.dispatcher.yield?view=netcore-3.1
VM1601:1 Understanding C# async / await (2) The Awaitable-Awaiter Pattern
VM1601:1 https://weblogs.asp.net/dixin/understanding-c-sharp-async-await-2-awaitable-awaiter-pattern
VM1601:1 Eduasync part 5: Making Task Awaitable
VM1601:1 https://codeblog.jonskeet.uk/2011/05/17/eduasync-part-5-making-task-lt-t-gt-awaitable/
VM1601:1 When would I use Task.Yield()?
VM1601:1 https://stackoverflow.com/questions/22645024/when-would-i-use-task-yield
VM1601:1 Task.Yield - real usages?
VM1601:1 https://stackoverflow.com/questions/23431595/task-yield-real-usages
VM1601:1 “await Task.Yield()” and its alternatives
VM1601:1 https://stackoverflow.com/questions/20319769/await-task-yield-and-its-alternatives
VM1601:1 A Tour of Task, Part 10: Promise Tasks
VM1601:1 https://blog.stephencleary.com/2015/04/a-tour-of-task-part-10-promise-tasks.html

AsyncLazy
VM1990:1 https://devblogs.microsoft.com/pfxteam/asynclazyt/
VM1990:1 New in .NET 4.5: ThreadLocal.Values
VM1990:1 https://devblogs.microsoft.com/pfxteam/new-in-net-4-5-threadlocal-values/
VM1990:1 Very high latency for GC when using (lots of) ThreadLocal #2382
VM1990:1 https://github.com/dotnet/runtime/issues/2382
VM1990:1 RavenDB's own implementation - LightWeightThreadLocal
VM1990:1 https://github.com/ravendb/ravendb/blob/v4.2/src/Sparrow/Threading/LightWeightThreadLocal.cs
VM1990:1 Asynchronous Lazy Initialization
VM1990:1 https://blog.stephencleary.com/2012/08/asynchronous-lazy-initialization.html
VM1990:1 AsyncEx - AsyncLazy documentation
VM1990:1 https://github.com/StephenCleary/AsyncEx/wiki/AsyncLazy
VM1990:1 AsyncEx - AsyncLazy source code
VM1990:1 https://github.com/StephenCleary/AsyncEx/blob/db32fd5db0d1051e867b36ae039ea13d2c36eb91/src/Nito.AsyncEx.Coordination/AsyncLazy.cs
VM1990:1 Cancelable AsyncLazy that is thread-safe
VM1990:1 https://codereview.stackexchange.com/questions/224232/cancelable-asynclazy-that-is-thread-safe
