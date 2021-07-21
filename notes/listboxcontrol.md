# HTML Lists, CSS Box Model, & Accessing Array Values

### Lists

There are three types of lists one can make:

- *Unordered* - items in these lists use bullet points
- *Ordered* - items in these lists are numbered
- *Definition* - items in these lists are displayed as if they are entries in a dictionary

#### General list structure

I'll use an unordered list to demonstrate how lists are typically structured.

```JavaScript
<ul>
  <li>1 tbs Olive Oil</li>
  <li>1 lbs Chicken Breasts</li>
  <li>1 lbs Chicken Andouille Sausage</li>
  <li>3 cups Heavy Cream</li>
  <li>4 cups Chicken Broth</li>
  <li>4 tbs Butter</li>
</ul>

```
In this instance, I created a list by writing opening & closing `ul` tags. For ordered lists it'd be `ol` and for definition lists `dl`. Inside said tags are `li` elements. These are essentially list entries. You use these elements to show the items in your list. It's `li` for both ordered & unordered lists. It's a little different for definition lists since you need to list the term along with its definition. Here's an example of a definition list:

```JavaScript
<dl>
  <dt>Asynchronous</dt>
  <dd>not simultaneous or concurrent in time.</dd> 
  <dt>Promise</dt>
  <dd>A declaration assuring the one will or will not do something; a vow.</dd> 
</dl>

```
In these types of lists, there's a term (represented by `dt`) accompanied by a definition (`dd`).

### CSS Box Model

![Box Model](../assets/box-model.png) 

The illustration above demonstrates what the box model is. You should probably look at every element as if it was a box. The four main components of the box model are:

- Content *(the actual content of the element)*
- Padding *(whitespace around the content, but still within the border)*
- Border *(border box that wraps around the padding & content)*
- Margin *(wraps around the content, padding, and border as whitespace between this box and other elements)*

### Accessing values in arrays

Since arrays are essentially collections of values, there's often a need to access a singular item in said collections. There's a pretty easy way to do that. Say we make an array:
`let cereals = ['fruit loops', 'cocoa puffs', 'trix', 'vanilla chex'];`

If we wanted to store the value `'cocoa puffs'` into a variable named 'chocolate', we'd do it like this:

`let chocolate = cereals[1];`

Values that are stored inside arrays are indexed. These values can be accessed by referencing the array with square brackets appended to the end of it. The integer inside of the brackets respresents the index you're attempting to access. Please note that the first item in an array always has an index of zero.
