# Silent Failure in Asynchronous Dart Code

This repository demonstrates a common error in asynchronous Dart code: silently failing to propagate exceptions. The example uses `http` to fetch data from an API.  The `catch` block logs the error but doesn't re-throw it, leading to a silent failure that can be difficult to debug.

The `bugSolution.dart` file shows how to fix this by re-throwing the exception or handling it appropriately at higher level.