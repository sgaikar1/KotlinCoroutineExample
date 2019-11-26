# KotlinCoroutineExample
KotlinCoroutineExample

Kotlin coroutins pin points
What problem does it solve?
Manage long-running tasks that might otherwise block the main thread and cause your app to freeze.
Providing main-safety, or safely calling network or disk operations from the main thread.
Also in addition of above it gives more flexibilty for reading the code
1. Use suspend keyword before fun to make it coroutins type
2. Kotlin provides three dispatchers that you can use i.e. Main, IO, Default
3.Default dispatcher is used to optimize CPU-intensive work such as sorting or filtering long lists
4. method defined with suspend keyword can not be called directly from any method, to use that method we need to use coroutines scope,
5. to use result received from coroutins we need to use withContext() with dispatcher of where we want to use that result, example main if we want to show result on UI
6. suspend functionsdefined  inside scope waits for the execution of suspend function called before them, and once execution of one task is complete sequential suspend gets called
