# Building Cat Photo App - FreeCodeCamp

This is a practical project from FreeCodeCamp Responsive Web Design

## Heading

There are 6 level of heading, from 1 to 6.

The font is smaller from 1 to 6.

```html
<h1></h1>
<h2></h2>
<h3></h3>
<h4></h4>
<h5></h5>
<h6></h6>
```

## Paragaph

The paragaph tag is used to display paragaph in html

```html
<p></p>
```

## Comment

HTML will ignore the content in the comment, thus will not display it to the screen.

```html
<!-- This is the comment -->
```

## Main

The `main` tag is to declare main section of the document.

```html
<main>
    <h1>Content</h1>
    <p>Content</p>
</main>
```

## Image

Image tag is a self-closed tag. It is used to display image in a html document.

Image has `src` to specify the source, where the image located.

Image has `alt` to display a alternative text when the image cannot display.

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" atl="A cute orange cat lying on its back" >
```

> Cat image from FreeCodeCamp
>
>![Cat at FreeCodeCamp](https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg)

## Anchor

Anchor can be used to link to other page

The `href` is where to put the link to other page. Wrapped by anchor tag is the text alternative for the link.

The `target="_blank"` to open link in new browser tab.

```html
<a href="https://freecatphotoapp.com">cat photos</a>
```

The tag can be nested in other tag

```html
<p>
    Click here to see 
    <a href="https://freecatphotoapp.com">cat photos</a>
</p>
<!-- or  -->
<a href="https://site.com/link-when-click-image">
    <img src="https://site.com/the-image.png">
</a>
```

## Section

Each section should be in a `section` tag.

```html
<section></section>
```

## List

Listing in HTML

### Unordered List

```html
<ul>
    <li>item</li>
    <li>item</li>
    <li>item</li>
</ul>
```

### Ordered List

```html
<ol>
    <li>item</li>
    <li>item</li>
    <li>item</li>
</ol>
```

## Figure

The `figure` element represents self-contained content and will allow you to associate an image with a caption.

The `figcaption` is the caption for the figure.

```html
<figure>
    <img >
    <figcaption>Caption for the image</figcaption>
</figure>
```

## Emphasis

To emphasis a text, use tag `em`

```html
<em>The emphasised text</em>
```

## Strong

The strong element is used to indicate that some text is of strong importance or urgent.

```html
<strong>The importance text</strong>
```

## Form

To create a form, use `form` tag.

The `action` attribute indicates where form data should be sent

### Input

The `input` element allows you several ways to collect data from a web form

The `type` attribute with the value `text` to the `input` element.

The `type=radio` is only one answer allowed to select
The `type=checkbox` is multiple answer allowed to select

The `name` attribute is the name of `input`

The `placeholder` attribute if the text placeholder of `input`

The `required` attribute is to make user to fill in the `input`

### Button

Use the `button` element to create a clickable button.

### Id

The `id` attribute is used to identify specific HTML elements. Each `id` attribute's value must be unique from all other id values for the entire page.

### Fieldset

The `fieldset` element wrap the set of field in a form

The legend element acts as a caption for the content in the fieldset element. It gives users context about what they should enter into that part of the form.

```html
<form action="/submit-url">
    <fieldset>
        <legend>Is your cat an indoor or outdoor cat?</legend>
        <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
        <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
    </fieldset>
    <input type="text" name="input-name" placeholder="text placeholder" required />
    <button type="submit">Submit</button>
</form>
```

## Footer

The `footer` element is to define the footer area in the document.

```html
<footer></footer>
```

## The result

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <title>CatPhotoApp </title>
</head>

<body>
    <h1>CatPhotoApp</h1>
    <main>
        <section>
            <h2>Cat Photos</h2>
            <!-- TODO: Add link to cat photos -->
            <p>
                Click here to view more
                <a href="https://freecatphotoapp.com">cat photos</a>
            </p>
            <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg"
                atl="A cute orange cat lying on its back" />
        </section>
        <section>
            <h2>Cat Lists</h2>
            <h3>Things cats love:</h3>
            <ul>
                <li>cat nip</li>
                <li>laser pointers</li>
                <li>lasagna</li>
            </ul>
            <figure>
                <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg"
                    alt="A slice of lasagna on a plate." />
                <figcaption>Cats <em>love</em> lasagna.</figcaption>
            </figure>
            <h3>Top 3 things cats hate:</h3>
            <ol>
                <li>flea treatment</li>
                <li>thunder</li>
                <li>other cats</li>
            </ol>
            <figure>
                <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg"
                    alt="Five cats looking around a field." />
                <figcaption>
                    Cats <strong>hate</strong> other cats.
                </figcaption>
            </figure>
        </section>
        <section>
            <h2>Cat Form</h2>
            <form action="https://freecatphotoapp.com/submit-cat-photo">
                <fieldset>
                    <legend>Is your cat an indoor or outdoor cat?</legend>
                    <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked />
                        Indoor</label>
                    <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor" />
                        Outdoor</label>
                </fieldset>
                <fieldset>
                    <legend>What's your cat's personality?</legend>
                    <input id="loving" type="checkbox" name="personality" value="loving" checked />
                    <label for="loving">Loving</label>
                    <input id="lazy" type="checkbox" name="personality" value="lazy" />
                    <label for="lazy">Lazy</label>
                    <input id="energetic" type="checkbox" name="personality" value="energetic" />
                    <label for="energetic"> Energetic</label>
                </fieldset>
                <input type="text" name="catphotourl" placeholder="cat photo URL" required />
                <button type="submit">Submit</button>
            </form>
        </section>
    </main>
    <footer>
        <p>
            No Copyright -
            <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
        </p>
    </footer>
</body>

</html>
```

## Preview the result

CatPhotoApp

CatPhotoApp
===========

Cat Photos
----------

Click here to view more [cat photos](https://freecatphotoapp.com)

![A cute orange cat lying on its back](https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg)

Cat Lists
---------

### Things cats love

* cat nip
* laser pointers
* lasagna

![A slice of lasagna on a plate.](https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg)

Cats _love_ lasagna.

### Top 3 things cats hate

1. flea treatment
2. thunder
3. other cats

![Five cats looking around a field.](https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg)

Cats **hate** other cats.

Cat Form
--------

Is your cat an indoor or outdoor cat?  Indoor  Outdoor

What's your cat's personality?  Loving  Lazy  Energetic

 Submit

No Copyright - [freeCodeCamp.org](https://www.freecodecamp.org)
