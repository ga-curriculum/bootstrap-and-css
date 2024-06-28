# ![Bootstrap and CSS - Components that Use JavaScript](./assets/components-that-use-javascript.png)

**Learning objective:** By the end of this lesson, students will be able to implement JavaScript-dependent Bootstrap components, such as the mobile navbar with a hamburger menu, ensuring proper integration of Bootstrap’s JS dependencies. 

## Components that Use JavaScript
Many complicated Bootstrap components rely on JavaScript because they are animated. One prominent example that you can find everywhere on the Internet is the infamous hamburger menu on sliding mobile navbars.

You can bring in a navbar from Bootstrap's [component library](https://getbootstrap.com/docs/5.2/examples/#snippets) (this is the navbar that was in the `index.html` file). Notice the many nested divs and bootstrap classes on several elements.
```html
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
      <div class="navbar-nav">
        <a class="nav-link active" aria-current="page" href="#">Home</a>
        <a class="nav-link" href="#">Features</a>
        <a class="nav-link" href="#">Pricing</a>
        <a class="nav-link disabled">Disabled</a>
      </div>
    </div>
  </div>
</nav>
```
A common mistake is to bring in this Navbar without connecting to Bootstrap's JS dependencies. Additionally, the Hamburger Icon will only show up on mobile views and will be hidden on larger screen sizes. With complex Bootstrap components, you should read documentation how to customize elements properly.

