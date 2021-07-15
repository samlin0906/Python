# Asyncio — Asynchronous I/O
asyncio is a library to write concurrent code using the async/await syntax.

#Tuple

Tuples are immutable sequences, typically used to store collections of heterogeneous data

#Tasks

asyncio.gather(*aws, loop=None, return_exceptions=False)
Run awaitable objects in the aws sequence concurrently.

asyncio.add_done_callback(callback, *, context=None)
Add a callback to be run when the Task is done.

#Event Loop

The event loop is the core of every asyncio application. 
Event loops run asynchronous tasks and callbacks, perform network IO operations, and run subprocesses.

asyncio.get_event_loop()
Get the current event loop.

loop.run_until_complete(future)
Run until the future (an instance of Future) has completed.

loop.close()
Close the event loop.

#Future

.result()
Return the result of the Future.
If the Future is done and has a result set by the set_result() method, the result value is returned.
