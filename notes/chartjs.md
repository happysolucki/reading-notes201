# Chart.js

Chart.js is a JavaScript library that utilizes HTML5's canvas element to easily illustrate data with pretty charts. Line, bar, pie, and other charts can be used with this plugin, and there's rich documentation that explains how to tailor your chart to your needs.

### Setup

Setup is pretty easy. Of course, you need to link the Chart.js library to your html file in some way. The fastest way is to link the CDN to your page like so:

```html

<script src="https://cdn.jsdelivr.net/npm/chart.js@3.5.0/dist/chart.min.js"></script>


```

I like to put this before the closing body tag. I should note that any other scripts you have in your project should be sourced after this library to ensure everything works properly.

In order to actually use Chart.js there needs to be a `<canvas>` element in the html file. The typical canvas element looks like this: `<canvas id="my-chart" width="400" height="400"></canvas>`

### Usage

First, in your js file you need to capture the DOM canvas element. There is a little extra needed on top of this though. Here's an example:

```js

const canvasEl = document.querySelector('#my-chart').getContext('2d');

```

There are different ways to construct your chart. Here's an example of how I did it in my most recent lab.

```js

const canvasEl = document.querySelector('#my-chart').getContext('2d');

const barData = {
  type: "bar",
  data: {
    labels: ['Monday','Tuesday','Wednesday','Thursday','Friday'],
    datasets: [
      {
        label: "# of votes",
        data: [2,5,13,19.39],
        backgroundColor: "#48a497",
        borderColor: "#48a4d1",
      },
    ],
  },
  options: {
    responsive: false,
    scales: {
      y: [
        {
          ticks: {
            beginAtZero: true,
            stepSize: 1,
          },
        },
      ],
    },
  },
};

const barChart = new Chart(canvasEl, barData)

```

The `barData` variable holds a template for my bar chart. Refer to documentation for info on how to set this up yourself. I created the chart by making the variable `barChart` and assigning it a new chart that takes in `canvasEl` and `barData` as arguments. After you do this you're done. There will be a pretty bar graph shown on the webpage.
