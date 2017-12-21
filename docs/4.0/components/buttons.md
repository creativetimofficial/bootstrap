---
layout: docs
title: Buttons
description: Use Bootstrap's custom button styles for actions in forms, dialogs, and more with support for multiple sizes, states, and more.
group: components
redirect_from: "/docs/4.0/components/"
toc: true
---

## Examples

Bootstrap includes several predefined button styles, each serving its own semantic purpose, with a few extras thrown in for more control.

{% example html %}
{% for color in site.data.theme-colors %}
<button type="button" class="btn btn-{{ color.name }}">{{ color.name | capitalize }}</button>{% endfor %}

{% endexample %}

## Style buttons

{% example html %}
<button class="btn btn-primary">Default</button>
<button class="btn btn-primary btn-round">Round</button>
<button class="btn btn-primary btn-round">
  <i class="material-icons">favorite</i> With Icon
</button>
<button class="btn btn-primary btn-fab btn-fab-mini btn-round">
  <i class="material-icons">favorite</i>
</button>
<button class="btn btn-primary btn-link">Simple</button>
{% endexample %}

## Sizes

Fancy larger or smaller buttons? Add `.btn-lg` or `.btn-sm` for additional sizes.

{% example html %}
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary">Regular</button>
<button class="btn btn-primary btn-lg">Large</button>
{% endexample %}

## Social Buttons

{% example html %}

<div class="row">
   <div class="col-md-3 social-buttons-demo">
     <h3><small> Default </small></h3>
    <button class="btn btn-social btn-fill btn-twitter">
      <i class="fa fa-twitter"></i> Connect
    </button><br>
    <button class="btn btn-social btn-fill btn-facebook">
      <i class="fa fa-facebook-square"></i> Share &middot; 2.2k
    </button><br>
    <button class="btn btn-social btn-fill btn-google">
      <i class="fa fa-google-square"></i> Share on Google+
    </button><br>
    <button class="btn btn-social btn-fill btn-linkedin">
      <i class="fa fa-linkedin-square"></i> Connect
    </button><br>
    <button class="btn btn-social btn-fill btn-pinterest">
      <i class="fa fa-pinterest"></i> Pint it &middot; 212
    </button><br>
    <button class="btn btn-social btn-fill btn-youtube">
      <i class="fa fa-youtube-play"></i> View
    </button><br>
    <button class="btn btn-social btn-fill btn-tumblr">
      <i class="fa fa-tumblr-square"></i> Repost
    </button><br>
    <button class="btn btn-social btn-fill btn-github">
      <i class="fa fa-github"></i> Connect
    </button><br>
    <button class="btn btn-social btn-fill btn-behance">
      <i class="fa fa-behance-square"></i> Follow us
    </button><br>
    <button class="btn btn-social btn-fill btn-dribbble">
      <i class="fa fa-dribbble"></i> Find us
    </button><br>
    <button class="btn btn-social btn-fill btn-reddit">
      <i class="fa fa-reddit"></i> Repost &middot; 232
    </button><br>
   </div>
   <div class="col-md-1 social-buttons-demo">
   <h3><small>&nbsp;</small></h3>
    <button class="btn btn-just-icon btn-twitter">
      <i class="fa fa-twitter"></i>
    </button><br>
    <button class="btn btn-just-icon  btn-facebook">
      <i class="fa fa-facebook"> </i>
    </button><br>
    <button class="btn btn-just-icon  btn-google">
      <i class="fa fa-google"> </i>
    </button><br>
    <button class="btn btn-just-icon  btn-linkedin">
      <i class="fa fa-linkedin"></i>
    </button><br>
    <button class="btn btn-just-icon  btn-pinterest">
      <i class="fa fa-pinterest"></i>
    </button><br>
    <button class="btn btn-just-icon  btn-youtube">
      <i class="fa fa-youtube"> </i>
    </button><br>
    <button class="btn btn-just-icon  btn-tumblr">
      <i class="fa fa-tumblr"> </i>
    </button><br>
    <button class="btn btn-just-icon  btn-github">
      <i class="fa fa-github"></i>
    </button><br>
    <button class="btn btn-just-icon  btn-behance">
      <i class="fa fa-behance"></i>
    </button><br>
    <button class="btn btn-just-icon  btn-dribbble">
      <i class="fa fa-dribbble"></i>
    </button><br>
    <button class="btn btn-just-icon  btn-reddit">
      <i class="fa fa-reddit"></i>
    </button><br>
   </div>
   <div class="col-md-1 social-buttons-demo">
     <h3><small>&nbsp;</small></h3>
    <button class="btn btn-just-icon btn-round btn-twitter">
      <i class="fa fa-twitter"></i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-facebook">
      <i class="fa fa-facebook"> </i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-google">
      <i class="fa fa-google"> </i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-linkedin">
      <i class="fa fa-linkedin"></i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-pinterest">
      <i class="fa fa-pinterest"></i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-youtube">
      <i class="fa fa-youtube"> </i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-tumblr">
      <i class="fa fa-tumblr"> </i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-github">
      <i class="fa fa-github"></i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-behance">
      <i class="fa fa-behance"></i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-dribbble">
      <i class="fa fa-dribbble"></i>
    </button><br>
    <button class="btn btn-just-icon btn-round btn-reddit">
      <i class="fa fa-reddit"></i>
    </button><br>
   </div>
   <div class="col-md-1 social-buttons-demo">
     <h3><small>Simple</small></h3>
    <button class="btn btn-link btn-twitter">
      <i class="fa fa-twitter"></i>
    </button><br>
    <button class="btn btn-link btn-facebook">
      <i class="fa fa-facebook-square"> </i>
    </button><br>
    <button class="btn btn-link btn-google">
      <i class="fa fa-google"> </i>
    </button><br>
    <button class="btn btn-link btn-linkedin">
      <i class="fa fa-linkedin-square"></i>
    </button><br>
    <button class="btn btn-link btn-pinterest">
      <i class="fa fa-pinterest"></i>
    </button><br>
    <button class="btn btn-link btn-youtube">
      <i class="fa fa-youtube"> </i>
    </button><br>
    <button class="btn btn-link btn-tumblr">
      <i class="fa fa-tumblr-square"> </i>
    </button><br>
    <button class="btn btn-link btn-github">
      <i class="fa fa-github"></i>
    </button><br>
    <button class="btn btn-link btn-behance">
      <i class="fa fa-behance"></i>
    </button><br>
    <button class="btn btn-link btn-dribbble">
      <i class="fa fa-dribbble"></i>
    </button><br>
    <button class="btn btn-link btn-reddit">
      <i class="fa fa-reddit"></i>
    </button><br>
   </div>
   <div class="col-md-3 social-buttons-demo">
     <h3><small>&nbsp;</small></h3>
    <button class="btn btn-link btn-twitter">
      <i class="fa fa-twitter"></i> Connect
    </button><br>
    <button class="btn btn-link btn-facebook">
      <i class="fa fa-facebook-square"></i> Share &middot; 2.2k
    </button><br>
    <button class="btn btn-link btn-google">
      <i class="fa fa-google-square"></i> Share on Google+
    </button><br>
    <button class="btn btn-link btn-linkedin">
      <i class="fa fa-linkedin-square"></i> Connect
    </button><br>
    <button class="btn btn-link btn-pinterest">
      <i class="fa fa-pinterest"></i> Pint it &middot; 212
    </button><br>
    <button class="btn btn-link btn-youtube">
      <i class="fa fa-youtube-play"></i> View
    </button><br>
    <button class="btn btn-link btn-tumblr">
      <i class="fa fa-tumblr-square"></i> Repost
    </button><br>
    <button class="btn btn-link btn-github">
      <i class="fa fa-github"></i> Connect
    </button><br>
    <button class="btn btn-link btn-behance">
      <i class="fa fa-behance-square"></i> Follow us
    </button><br>
    <button class="btn btn-link btn-dribbble">
      <i class="fa fa-dribbble"></i> Find us
    </button><br>
    <button class="btn btn-link btn-reddit">
      <i class="fa fa-reddit"></i> Repost &middot; 232
    </button><br>
   </div>
