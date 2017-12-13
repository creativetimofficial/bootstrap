---
layout: docs
title: Badges
description: Documentation and examples for badges, our small count and labeling component.
group: components
toc: true
---

## Example

Badges can be used as part of links or buttons to provide a counter.

{% example html %}
<button type="button" class="btn btn-primary">
  Notifications <span class="badge badge-light">4</span>
</button>
{% endexample %}


## Contextual variations

Add any of the below mentioned modifier classes to change the appearance of a badge.

{% example html %}
{% for color in site.data.theme-colors %}
<span class="badge badge-{{ color.name }}">{{ color.name | capitalize }}</span>{% endfor %}
{% endexample %}

## Pill badges

Use the `.badge-pill` modifier class to make badges more rounded (with a larger `border-radius` and additional horizontal `padding`). Useful if you miss the badges from v3.

{% example html %}
{% for color in site.data.theme-colors %}
<span class="badge badge-pill badge-{{ color.name }}">{{ color.name | capitalize }}</span>{% endfor %}
{% endexample %}

## Links

Using the contextual `.badge-*` classes on an `<a>` element quickly provide _actionable_ badges with hover and focus states.

{% example html %}
{% for color in site.data.theme-colors %}
<a href="#" class="badge badge-{{ color.name }}">{{ color.name | capitalize }}</a>{% endfor %}
{% endexample %}
