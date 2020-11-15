# Canvas Discussion Assignment 4
## Process
I started this assignment by playing around with the feature.canny feature set representation. This was the default feature set representation for this assignment. I tested out several different sigma values to see if this would have any effect on performance.

I tested the default sigma, sigma=1.5, sigma=0.5, and sigma=1.3. The multilayer perceptron TP test rate went up for sigma=1.5 compared to the default, but the perceptron TP test rate went down. Both the perceptron and multilayer perceptron did worse for sigma=0.5. At this point, I noticed that the perceptron model was doing best for all of these and I concluded that a sigma value between 1.0 and 1.5 would do the best. I tested out multiple sigma values in between 1.0 and 1.5. For sigma=1.3, neither the perceptron nor the multilayer perceptron did better than the default sigma. None of the other values between 1.0 and 1.5 did better than the default either, so I concluded that the default value of sigma was the best.

If I decide to use feature.canny for my final iteration, I will use the default sigma and the perceptron model.

I have included the images of my tests below:

![](Feature.canny.png)
