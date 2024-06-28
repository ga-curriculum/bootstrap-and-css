# ![Bootstrap and CSS - Layout System](./assets/bootstrap-and-css-layoutsystem.png)

**Learning objective:** By the end of this lesson, students will be able to utlize Bootstrap's 12-column grid system to create responsive layouts, using containeres, row, and breakpoint classes.

## Bootstrap Layout System
Bootstap applies default styles to most built-in HTML tags, but it also uses several class-based styles to give it that signature Bootstrap look. Let's check out the Bootstrap layout system!


### Containing Divs
Bootstrap uses Flexbox and Grid underneath the hood to create its own 12-column layout system. Remember: **the magic number in Bootstrap Layouts is 12**.

To begin using Bootstrap's layout system, we first need a `div` with a class of `container`. Inside this div, we also need a div with a class of `row`. Clear out all the elements inside the `body` tag and replace it with the following:
```html
<div class="container">
    <div class="row">
    </div>
</div>
```
These two nested divs act as the containing elements. Now, let's bring in one of the components for Bootstrap to demonstrate how the layout system can be used to arrange elements easily.

You can bring in Bootstrap Components into your project by selecting what you need from the sidebar. Cards are a common UX component on many websites with helpful information. Let's use Bootstrap's version of a Card to demonstrate Bootstrap Layout.

Here is a Bootstrap Card:
```html
<div class="card">
    <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
        <a href="#" class="card-link">Card link</a>
        <a href="#" class="card-link">Another link</a>
    </div>
</div>
```
Copy and paste two of these card elements INSIDE the `div` with class `row` we made earlier.

So, inside your `body` tag, your HTML should look like this:
```html
<div class="container">
    <div class="row">
        <div class="card">
            <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the
                    card's content.</p>
                <a href="#" class="card-link">Card link</a>
                <a href="#" class="card-link">Another link</a>
            </div>
        </div>
        <div class="card">
            <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <h6 class="card-subtitle mb-2 text-muted">Card subtitle</h6>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the
                    card's content.</p>
                <a href="#" class="card-link">Card link</a>
                <a href="#" class="card-link">Another link</a>
            </div>
        </div>
    </div>
</div>
```
Great! Now, let's arrange these cards and make them mobile-friendly too!


### Columns and Built-In Breakpoints
Remember how we emphasized that 12 is the magic number? The number of columns across the containg divs should always add up to 12.

In general, to determine how many columns a Bootstrap component should cover, we use a class name like this:
```css
col-SIZE-NUMBER
```

For size, we can use these built-in breakpoints:
- SM
- MD
- LG

1. And for number, any number from 1-12 will work.
1. An element can also contain multiple column classes to change its appearance between different screen sizes.
    1. For example a `div` with both `col-md-6` and `col-sm-3` will take up 6 columns on medium-sized screens and up, but will take up 3 columns across on small-sized screens and smaller.
1. Add `col-md-6` as a class to both Card elements inside of their opening `div` tags. Notice how their layout is effected.
1. Let's add a third card, and change the `col-md-*` class to have three cards across.

