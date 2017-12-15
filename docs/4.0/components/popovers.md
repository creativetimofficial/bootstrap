---
layout: docs
title: Popovers
description: Documentation and examples for adding Bootstrap popovers, like those found in iOS, to any element on your site.
group: components
toc: true
---

## Static popover

Four options are available: top, right, bottom, and left aligned.

<div class="bd-example bd-example-popover-static">
  <div class="popover bs-popover-top bs-popover-top-docs">
    <div class="arrow"></div>
    <h3 class="popover-header">Popover top</h3>
    <div class="popover-body">
      <p>Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.</p>
    </div>
  </div>

  <div class="popover bs-popover-right bs-popover-right-docs">
    <div class="arrow"></div>
    <h3 class="popover-header">Popover right</h3>
    <div class="popover-body">
      <p>Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.</p>
    </div>
  </div>

  <div class="popover bs-popover-bottom bs-popover-bottom-docs">
    <div class="arrow"></div>
    <h3 class="popover-header">Popover bottom</h3>
    <div class="popover-body">
      <p>Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.</p>
    </div>
  </div>

  <div class="popover bs-popover-left bs-popover-left-docs">
    <div class="arrow"></div>
    <h3 class="popover-header">Popover left</h3>
    <div class="popover-body">
      <p>Sed posuere consectetur est at lobortis. Aenean eu leo quam. Pellentesque ornare sem lacinia quam venenatis vestibulum.</p>
    </div>
  </div>

  <div class="clearfix"></div>
</div>

## Live demo

{% example html %}
<button type="button" class="btn btn-lg btn-danger" data-toggle="popover" title="Popover title" data-content="And here's some amazing content. It's very engaging. Right?">Click to toggle popover</button>
{% endexample %}

### Four directions

<div class="bd-example popover-demo">
  <div class="bd-example-popovers">
    <button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="top" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
      Popover on top
    </button>
    <button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="right" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
      Popover on right
    </button>
    <button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="bottom" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
      Popover on bottom
    </button>
    <button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="left" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
      Popover on left
    </button>
  </div>
</div>

{% highlight html %}
<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="top" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on top
</button>

<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="right" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on right
</button>

<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="bottom" data-content="Vivamus
sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on bottom
</button>

<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="left" data-content="Vivamus sagittis lacus vel augue laoreet rutrum faucibus.">
  Popover on left
</button>
{% endhighlight %}

### Dismiss on next click

Use the `focus` trigger to dismiss popovers on the user's next click of a different element than the toggle element.

{% callout danger %}
#### Specific markup required for dismiss-on-next-click

For proper cross-browser and cross-platform behavior, you must use the `<a>` tag, _not_ the `<button>` tag, and you also must include a [`tabindex`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex) attribute.
{% endcallout %}

{% example html %}
<a tabindex="0" class="btn btn-lg btn-danger" role="button" data-toggle="popover" data-trigger="focus" title="Dismissible popover" data-content="And here's some amazing content. It's very engaging. Right?">Dismissible popover</a>
{% endexample %}

{% highlight js %}
$('.popover-dismiss').popover({
  trigger: 'focus'
})
{% endhighlight %}

If you want to see more examples and properties please check the official [Bootstrap Documentation](http://getbootstrap.com/docs/4.0/components/popovers/)
