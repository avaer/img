Convert any dom tree to an image element.

```
const img = require('img');

// create a rendered image of the DOM element with id 'my-element' and attach it to the end of the document
img($('#my-element')[0], function(img) {
  document.body.appendChild(img);
});

// create a rendered <h1> as an image and open the result in a new window
img($('<h1>Please render this heading</h1>')[0], function(img) {
  window.open(img.src, '_blank');
});
```
