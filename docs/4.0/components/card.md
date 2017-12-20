---
layout: docs
title: Cards
description: Bootstrap's cards provide a flexible and extensible content container with multiple variants and options.
group: components
toc: true
---

## About

A **card** is a flexible and extensible content container. It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options. If you're familiar with Bootstrap 3, cards replace our old panels, wells, and thumbnails. Similar functionality to those components is available as modifier classes for cards.

## Example

Cards are built with as little markup and styles as possible, but still manage to deliver a ton of control and customization. Built with flexbox, they offer easy alignment and mix well with other Bootstrap components. They have no `margin` by default, so use [spacing utilities]({{ site.baseurl }}/docs/{{ site.docs_version }}/utilities/spacing/) as needed.

Below is an example of a basic card with mixed content and a fixed width. Cards have no fixed width to start, so they'll naturally fill the full width of its parent element. This is easily customized with our various [sizing options](#sizing).

{% example html %}
<div class="card" style="width: 20rem;">
  <img class="card-img-top" data-src="holder.js/100px180/" alt="Card image cap">
  <div class="card-body">
    <h4 class="card-title">Card title</h4>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
{% endexample %}

## Content types

Cards support a wide variety of content, including images, text, list groups, links, and more. Below are examples of what's supported.

### Body

The building block of a card is the `.card-body`. Use it whenever you need a padded section within a card.

{% example html %}
<div class="card">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>
{% endexample %}

### Titles, text, and links

Card titles are used by adding `.card-title` to a `<h*>` tag. In the same way, links are added and placed next to each other by adding `.card-link` to an `<a>` tag.

Subtitles are used by adding a `.card-subtitle` to a `<h*>` tag. If the `.card-title` and the `.card-subtitle` items are placed in a `.card-body` item, the card title and subtitle are aligned nicely.

{% example html %}
<div class="card" style="width: 20rem;">
  <div class="card-body">
    <h4 class="card-title">Card title</h4>
    <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="card-link">Card link</a>
    <a href="#" class="card-link">Another link</a>
  </div>
</div>
{% endexample %}

### Images

`.card-img-top` places an image to the top of the card. With `.card-text`, text can be added to the card. Text within `.card-text` can also be styled with the standard HTML tags.

{% example html %}
<div class="card" style="width: 20rem;">
  <img class="card-img-top" data-src="holder.js/100px180/?text=Image cap" alt="Card image cap">
  <div class="card-body">
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
  </div>
</div>
{% endexample %}

### List groups

Create lists of content in a card with a flush list group.

{% example html %}
<div class="card" style="width: 20rem;">
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>
{% endexample %}

{% example html %}
<div class="card card-nav-tabs" style="width: 20rem;">
  <div class="card-header card-header-danger">
    Featured  
  </div>
  <ul class="list-group list-group-flush">
    <li class="list-group-item">Cras justo odio</li>
    <li class="list-group-item">Dapibus ac facilisis in</li>
    <li class="list-group-item">Vestibulum at eros</li>
  </ul>
</div>
{% endexample %}

### Header and footer

Add an optional header and/or footer within a card.

{% example html %}
<div class="card card-nav-tabs">
  <div class="card-header card-header-warning">
    Featured
  </div>
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
{% endexample %}

Card headers can be styled by adding `.card-header` to `<h*>` elements.

{% example html %}
<div class="card card-nav-tabs">
  <h4 class="card-header card-header-info">Featured</h4>
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
{% endexample %}

{% example html %}
<div class="card card-nav-tabs">
  <div class="card-header card-header-success">
    Quote
  </div>
  <div class="card-body">
    <blockquote class="blockquote mb-0">
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer posuere erat a ante.</p>
      <footer class="blockquote-footer">Someone famous in <cite title="Source Title">Source Title</cite></footer>
    </blockquote>
  </div>
</div>
{% endexample %}

{% example html %}
<div class="card card-nav-tabs text-center">
  <div class="card-header card-header-primary">
    Featured
  </div>
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
  <div class="card-footer text-muted">
    2 days ago
  </div>
</div>
{% endexample %}

## Text alignment

