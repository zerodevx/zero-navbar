v0.1.1

# `<zero-navbar>`

Auto-hiding top navigation bar. A Polymer 1.2+ web component to create a top
horizontal toolbar that reveals itself only when a quick upward scroll is
detected.

It's super lightweight, responsive and animated.


### Let's get this money

Use like:

```html
<style>
  zero-navbar {
    /* If not defined, header height defaults to 50px */
    height: 100px;
    background-color: blue;
  }
</style>

<zero-navbar shadow offset="400px" sensitivity="50">

  <!-- Align my logo to left -->
  <img class="zero-navbar-left" src="logo.jpg">

  <!-- These are aligned to right -->
  <div class="my-menu-link">HOME</div>
  <div class="my-menu-link">ABOUT</div>
  <div class="my-menu-link">CONTACT</div>

</zero-navbar>
```


### Demo

Try [this](https://rawgit.com/zerodevx/zero-navbar/master/demo/demo.html).


### Published properties

| Property    | Type    | Description |
|-------------|---------|-------------|
| reveal      | Boolean | Set or get navbar reveal status. |
| shadow      | Boolean | Displays a drop-shadow effect under navbar. Defaults to false. |
| offset      | Number  | Starts the navbar only after document has been scrolled by distance of `offset` in px. |
| duration    | Number  | Duration of slide up/down animation in ms. Set to 0 to disable. Defaults to 500. |
| disableAuto | Boolean | Disables automatic reveal of the navbar when a fast upward scroll is detected. |
| sensitivity | Number  | Smaller to increase sensitivity, larger to decrease. Defaults to 100. |


### Version history

1. 2015-11-30: v0.1.0
  * Initial implementation.

