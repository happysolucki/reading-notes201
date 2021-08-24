# CSS Transforms, Transitions, and Animations

The `transform` property allows you to rotate, scale, skew, or translate an element. Say you have a `div` with a class named `shrink`, and you want to shrink the div when it is hovered over. You can achieve this with transform's scale function:

```css

.shrink:hover {
  transform: scale(0.95);
}

```

Problem solved! Though, just leaving it like this results in the hover effect being somewhat jarring. **Transitions** can be used to remedy this. Transitions typically have three properties that you need to account for:

1. What property/properties should be transitioned
2. The duration of the transition
3. The type of transition

You can also add a delay to the transition if you want aswell.
Here's how you'd make the hover effect transition for half a second that eases in and out:

```css

.shrink {
  transition: transform 0.5s ease-in-out
}

```

If you desire more control over these types of things, **animations** are here for the rescue. Making animations is a two-step process. First comes actually making the animation using *keyframes*. Here's an example of what that would look like: 

```css
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```

To use this transition on a element, like the `div` earlier, you'd do something like this:

```css
.shrink:hover {
  animation-name: slide;
  animation-duration: 3s;
  animation-timing-function: ease-in-out;
}

```

###### Sources
[MDN | Transform](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)
[CSS Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)
