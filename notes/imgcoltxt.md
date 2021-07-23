# Images, Color, and Text

### Images

Images are a common occurance on the web. Typically images are deployed with the `<img>` element. It is possible to show images without using `<img>` elements. It can be done with the `background-image` CSS rule. Here are examples of how to do both:

```html
<img src="https://guardian.ng/wp-content/uploads/2018/12/orange-juice.jpg" alt="A jar of orange juice with multiple oranges stacked behind it">

```

```css
// make div bg show image
div {
    width: 500px;
    height: 500px;
    background-image: url(assets/orange.jpg);
    background-size: contain;
    background-position: center;
  }

```

### Color

Before learning how to use color in CSS files, it's imperative to understand how color is transmitted digitally. Colors on digital screens are based around RGB (acronym for Red Green Blue). Every color displayed digitally is a mixture of differing amounts of red, green, and blue. It's like this because computer monitors are composed of pixels. When the screen isn't on, it's black since it's not emitting any light. When it's on, each individual pixel can be a different color, thus creating a picture.

There are several ways to reference a color in CSS:

- **Names:** *red, yellow, blue, lightgray*
- **RGB/RGBA:** *rgb(220, 100, 65), rgba(23, 100, 210, 0.45)*
- **Hex:** *#3a581d*
- **HSL/HSLA:** *hsl(202, 50%, 50%), hsla(90, 100%, 80%, 0.95)*

The 'A' in RGBA & HSLA stands for alpha, which is another term for opacity.

### Text

There several things to account for in regards to text such as weight, style, size, letter spacing, color, etc. Luckily, there are CSS properties for most of these things. Here's an example of what it would look like to modify the text of a paragraph element:
```css
p {
    font-weight: bold;
    font-style: italic;
    font-size: 1.25rem;
    letter-spacing: 3px;
    color: #fff;
  }

```


