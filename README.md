# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart applications involving the decoding of JSON data.  The provided code snippet shows how a `FormatException` can occur if the JSON response is invalid, leading to application crashes.  The solution provides a robust way to handle this potential exception.

## Bug Description:

The original `fetchData` function attempts to decode a JSON response without error handling. If the server returns an invalid JSON structure or a non-JSON response, `jsonDecode` throws a `FormatException`, causing the application to crash. 

## Solution:

The solution incorporates a `try-catch` block to gracefully handle the `FormatException`.  This prevents the application from crashing, providing a more robust user experience.