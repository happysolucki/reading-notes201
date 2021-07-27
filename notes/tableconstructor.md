# HTML Tables & JS Contstructor Functions

### Table Basics

Tables are used to display information in a grid format. Tables are created through
the use of the `<table>` element. Inside this element typically lies some `<tr>`
elements, which indicate the start of each table row. The `<tr>` elements usually
contain `<td>` elements represent table cells. Here's an solid example of creating
a table:

```js
<table>
    <tr>
        <td>7</td>
        <td>14</td>
        <td>21</td>
    </tr>
    <tr>
        <td>8</td>
        <td>16</td>
        <td>24</td>
    </tr>
    <tr>
        <td>9</td>
        <td>18</td>
        <td>27</td>
    </tr>
<table>
```

Table headings can also be added using the `<th>` element. These sort of function
like `<td>` elements, so they should be placed within `<tr>` elements.

### Contstructor Functions

There's an alternative way to create objects that's more suited towards making several
instances of similar objects. It's know as constructor notation. This method relies
on using a function to create new objects. Here's an example:

```js
function Shop(name, avgCustomers, purchasesPerCustomer) {
  this.name = name;
  this.avgCustomers = avgCustomers;
  this.purchasesPerCustomer = purchasesPerCustomer;
  this.purchasesPerDay = function () {
    return this.avgCustomers * this.purchasesPerCustomer;
  };
}
```

Making objects this way allows one to easily create instances of said object, like so:

```js
const cookieShop = new Shop("Salmon Cookies", 45, 5);
const doughnutShop = new Shop("Gibson's", 85, 8);

// log name of doughnut shop
console.log(doughnutShop.name);
```
