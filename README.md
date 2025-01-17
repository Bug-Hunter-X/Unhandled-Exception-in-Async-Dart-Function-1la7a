# Unhandled Exception in Async Dart Function

This repository demonstrates a subtle bug in Dart asynchronous programming: neglecting to rethrow an exception caught within an async function.  The `fetchData` function fetches data from a remote API. If an error occurs, the exception is caught, printed to the console, and then the function continues execution. This is likely not the intended behavior; a more robust approach would be to rethrow the exception, allowing calling functions to handle it appropriately.

The solution demonstrates the correct way to handle exceptions in async functions, ensuring that errors are properly propagated up the call stack.