</div>

{% endexample %}
## Disabled state

Make buttons look inactive by adding the `disabled` boolean attribute to any `<button>` element.

{% example html %}
<button type="button" class="btn btn-lg btn-primary" disabled>Primary button</button>
<button type="button" class="btn btn-secondary btn-lg" disabled>Button</button>
{% endexample %}

Disabled buttons using the `<a>` element behave a bit different:

- `<a>`s don't support the `disabled` attribute, so you must add the `.disabled` class to make it visually appear disabled.
- Some future-friendly styles are included to disable all `pointer-events` on anchor buttons. In browsers which support that property, you won't see the disabled cursor at all.
- Disabled buttons should include the `aria-disabled="true"` attribute to indicate the state of the element to assistive technologies.

{% example html %}
<a href="#" class="btn btn-primary btn-lg disabled" role="button" aria-disabled="true">Primary link</a>
<a href="#" class="btn btn-secondary btn-lg disabled" role="button" aria-disabled="true">Link</a>
{% endexample %}

{% callout warning %}
#### Link functionality caveat

The `.disabled` class uses `pointer-events: none` to try to disable the link functionality of `<a>`s, but that CSS property is not yet standardized. In addition, even in browsers that do support `pointer-events: none`, keyboard navigation remains unaffected, meaning that sighted keyboard users and users of assistive technologies will still be able to activate these links. So to be safe, add a `tabindex="-1"` attribute on these links (to prevent them from receiving keyboard focus) and use custom JavaScript to disable their functionality.
{% endcallout %}

### Toggle states

Add `data-toggle="button"` to toggle a button's `active` state. If you're pre-toggling a button, you must manually add the `.active` class **and** `aria-pressed="true"` to the `<button>`.

{% example html %}
<button type="button" class="btn btn-primary" data-toggle="button" aria-pressed="false" autocomplete="off">
  Single toggle
</button>
{% endexample %}

If you want to see more examples and properties please check the official [Bootstrap Documentation](http://getbootstrap.com/docs/4.0/components/buttons/)
