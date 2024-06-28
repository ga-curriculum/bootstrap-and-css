# ![Bootstrap and CSS - Overwriting Bootstrap Default Style](./assets/overwriting-bootstrap-default-style.png)

**Learning objective:** By the end of this lesson, students will be able to apply CSS to modify and enhance default Bootstrap styles, exploring how to customize button appearances and overall design to distinguish your site from commonly used Bootstrap themes.

## Overwriting Bootstrap Default Styles
With our own CSS Styles, we override default Bootstrap styles if want a more customized look. As an example, let's bring in a form with several buttons.
```html
<form>
  <div class="mb-3">
    <label for="exampleInputEmail1" class="form-label">Email address</label>
    <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
    <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
  </div>
  <div class="mb-3">
    <label for="exampleInputPassword1" class="form-label">Password</label>
    <input type="password" class="form-control" id="exampleInputPassword1">
  </div>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1">
    <label class="form-check-label" for="exampleCheck1">Check me out</label>
  </div>
  <button type="submit" class="btn btn-primary">Submit</button>
</form>
```
Notice the classes on the buttons are `btn` and `btn-primary`.

Create a `main.css` file and write a new color we want for `.btn-primary,` which is the color most buttons will take.
```css
.btn-primary {
    background-color: WHATEVER YOU WANT
}
```
Here are some popular button customizations that many people use with bootstrap:
1. Sharp Corners:
    ```css
    .btn {
        border-radius: 0
    }
    ```
1. Pill Shape:
    ```css
    .btn {
        border-radius: 50px
    }
    ```


## Avoid the Bootstrap Default Look
Once you start using Bootstrap, you might start to notice how prevalent it is on the Internet. In fact, it is an inside joke of how common this look is on Start-up and Corporate Websites: https://www.dagusa.com/

In addition to using your own CSS, several devs have published Bootstrap Themes that overlay on top of Bootstrap's default styles to give a more customized look. 

You can create your own custom color scheme and font-styles for Bootstrap here: https://themestr.app/