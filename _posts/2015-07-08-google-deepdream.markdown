---
layout: post
title:  "Google DeepDream"
date:   2015-07-08 22:00
summary: The Google DeepDream can be very very deep. You must see this !
categories: other
---
In the last few days, I found [DeepDream](https://github.com/google/deepdream) and I was interested in learning this. So, I decide to make a try to create my own image with DeepDream.

I will explain how to do it the easy way on Ubuntu. First, install the docker.io.

{% highlight html %}sudo apt-get install docker.io{% endhighlight %}

Then, you just need to run this command in your terminal.

###Example{% highlight html %}docker run --rm -v `pwd`/images:/images mjibson/deepdream 'https://www.google.com/logos/2013/zamboni-1005006-hp.jpg' {% endhighlight %}

It can take a few minutes to install and download the docker image.

For more information, you can visit the [mjibson repo](https://github.com/mjibson/ddd). Thanks to him to make the Google DeepDream a lot easier to try.

###Original imageI use the default setting which is ```inception_4c/output```
![Original image]({{ site.url }}/images/google-deepdream/original.jpg)

###Result
![Output image]({{ site.url }}/images/google-deepdream/final.png)
