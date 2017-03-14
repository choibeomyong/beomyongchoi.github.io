---
layout: post
title: "Load Images from Image's src in Python"
description: "images in python"
tags: [python]
---

This document is based on __python 3__. Before you follow this, you need _PIL_,

`pip3 install PIL`

and this is code:
{% highlight python %}
from PIL import Image
from urllib.request import urlopen
from io import BytesIO

response = urlopen(url).read()
img = Image.open(BytesIO(response))
{% endhighlight %}

if you use __python 2.7__

{% highlight python %}
from PIL import Image
from urllib import urlopen # this part is differnt
from io import BytesIO

response = urlopen(url).read()
img = Image.open(BytesIO(response))
{% endhighlight %}
