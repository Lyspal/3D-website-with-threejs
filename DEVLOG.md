# 3D-website-with-threejs Dev Log

## 2022-05-19

Getting started with [Build a Mindblowing 3D Portfolio Website // Three.js Beginner’s Tutorial](https://youtu.be/Q7AOvWpIVHU) by Fireship.

This tutorial includes the use of these new tools:

- Vite
- Three.js

---

`requestAnimationFrame(animate);`

---

Got a problem with `document.body.getBoundingClientRect().top` in camera motion
while scrolling: the camera is jumping after a little scroll.

Found that `t` value was positive and negative due to a default margin applied to the body element. This may be the problem.

However, after completing the script, I tested with the provided CSS: with no
edit of the `body`'s margin, the camera was not jumping.

I then tried to remove my own fix, and everything was fine.

Not sure why.

---

Still kept the `body`'s margin fix because margins caused horizontal
scrolling.

---

Little tweaking of the moon position.

Corrected layout problem when waiting for script to load:

- Moved the CSS import to the HTML file.
- Added a colored backgroud to the page which is seen during loading.

Made a quick fix to the loading of the canvas by adding an opacity transition.
