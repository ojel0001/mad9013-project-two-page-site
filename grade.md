# Grade
HTML Code Quality: 3.5/5
CSS Code Quality: 4.25/5
Responsive Design: 4.25/5
Assignment Requirements: 4.25/5

Total: 16.25/20

## Comments

### HTML
Search for `prof comment` in individual files for specific comments.

- There is no need to separate the blog content into a bunch of `<div class="container article-intro-container">` elements. You could wrap all of it in a single one. Requires less elements and doesn't change the meaning of the content because `div` doesn't apply meaning to content.

### CSS
Search for `prof comment` in individual files for specific comments.

- The blog content is an example of where its better to use descendent selectors over classes. You put a class on every single heading and `p` tag, which was a lot of work. Instead you could have applied those styles without needing the classes with a selector like `.article p`. This is both simpler, and safer, because it protects you if you forget to add a class somewhere.
- When you are using `clamp()` you are setting different minimum and maximum values, but the preferred value is always the same at `7.5cqi`. This value should also vary based on the desired scale of the text size.
  - Also, it often is too large of a value, meaning the maximum value is hit at a very small screen size, defeating the purpose of even using `clamp()`

### Responsive Design
- There is some inconsistency in the width and alignment of different section content. Ideally all sections should have the same width of container, and the same padding on the left and right, applied through the `.container`, to ensure everything lines up perfectly.
- The blog body text is too large. Stick with the browser default text size for large blocks of content.
- The blog content is too wide. The width of the text blocks are too wide (too large of line-length), which causes poor readability. A narrower text container should be used.

### Assignment Requirements
- A new Google font was not used.
- CSS Variables should be used for applying colours.
- You have not fully removed the original colour scheme from the deliverables