# HTML Comprehension Questions

## Q1 - For each of the following HTML documents, is the HTML valid?

Type true/false in the provided [ ].

a) [false] `<div><span>hello</div></span>`
 `<div><span>hello</span></div>`

b) [false]


```html
<ul>
<li>one</li>
</ol>
```

```html
<ul>
    <li>one</li>
</ul>
```

c) [false] `<ul></ul><img/><ol><li>one</li></ol>`

```html
<ul>
    <img/>
    <ol>
        <li>one</li>
    </ol>
</ul>`
```

## Q2 - What is a screenreader and why should we care about them?

A screen reader is an assistive technology that those with visual impairments or blindness can use to view and browse the web. They can render tex and image content as speech or braille output. It is essential to write web content with accessibility in mind! For example, using `alt` attributes for images, declaring the `lang` tag, and making sure that hyperlink text is describtive [1](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)

Additionally, there are policies and laws implemented to ensure compliance.


## Q3 - For each of the following cases, which tags will be needed?

a) You want to create a webpage with the photos from your latest vacation
html, head, body, ul (ol), li, img, src, alt

```html
<html>
 <head>
 </head>
 <body>
   <ul>
     <li>
       <img src="https://picsum.photos/200" alt="my vacation photo">
       </li>
        <li>
       <img src="https://picsum.photos/300" alt="my vacation photo">
       </li>
    </ul>
 </body>
</html>
```


b) You want to create a website that lists all the art gallery websites in your city and links to their website.

html, head, body, ul (ol), li, a
```html
<html>
 <head>
 </head>
 <body>
   <ul>
     <li>
       <a href="https://fake_somegallery.com">Some gallery! </a>
       </li>
            <li>
       <a href="https://fake_othergallery.com">Some gallery! </a>
       </li>

    </ul>
 </body>
</html>
```

c) You want to sell designer hats. You need to receive orders from the user.
html, head, body, img, ul (ol), lit, a, button, label, input
<html>
 <head>
 </head>
 <body>
   <ul>
     <li>
         <input type="checkbox" id="beret">
  <label for="beret"> beret</label><br>
       <img src="https://upload.wikimedia.org/wikipedia/commons/7/71/Sven_Palmqvist_1965.jpg" alt="beret hat" width="200px"
       </li>
            <li>
         <input type="checkbox" id="beret">
  <label for="beret"> beret</label><br>
       <img src="https://upload.wikimedia.org/wikipedia/commons/8/8b/StetsonHatFortHoodArmy.jpg" alt="beret hat" width="200px"
       </li>
       <button>Order</button>
 </body>
</html>


## Q4 - Can a `button` be a child of a `button`? Explain your reasoning
No, buttons are not block elements, they are inline, so should not have child elements. Also likely doesn't make sense from a UI point of view, as it is clickable.

## Q5 - What is the most generic tag you can use?
div

## Q6 - What do the following achronyms stand for?

a) `a` anchor

b) `ol` ordered list

c) `ul` unordered list

d) `li` list item

e) `tr` table row

f) `th` table header cell

g) `td` standard table cell

## Q7 - Usually, `td` elements are children of what kind of elements?
<tr>

## Q8 - What is the difference between td and th?
<th>` used for header cells while <td> used for data cells. <th> elements will be bold and centered by default, while <td> elements are regular and left-aligned by default.

## Q9 - Which tag makes the text appear bigger: h1 or h3?
By default <h1>, but could differ based on styling.

## Q10 - In which situation can you use self closing tags?
When there is nothing to render between an opening and a closing tag, for example <img>, <hr>.

## Q11 - What is autofilling and why is it important?
`Autocomplete` attibute adds automatic population of certain input fields. It is important because it makes things easier for the end user.

## Q12 - Which attributes are always present in an img element?
`src`, but you should always use `alt`

## Q13 - Which attribute is always present for an anchor tag?
`href`