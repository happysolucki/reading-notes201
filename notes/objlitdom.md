# JS Object Literals & the DOM

### Objects

An object is a standalone entity, with properties and type. Objects in JavaScript
are comparable to objects in real-life. A phone is an object. It has properties
like height, color, weight, cpu, battery, etc. JavaScript objects can have properties
in the same way. It also should be noted that functions that are properties of
objects are known as **methods**.

#### Object Literals

Generally, objects are created using literal notation.

```JavaScript
const restaurant = {
    name: "Fannie's",
    tables: 25,
    occupied: 22,
    openTables: function() {
        return this.tables - this.occupied;
    }
}
```

The keyword `this` in `openTables` indicates that _this_ object's `tables` &
`occupied` properties are being used.

#### Accessing an Object's Properties

Dot notation is usually the go-to way to access properties & methods on objects.
Here's an example:

```JavaScript
let restaurantName = restaurant.name;
let availableTables = restaurant.openTables();
```

One can also use square brackets to access properties like so:

```JavaScript
let maxTables = restaurant['tables'];
let availableTables = restaurant.['openTables']();
```

### DOM

The Document Object Model (DOM) specifies how browsers should create a model of an
HTML page and how JavaScript can access and update the contents of a web page while
it is in the browser window.

#### Accessing the DOM

There are several ways to access the DOM. The most recent and flexible way is using
`querySelector()` and `querySelectorAll()`. Say there's an element in the DOM that
has a class of `item`. Here's how to access it using `querySelector()`:

```JavaScript
let item = document.querySelector('.item');
```

Say there were multiple objects with this class. To access all of them, use `querySelectorAll()`:

```JavaScript
let items = document.querySelectorAll('.item');
```

Using the above function stores all elements with the class of `item` into an array.
So, referencing the third element in array would be done using `items[2]`. It should
be noted that elements captured by `querySelectorAll()` are ordered based their position
in the DOM tree.
