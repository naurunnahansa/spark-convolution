# spark-convolution

0.0 Abstract

The importance of local operators in the context of image processing is important but when attempting to run such an operation, as easy as it sounds, turns out to be a nightmare in the context of processing data with maps, reduces and shuffles. In this small article it will describe how to run a local operator in a straightforward way taking a simple convolution operation as an example.

1.0 The Basic Idea

Put simply, the idea behind running a local operator in the context of spark is to group your data by what is required for your local operator to get an output and doing a reduce on the group of data however you choose to do it.

