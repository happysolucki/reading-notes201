# Relationship between HTML, CSS, & JavaScript

### HTML Text Semantics

Here are some HTML text semantics that I wasn't privy to beforehand:

#### &lt;cite&gt;

You would typically use this when referencing a piece of work like a book, play, film, etc. to indicate where the citation is from. Browsers tend to render this content in italics.

#### &lt;address&gt;

This designates an element that contains the contact details for the author of the page. It can contain a physical address, but it doesn't have to. Browsers tend to render this content in italics.

#### &lt;ins&gt; & &lt;del&gt;

The `<ins>` element can be used to show content that can be inserted into a document. The `<del>` element does the exact opposite; it can show text that has been deleted from it. Typically, the `<ins>` content is rendered with an underline while the `<del>` content is rendered with a strikethrough.

### External CSS & Browser Quirks

There are a multitude of advantages that come with placing your css rules in separate style sheets. First, all of your webpages can share the same style sheet. Instead of having to copy & paste your css rules into every html file, you can just link to it. It's just all-around easier to apply the same css rules to multiple html files if your css is contained in an external style sheet. Using external style sheets also makes maintaining your code more manageable. It elemenates any possible confusion you could have if you used internal css.

Be aware of the fact that there are some inconsistencies between browsers for certain css stuff. One example is css defaults. On every webpage Chrome, Firefox, Edge, and other browsers have default values for certain css rules if they aren't defined by the publisher. Rules such as font-size, padding & margin for certain elements, button styling, etc. are accounted for by default in case they aren't defined by the developer. These defaults can differ across browser. Also, some css rules don't work on every browser. Make sure to research whether the css rule you use works for the most used browsers, and if it doesn't make sure to find a way to account for it.

### Creating Variables & Arrays

Variables are named values that can store any type of JavaScript value. Arrays are somewhat like this, but they're more like containers that can hold several other values.

Creating variables & arrays will typically look like this:
```JavaScript
// variable declaration
let student = 'Karissa';

// array declaration
let subjects = ['Math', 'Biology', 'Health & Wellness', 'Social Studies', 'Digital Arts & Design'];

```

The keyword `let` basically tells JavaScript that you want make a declaration of some sort, which in this case is for a variable & an array. Note that `let` can be substituted for `var` or `const`. The optimal keyword to use will depend on how you actually plan using said variable or array. The word following a declaration keyword is the name of your variable. This is the name that'll be used as a reference to whatever data you assigned to it. You might have also noticed that square brackets where used in the array declaration. Those brackets are required to declare an array. They basically denote that the variable is responible for a collection of values.
