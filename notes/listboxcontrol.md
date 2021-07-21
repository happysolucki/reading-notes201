# HTML Lists, CSS Box Model, & JS Control Flow

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
