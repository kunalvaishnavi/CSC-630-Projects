The purpose of this lab was to demonstrate the normal distribution in a histogram. Here was the lab background from our course page:

A histogram is a univariate visualization --- that means that it only displays information about one variable, or column, of data. The idea behind a histogram is to take your column of data and break its range into distinct bins, and to create a count of all the samples (or rows) that lie in each bin. You then plot those counts, rather than the data itself. This gives a rough approximation to the distribution of the data, i.e. if you were to collect larger and larger samples of this data, how the limiting shape would appear.

Now, in JavaScript, one can create a random number by using Math.random(). This will generate a number between 0 and 1, uniformly. 
Hence the histogram your create will approximate the uniform distribution However, the Central Limit Theorem says (among other things) 
that we can use this to approximate another important distribution: the normal distribution. Here's how: if you generate 2 random numbers
in this way, and add them together, then they're a number between 0 and 2, but more likely to be closer to 1 (Think about rolling two 
dice and summing their outputs; you're much more likely to get a 7 than a 1). So divide by 2, and you've got a number that's randomly 
generated between 0 and 1, but has a better chance of being near 0.5. Great, now generate 3 numbers and add them, and divide by 3 instead.
Now 4...etc. The more numbers you add, the more closely you approximate the normal distribution. Our histogram will demonstrate this 
phenomenon.
