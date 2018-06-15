# functime
## install
```
pip install functime
```
## usage
```python
import functime

func_time(sorted, [5,4,3,2,1])
```
out:
```
sorted AVG(1000000): 0.537999us
```
## api
This moudle provides a simple way to time a function.
* func_time(func, *args, **kwargs):
  Time func with arguments.Run repeatedly with times set to (10, 100, 1000, ...) until the total time >= 0.2s. Print average run time with readable format.