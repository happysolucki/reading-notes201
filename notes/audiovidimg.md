# Audio, Video, and Images

### Controlling Images using CSS

Even though it's possible to modify aspects of images within the HTML markup, it's preferable to control the properties of images using CSS. Controlling the dimensions of images is pretty straightforward. Outside of that, here are some CSS rules that I use often:

- `background-image`: set image as background`
- `background-repeat`: set behavior of image in regards to repeating itself
- `background-position`: specify where the background image is placed in the browser window (only works if image isn't being repeated)
- `background-size`: set size of background image

There's even a shorthand rule for this. The `background` rule accounts for these properties:

1. `background-color`
2. `background-image`
3. `background-repeat`
4. `background-attachment`
5. `background-position`

### Audio and Video

Audio and video can be implemented in a website using `<audio>` and `<video>` tags respectively. Before add a video to a webpage, factors such as format, players and plugins, and general approach should be considered. The easiest way to add a video to a site is to upload the video to a hosted video service such as YouTube, Vimeo, Imgur, etc and use the features provided on their site to embed the video on the webpage.
