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