You can quickly change the text alignment of any card—in its entirety or specific parts—with our [text align classes]({{ site.baseurl }}/docs/{{ site.docs_version }}/utilities/text/#text-alignment).

{% example html %}
<div class="card" style="width: 20rem;">
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card text-center" style="width: 20rem;">
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card text-right" style="width: 20rem;">
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
{% endexample %}

## Navigation

Add some navigation to a card's header (or block) with Bootstrap's [nav components]({{ site.baseurl }}/docs/{{ site.docs_version }}/components/navs/).

{% example html %}
<div class="card text-center">
  <div class="card-header card-header-rose">
    <ul class="nav nav-tabs">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link disabled" href="#">Disabled</a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
{% endexample %}

{% example html %}
<div class="card text-center">
  <div class="card-header">
    <ul class="nav nav-pills card-header-pills">
      <li class="nav-item">
        <a class="nav-link active" href="#">Active</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
      <li class="nav-item">
        <a class="nav-link disabled" href="#">Disabled</a>
      </li>
    </ul>
  </div>
  <div class="card-body">
    <h4 class="card-title">Special title treatment</h4>
    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
{% endexample %}

## Images

Cards include a few options for working with images. Choose from appending "image caps" at either end of a card, overlaying images with card content, or simply embedding the image in a card.

### Image caps

Similar to headers and footers, cards can include top and bottom "image caps"—images at the top or bottom of a card.

{% example html %}
<div class="card mb-3">
  <img class="card-img-top" data-src="holder.js/100px180/" alt="Card image cap">
  <div class="card-body">
    <h4 class="card-title">Card title</h4>
    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
    <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
  </div>
</div>
<div class="card">
  <div class="card-body">
    <h4 class="card-title">Card title</h4>
    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
    <p class="card-text"><small class="text-muted">Last updated 3 mins ago</small></p>
  </div>
  <img class="card-img-bottom" data-src="holder.js/100px180/" alt="Card image cap">
</div>
{% endexample %}

### Image overlays

Turn an image into a card background and overlay your card's text. Depending on the image, you may or may not need additional styles or utilities.

{% example html %}
<div class="card bg-dark text-white">
  <img class="card-img" data-src="holder.js/100px270/#55595c:#373a3c/text:Card image" alt="Card image">
  <div class="card-img-overlay">
    <h4 class="card-title">Card title</h4>
    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
    <p class="card-text">Last updated 3 mins ago</p>
  </div>
</div>
{% endexample %}

## Examples

### Blog Cards

{% example html %}

<div class="card card-blog">
    <div class="card-header card-header-image">
        <a href="#pablo">
            <img class="img" src="https://images.unsplash.com/photo-1511439817358-bee8e21790b5?auto=format&fit=crop&w=750&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
            <div class="card-title">
                This Summer Will be Awesome
            </div>
        </a>
    </div>
    <div class="card-body">
        <h6 class="card-category text-info">Fashion</h6>
        <p class="card-description">
            Don&apos;t be scared of the truth because we need to restart the human foundation in truth And I love you like Kanye loves Kanye I love Rick Owens&#x2019; bed design but the back is...
        </p>
    </div>
</div>
{% endexample %}

{% example html %}

  <div class="card">
      <div class="card-body bg-info">
          <h5 class="card-category card-category-social">
              <i class="fa fa-twitter"></i> Twitter
          </h5>
          <h4 class="card-title">
              <a href="#pablo">&quot;You Don&apos;t Have to Sacrifice Joy to Build a Fabulous Business and Life&quot;</a>
          </h4>

          <div class="card-stats">
              <div class="author">
                  <a href="#pablo">
                     <img src="https://images.unsplash.com/photo-1476493279419-b785d41e38d8?auto=format&fit=crop&w=750&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D" alt="..." class="avatar img-raised">
                     <span>Tania Andrew</span>
                  </a>
              </div>
             <div class="stats ml-auto">
                  <i class="material-icons">favorite</i> 2.4K &#xB7;
                  <i class="material-icons">share</i> 45
              </div>
          </div>
      </div>
  </div>

{% endexample %}

{% example html %}

<div class="card">
  <div class="card-body ">
        <h6 class="card-category text-danger">
            <i class="material-icons">trending_up</i> Trending
        </h6>
        <h4 class="card-title">
            <a href="#pablo">To Grow Your Business Start Focusing on Your Employees</a>
        </h4>

    </div>
    <div class="card-footer ">
            <div class="author">
                <a href="#pablo">
                   <img src="https://images.unsplash.com/photo-1506794778202-cad84cf45f1d?auto=format&fit=crop&w=334&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D" alt="..." class="avatar img-raised">
                   <span>Lord Alex</span>
                </a>
            </div>
           <div class="stats ml-auto">
                <i class="material-icons">favorite</i> 342 &#xB7;
                <i class="material-icons">chat_bubble</i> 45
            </div>
        </div>
      </div>
{% endexample %}


### Profile Card

{% example html %}


<div class="card card-profile">
  <div class="card-header card-header-image">
        <a href="#pablo">
            <img class="img" src="https://images.unsplash.com/photo-1492447273231-0f8fecec1e3a?auto=format&fit=crop&w=334&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D">
        </a>
    </div>

    <div class="card-body ">
        <h4 class="card-title">Alec Thompson</h4>
        <h6 class="card-category text-gray">CEO / Co-Founder</h6>
    </div>
    <div class="card-footer justify-content-center">
        <a href="#pablo" class="btn btn-just-icon btn-link">
            <i class="fa fa-twitter"></i>
        </a>
        <a href="#pablo" class="btn btn-just-icon btn-facebook btn-round">
            <i class="fa fa-facebook-square"></i>
        </a>
        <a href="#pablo" class="btn btn-just-icon btn-google btn-round">
            <i class="fa fa-google"></i>
        </a>
    </div>
</div>
{% endexample %}

### Full Background Card

{% example html %}

<div class="card card-background" style="background-image: url('https://images.unsplash.com/photo-1497366811353-6870744d04b2?auto=format&fit=crop&w=750&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D')">
  <div class="card-body">
    <h6 class="card-category text-info">Productivy Apps</h6>
    <a href="#pablo">
      <h3 class="card-title">The Best Productivity Apps on Market</h3>
      </a>
      <p class="card-description">
      Don't be scared of the truth because we need to restart the human foundation in truth And I love you like Kanye loves Kanye I love Rick Owens’ bed design but the back is...
      </p>
    <a href="#pablo" class="btn btn-white btn-link">
      <i class="material-icons">subject</i> Read Article
    </a>
    <a href="#pablo" class="btn btn-white btn-link">
      <i class="material-icons">watch_later</i> Watch Later
    </a>
  </div>
</div>

{% endexample %}

### Pricing Card

{% example html %}

<div class="card card-pricing"><div class="card-body bg-primary">
  <div class="icon">
      <i class="material-icons">business</i>
  </div>
  <h3 class="card-title">$69</h3>
  <p class="card-description">
      This is good if your company size is between 11 and 99 Persons.
  </p>
  <a href="#pablo" class="btn btn-white btn-round">Choose Plan</a>
  </div>
</div>

{% endexample %}

### Rotating Card

{% example html %}

<div class="rotating-card-container">
    <div class="card card-rotate card-background">
        <div class="front front-background" style="background-image:url('https://images.unsplash.com/photo-1493787039806-2edcbe808750?auto=format&fit=crop&w=750&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D');">
            <div class="card-body">
                <h6 class="card-category">Full Background Card</h6>
                <a href="#pablo">
                    <h3 class="card-title">This Background Card Will Rotate on Hover</h3>
                </a>
                <p class="card-description">
                    Don't be scared of the truth because we need to restart the human foundation in truth And I love you like Kanye loves Kanye I love Rick Owens’ bed design but the back is...
                </p>
            </div>
        </div>

        <div class="back back-background" style="background-image: url('https://images.unsplash.com/photo-1493787039806-2edcbe808750?auto=format&fit=crop&w=750&q=80&ixid=dW5zcGxhc2guY29tOzs7Ozs%3D');">
            <div class="card-body">
                <h5 class="card-title">
                    Manage Post
                </h5>
                <p class="card-description">As an Admin, you have shortcuts to edit, view or delete the posts.</p>
                <div class="footer text-center">
                    <a href="#pablo" class="btn btn-info btn-just-icon btn-fill btn-round">
                        <i class="material-icons">subject</i>
                    </a>
                    <a href="#pablo" class="btn btn-success btn-just-icon btn-fill btn-round btn-wd">
                        <i class="material-icons">mode_edit</i>
                    </a>
                    <a href="#pablo" class="btn btn-danger btn-just-icon btn-fill btn-round">
                        <i class="material-icons">delete</i>
                    </a>
                </div>
            </div>
        </div>
    </div>
</div>

{% endexample %}
