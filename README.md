# roughsr2
An improved version of roughsr - which was a module for finding support and resistance levels.

# WARNING
Please be aware that this is a very rough piece of code and I take no responsibility for any financial loss that may incur from it's use.

# Improvements on roughsr
Now all you need to do is put your call the function with the single argument of your data as a pandas series object, as opposed to all the frivolous arguments from before. It can also find support and resistance levels for any security, regardless of the price level, and uses a different technique to find those levels than the original model. This new technique has shown to be more accurate.

# Prerequisites
numpy and pandas

# Installation
Clone or download the ZIP file and unpack.
Bring roughsr.py file to the same folder as the project you want to use it in, or put it in your modules folder and make sure that is added to your path.
-from roughsr2 import find_support, find_resistance- in your python file

# Use
Simply import the module and call find_resistance(data) or find_support(data) with your data as a pandas series object (preferably of between 100 and 500 entries), and it will return a series object of the price levels at which resistance or support levels (respectively) were found.

eg:

crsp_resistance = find_resistance(crsp)
crsp
0    19.325333
1    39.125000
2    49.848571
3    52.002917
4    56.334285
5    65.010000
Name: resistance, dtype: float64


