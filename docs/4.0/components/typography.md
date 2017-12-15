---
layout: docs
title: Typography
description: Documentation and examples for Bootstrap typography, including global settings, headings, body text, lists, and more.
group: content
toc: true
---

## Headings

All HTML headings, `<h1>` through `<h6>`, are available.

<table>
  <thead>
    <tr>
      <th>Heading</th>
      <th>Example</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        {% markdown %}`<h1></h1>`{% endmarkdown %}
      </td>
      <td><span class="h1">h1. Bootstrap heading</span></td>
    </tr>
    <tr>
      <td>
        {% markdown %}`<h2></h2>`{% endmarkdown %}
      </td>
      <td><span class="h2">h2. Bootstrap heading</span></td>
    </tr>
    <tr>
      <td>
        {% markdown %}`<h3></h3>`{% endmarkdown %}
      </td>
      <td><span class="h3">h3. Bootstrap heading</span></td>
    </tr>
    <tr>
      <td>
        {% markdown %}`<h4></h4>`{% endmarkdown %}
      </td>
      <td><span class="h4">h4. Bootstrap heading</span></td>
    </tr>
    <tr>
      <td>
        {% markdown %}`<h5></h5>`{% endmarkdown %}
      </td>
      <td><span class="h5">h5. Bootstrap heading</span></td>
    </tr>
    <tr>
      <td>
        {% markdown %}`<h6></h6>`{% endmarkdown %}
      </td>
      <td><span class="h6">h6. Bootstrap heading</span></td>
    </tr>
  </tbody>
</table>

{% highlight html %}
<h1>h1. Bootstrap heading</h1>
<h2>h2. Bootstrap heading</h2>
<h3>h3. Bootstrap heading</h3>
<h4>h4. Bootstrap heading</h4>
<h5>h5. Bootstrap heading</h5>
<h6>h6. Bootstrap heading</h6>
{% endhighlight %}

`.h1` through `.h6` classes are also available, for when you want to match the font styling of a heading but cannot use the associated HTML element.

{% example html %}
<p class="h1">h1. Bootstrap heading</p>
<p class="h2">h2. Bootstrap heading</p>
<p class="h3">h3. Bootstrap heading</p>
<p class="h4">h4. Bootstrap heading</p>
<p class="h5">h5. Bootstrap heading</p>
<p class="h6">h6. Bootstrap heading</p>
{% endexample %}

### Customizing headings

Use the included utility classes to recreate the small secondary heading text from Bootstrap 3.

<div class="bd-example">
  <span class="h3">
    Fancy display heading
    <small class="text-muted">With faded secondary text</small>
  </span>
</div>

{% highlight html %}
<h3>
  Fancy display heading
  <small class="text-muted">With faded secondary text</small>
</h3>
{% endhighlight %}

## Blockquotes

For quoting blocks of content from another source within your document. Wrap `<blockquote class="blockquote">` around any <abbr title="HyperText Markup Language">HTML</abbr> as the quote.

{% example html %}
<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
</blockquote>
{% endexample %}

### Naming a source

Add a `<footer class="blockquote-footer">` for identifying the source. Wrap the name of the source work in `<cite>`.

{% example html %}
<blockquote class="blockquote">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
{% endexample %}

### Alignment

Use text utilities as needed to change the alignment of your blockquote.

{% example html %}
<blockquote class="blockquote text-center">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
{% endexample %}

{% example html %}
<blockquote class="blockquote text-right">
  <p class="mb-0">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
  <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
</blockquote>
{% endexample %}

If you want to see more examples and properties please check the official [Bootstrap Documentation](http://getbootstrap.com/docs/4.0/components/typography/)
