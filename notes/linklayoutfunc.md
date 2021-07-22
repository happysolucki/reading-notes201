# HTML Links, CSS Layout, & JS Functions

### Links

List are an integral part of the web browsing experience. Almost every page you come across has a link of some sort on it. Typically, links will serve one of the following purposes:

- Link from one website to another
- Link from one page to another on the same website
- Link from one part of the webpage to another part of the same page
- Open link in a new window
- Link to email program with an already filled address to email someone

You want to use the `<a>` element to link to stuff. For reference, `<a>` stands for anchor. Here's how you'd link to another site:
```HTML
// linking to another website
<a href="https://en.wikipedia.org/wiki/Invincible_(TV_series)">Invincible wiki</a>

// linking to a local page for the same site
<a href="pages/about.html">About</a>

```

The `href` attribute is the url that the hyperlink points to. The text within the `<a>` tags is what'll show as the hyperlink.

### CSS Layout

Outside of thinking of elements more so as boxes, there are some other general topics you should know of in regards to layout.

#### Block vs Inline

Elements in a HTML file are either block-level boxes or inline boxes. Block basically means that the element starts on a new line. Elements such as `h1`, `p`, `div`, & `ul` inherit this property by default. Other elements like `img`, `b`, & `i` are inline by default. They basically flow in between surrounding text.

#### Page Flow / Positioning
There are ways to manipulate the normal way in which elements flow on a webpage. The CSS property `position` can do this. The most common values for `position` are relative, absolute, and fixed. Relative allows you to move an element from where it would normally flow in the document. On the other hand, *absolute* removes the element from the normal flow and positions the element in relation to it's parent container. *Fixed* is a flavor of absolute positioning, but in this case the element is positioned in relation to the browser window. Basically, the element will stay in the same place regardless of how much you scroll up or down the page.

### Functions, Methods, and Objects

Objects might seem unfamiliar, but in reality we've already been working with objects. Strings, arrays, & numbers are all examples of objects. We've already used methods as well. Methods are functions, but they were created as a part of an object. Here's a visual:
```JavaScript
// function
getAge();

// .toLowerCase is a method available the String object
let name = 'Kyrie';
return name.toLowerCase();

```

### Pair Programming

Pair programming can be extremely helpful in improving your communication, receiving of feedback, and simply writing code. It's more efficient that working alone because you essentially have a human linter checking your code and catching any mistakes you make. It also gives you the oppertunity to learn how others look at & solve problems. The social element of this is valuable too. Having to explain the design choices you made while pair programming will prepare you for coding interviews.
