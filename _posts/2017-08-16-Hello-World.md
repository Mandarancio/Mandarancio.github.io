---
layout: post
title: Up and running... Maybe
---

I'm keeping this diary to keep up with my work for the master project.
The idea is to find better and contextual image compression algorithms.
The first results however are not very promising...

Using the CELEBA data set I tried 2 different methods of compressions, first create a compression mask by averaging 1000 dct trasformation of the data set (to keep the *k* highest avarage components), then I tried to find few cluster (~20) from the 1000 dct transformations and find the more similar to the actual image to compress. 

![Mse]({{ site.baseurl }}/images/log_plot_20clusters.png)

On the *y* axis there is the log of the *mse* and the *x* axis is the number of components stored.
