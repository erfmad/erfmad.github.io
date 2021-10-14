Hello and welcome to this blog. 
---
layout: default
title: Home
---
<div class="l-page series">
<h3 class="series-title">Implementing Convolutional Neural Networks</h3>
<p>
<a href="/implementing-cnn">Implementing Convolutional Neural Networks</a> is a series of posts to understand the concepts and mathematics behind Convolutinal Neural Networks and implement your own CNN in Python and Numpy. Complete source code can be found here: <a href="https://github.com/parasdahal/deepnet">https://github.com/parasdahal/deepnet</a>.
</p>
</div>
<hr>
<div class="posts-list l-page">
  <!--<h2 class="post-tag">Latest Articles</h2>-->
  {% for post in paginator.posts %}
  <div class="post-preview">
    <div class="metadata">
            <div>{{ post.date | date: "%b %d, %Y" }}</div><br/>

             {% for cat in post.categories %}<a href="/category/{{cat}}">{{cat}}</a><br/>{% endfor %}
    </div>
    <div class="thumbnail"><img src="{{post.thumbnail}}"></div>
    <div class="description">
      <a href="{{ post.url }}"><h2 class="post-title">{{ post.title }}</h2></a>
      <p>{{ post.excerpt }}</p>
    </div>
  </div>
  {% endfor %}
</div>
</div>

