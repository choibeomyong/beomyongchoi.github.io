---
layout: post
title: "image saving in django"
description: "simple image"
og_image: "documentation/sample-image.jpg"
tags: [design, jekyll]
---



{% highlight python %}
from PIL import Image
import requests
from io import BytesIO

response = requests.get(url)
img = Image.open(BytesIO(response.content))
{% endhighlight %}

