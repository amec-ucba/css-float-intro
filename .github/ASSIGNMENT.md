# 📄 Introduction to CSS Float

Use the CSS `float` property to move an image or figure to one side of the page and let text
wrap around it.

## 🎯 Overview

In this coding exercise, you will use CSS to float images and figures to the left or right
while the surrounding text wraps around them. You will also improve the HTML by wrapping an
image and its caption in a `figure` element, and you will learn how to stop content from
wrapping with the `clear` property.

Floats were once used for entire page layouts, but modern web designers use **Flexbox** and
**Grid** for major layout work. Today, floats are mostly used for smaller effects, such as
wrapping text around an image, figure, or pull quote. That's why they are still worth
learning.

> [!IMPORTANT]
> **The companion videos for this exercise are in Canvas**, on the assignment page. They
> walk you through every step, so watch them there instead of working from this file
> alone.

## 🧠 What You Will Learn

By completing this exercise, you will practice how to:

- Use `float: left;` and `float: right;` to wrap text around content
- Explain why a broad selector like `img { float: right; }` is usually a bad idea
- Group an image and its caption with `figure` and `figcaption`
- Compare floating an image with floating a whole figure
- Use class selectors to target one specific figure
- Style a floated figure with `background-color`, `padding`, `width`, and `margin`
- Keep images inside their containers with `max-width: 100%;` and `height: auto;`
- Use `clear: both;` to make a section start below floated content

## 🎬 Watch the Videos in Canvas and Follow Along

The screencast videos are on this assignment's page in **Canvas**, not in this repo. Watch
them **in order** and follow along in Visual Studio Code. Pause whenever you need time to
finish a step — it is normal to pause, rewind, and rewatch parts of a coding demonstration.

Each video builds on the previous one, so please don't skip ahead.

| Video | What you will do |
| --- | --- |
| **Part 1 — Floating Images** | Experiment with `float: right;` and `float: left;` to move images and let text wrap around them. See why using `img` as a broad layout selector affects every image on the page. |
| **Part 2 — Using Figure and Figcaption** | Wrap an image in a `figure` and add a `figcaption`. See why floating the image alone leaves the caption behind, and why floating the whole figure keeps them together. |
| **Part 3 — Styling the Floated Figures** | Add `background-color`, `padding`, `width`, and `margin` so the floated content is easier to see and the text has room to breathe. |
| **Part 4 — Max-Width, Responsive Images, and Clearing Floats** | Learn why images can spill out of their containers and fix it with `max-width: 100%;` and `height: auto;`. Use `clear` so the notes section starts below the floated content. |

> [!IMPORTANT]
> **A few steps in this repo are different from Canvas and the videos.** Follow the videos
> for the HTML and CSS, and follow this repo for getting your files and submitting:
>
> - **Getting the starter files:** create your own repo from this template and clone it
>   in WebStorm, as described in the
>   [Getting Started guide](GETTING_STARTED.md). Don't download a ZIP.
> - **Branch:** do your work on a `develop` branch, not `main`. Before you commit, the
>   branch name at the top left of WebStorm should say `develop`, not `main`.
> - **Submitting:** publish your page to GitHub Pages, open a pull request into `main`,
>   and submit the **pull request URL** in Canvas — not your repository URL — as
>   described in the [Submitting guide](SUBMITTING.md).

> [!IMPORTANT]
> Open the entire project **folder** in VS Code, not a single HTML file. Your HTML needs
> to find the CSS and image files, so keep every starter file together in the root folder.

## 📂 Starter Files

| File | Purpose |
| --- | --- |
| `index.html` | The page content. You will wrap images in `figure` elements, add captions, and add classes here. |
| `styles.css` | Your stylesheet. Write your float rules under the **Float Practice** comment at the top. |
| `reset.css` | Removes browser default styles so every page starts from the same blank slate. Don't edit it. |
| `ivan-cookie.jpg` | Photo of Ivan and Cookie. This becomes your first floated figure. |
| `nap.jpg` | Ivan and Cookie taking a cat nap. Use it to practice floating in the opposite direction. |

`index.html` already links `reset.css` and then `styles.css`, in that order. Keep it that
way so your styles build on top of the reset.

## ✅ Before You Submit

Check the following:

- [ ] `index.html` still links `reset.css` and `styles.css`, and your styles show up in the browser
- [ ] Both images appear in the browser and have useful `alt` text
- [ ] The Ivan and Cookie photo and its caption are grouped in a `figure` with a `figcaption`
- [ ] Each floated element has a class, and your CSS targets that class — not every `img`
- [ ] Floated content goes to the left or right, and the text wraps around it
- [ ] Floated figures have a visible `background-color`, `padding`, and a `width`
- [ ] Floated content has `margin` so the text doesn't touch it
- [ ] The global image rule `img { max-width: 100%; height: auto; }` keeps images inside their figures
- [ ] The `.float-notes` section uses `clear: both;` and starts below the floated content
- [ ] You saved your files
- [ ] The page is live on GitHub Pages and the URL is in your pull request

## 🧮 Grading Rubric

| Criteria | Full credit | Points |
| --- | --- | --- |
| **Figure markup** | The photo and its caption are wrapped in a `figure` with a `figcaption`. Both images have useful `alt` text, and the HTML structure is intact. | 1 |
| **Floating with classes** | Content floats left and right using class selectors. There is no leftover broad `img { float: ... }` rule. Text wraps around the floated content. | 1 |
| **Styling the floated figures** | Floated figures have a `background-color`, `padding`, a `width`, and `margin` that keeps the text from touching them. | 1 |
| **Responsive images and clearing** | `img { max-width: 100%; height: auto; }` keeps images inside their containers. The `.float-notes` section clears the floats and starts below them. | 1 |
| **Publishing and submission** | The page is live on GitHub Pages. The pull request from `develop` into `main` is open, its template is filled in, and its URL is submitted in Canvas. | 1 |
| **Total** |  | **5** |

## 🛠️ Troubleshooting

If something is not working, check these common issues first:

- Did you save the file in VS Code?
- Is your CSS file linked correctly in `index.html`?
- Is the image file name spelled correctly, including `.jpg`?
- Did you float the image when you meant to float the whole figure?
- Does the class name in your HTML match the class selector in your CSS, including the `.`?
- Did you add margin so the text has space around the floated figure?
- Did you add `clear: both;` to the section that should start below the floats?
- Did you commit **and** push your changes in WebStorm?

**Having problems with the videos?**

- **Getting a warning about third-party cookies?** Try using Chrome. Safari's default
  security settings may prevent embedded Canvas videos from playing unless those settings
  are changed.
- **Getting an "Access Denied" error?** Refresh your browser. In many cases, the videos
  will load correctly after the page reloads.

## 📚 Resources

- [MDN — `float`](https://developer.mozilla.org/en-US/docs/Web/CSS/float)
- [MDN — `clear`](https://developer.mozilla.org/en-US/docs/Web/CSS/clear)
- [MDN — `<figure>`: The Figure with Optional Caption element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/figure)
- [MDN — Class selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)
- [MDN — The box model](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Styling_basics/Box_model)
- [W3C CSS Validation Service](https://jigsaw.w3.org/css-validator/#validate_by_input) —
  paste your CSS in to catch typos and missing semicolons

---

The AI policy and submission instructions are in the [README](../README.md).
