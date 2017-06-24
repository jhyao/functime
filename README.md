# timefunc
This moudle provides a simple way to time a function.
* timer(func, times=1)
  Run a function in loop, the number of repeats is given by argument times.Return the total time in seconds.This function can't receive any argument of func. Use func from functools.partial instead.
* timer_auto(func, *args, **kwargs):
  Recommended function.Time func with its arguments followed by func.Call timer(func, times) repeatedly with times set to (10, 100, 1000, ...) so that the total time >= 0.2.Print average run time with readable format.