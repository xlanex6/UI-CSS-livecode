###Avatar design

```html
<h2>Avatar design</h2>
<img src="http://placehold.it/50x50" alt="" class="avatar">
<img src="http://placehold.it/50x50" alt="" class="avatar-small">
```
```css
.avatar {
  border-radius: 50%;
  width: 50px;
}

.avatar-small {
  border-radius: 50%;
  width: 30px;
}
```

###Button design

```html
<a href="#" class="btn-medium">Write stories</a>
<a href="#" class="btn-treehouse">Start now</a>
```
```css
.btn-medium {
  color: #999999;
  border: 1px solid #999999;
  padding: 10px 15px;
  border-radius: 50px;
  font-weight: lighter;
  opacity: 0.6;
}

.btn-medium:hover {
  opacity: 1;
  text-decoration: none;
  color: #999999;
}

.btn-treehouse {
  color: white;
  padding: 10px 15px;
  border-radius: 4px;
  font-weight: bold;
  background: #6AD58B;
}

.btn-treehouse:hover {
  opacity: 1;
  background: #6AD58B;
  text-decoration: none;
  color: white;
}
```
###Dropdown design

[Bootstrap dropdown direct](http://getbootstrap.com/components/#dropdowns)

```html
<div class="dropdown">
  <img src="http://placehold.it/50x50" alt="" class="avatar dropdown-toggle" id="navbar-menu" data-toggle="dropdown">
  <ul class="dropdown-menu" aria-labelledby="navbar-menu">
    <li><a href="#">Profile</a></li>
    <li><a href="#">Dashboard</a></li>
    <li><a href="#">Logout</a></li>
  </ul>
</div>
```
```css
.dropdown-menu {
  box-shadow: none;
}
.dropdown-menu a {
  font-weight: lighter !important;
  color: #E6E6E6 !important;
}
```

###Card design

Structure first
then
Bootstrap

Card x3

```html
<div class="col-xs-12 col-sm-4">
  <div class="card">
    <img src="http://placehold.it/50x50" alt="" class="avatar card-user">
    <span class="card-category">POPULAR</span>
    <div class="card-description">
      <h3>Stripe</h3>
      <p>A cool payment API</p>
    </div>
  </div>
</div>
```
```css
.card {
  position: relative;
  height: 250px;
  background: linear-gradient(-225deg, rgba(30,30,30,0.6) 30%,
              rgba(46,46,46,0.5) 80%),
              url("http://unsplash.it/400/300/?random");
  background-size: cover;
  color: white;
}

.card-user {
  position: absolute;
  top: 10px;
  right: 10px;
}
.card-category {
  position: absolute;
  top: 10px;
  left: 10px;
}
.card-description {
  position: absolute;
  bottom: 10px;
  left: 10px;
}
```

###Badge design

```html
<img src="http://placehold.it/50x50" alt="" class="avatar">
<span class="badge">3</span>
```
```css
.badge {
  line-height: 20px !important;
  width: 20px !important;
  padding: 0 !important;
  background: #D73B3A !important;
  position: relative !important;
  top: -15px !important;
  left: -15px !important;
}

```

###Banner design

```html
<div class="banner">
  <div class="banner-content">
    <h1>Stripe</h1>
    <p>A cool payment API</p>
    <a href="#" class="btn-treehouse">Start now</a>
  </div>
</div>
```
```css
.banner {
  height: 100vh;
  background: linear-gradient(-225deg, rgba(30,30,30,0.6) 30%,
              rgba(46,46,46,0.5) 80%),
              url("http://unsplash.it/400/300/?random");
  background-size: cover;
  color: white;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.banner h1 {
  font-size: 50px;
  font-weight: bolder;
}

.banner p {
  font-size: 30px;
  font-weight: lighter;
}

```
###Tabs design

```html
<div class="tabs">
  <div class="tabs-item active">
    <h3>350</h3>
    <p>followers</p>
  </div>
  <div class="tabs-item">
    <h3>350</h3>
    <p>followers</p>
  </div>
  <div class="tabs-item">
    <h3>350</h3>
    <p>followers</p>
  </div>
  <div class="tabs-item">
    <h3>350</h3>
    <p>followers</p>
  </div>
</div>
```
```css
.tabs {
  background: #53443F;
  color: white;
  display: flex;
  padding: 10px 10px 0 10px
}

.tabs h3 {
  font-size: 17px;
}

.tabs p {
  opacity: 0.5;
}

.tabs-item {
  background: #756A66;
  flex: 0 0 25%;
  text-align: center;
}

.tabs-item:first-child {
  border-radius: 10px 0 0 0;
}
.tabs-item:last-child {
  border-radius: 0 10px 0 0;
}

.tabs-item.active {
  background: white;
  color: black;
}

```

### List design

```html
<ul class="list-unstyled">
  <li class="product">

    <div class="product-upvote text-center">
      <i class="fa fa-caret-up"></i>
      <p>16</p>
    </div>

    <img src="http://unsplash.it/200/120/?random" alt="" class="product-image img-rounded">

    <div class="product-description">
      <h3>Intercom</h3>
      <p>The best CRM tool.</p>
    </div>

    <ul class="list-inline product-controls">
      <li><a href=""><i class="fa fa-heart"></i></a></li>
      <li><a href=""><i class="fa fa-share"></i></a></li>
      <li><a href=""><i class="fa fa-star"></i></a></li>
    </ul>
  </li>
</ul>

  * 3
```
```css
  .product {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px;
    transition: all 0.3s ease;
    border-radius: 3px;
  }

  .product:hover {
    background: rgb(240, 240, 240);
  }

  .product:hover .product-upvote {
    font-size: 25px;
  }

  .product-upvote {
    font-size: 20px;
    padding: 20px;
    transition: all 0.3s ease;
  }

  .product-description {
    flex: 1 0 auto;
    padding: 20px;
  }
  .product-controls a {
    font-size: 15px;
    color: #CCCCCC;
  }
```
