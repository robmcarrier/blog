---
layout: post
title:  "How to use Yahoo Weatherman gem"
date:   2016-10-03 13:26:25 -0700
categories: Ruby
---
Yahoo Weatherman is a simple gem that allows you to access the Yahoo Weather API in a easy way.  It allows you to search for weather information for any location by using a postal code, city, landmark or any other combination compatible with Yahoo's GeoPlanet.

1.Install the gem.
In you console just enter "gem install yahoo_weatherman".

2.In a ruby file create a new weatherman client.

ex.
{% highlight ruby %}
client = Weatherman::Client.new
{% endhighlight %}

3.Now you can easily look up the temperature or other weather information for a location

ex.
{% highlight ruby %}
client = Weatherman::Client.new
puts client.lookup_by_location("san diego").condition['temp']
{% endhighlight %}

  The console will show the current temp of San Diego.

The gem makes it very easy to implement Yahoo Weather feed API in you ruby projects.
