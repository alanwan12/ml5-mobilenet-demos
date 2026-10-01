# ml5 MobileNet Demos

Three small browser demos that use [ml5.js](https://ml5js.org/) and [p5.js](https://p5js.org/) to classify images with the pre-trained MobileNet model.

| Folder | What it does |
| --- | --- |
| `ml-tutorial/` | Page titled "Getting Started with ml5.js". Loads MobileNet, classifies `robin.png`, and prints the results to the browser console. The canvas only shows a colored background. |
| `ml-test/` | Loads an image named `me.jpg`, runs MobileNet on it, draws the image on a canvas, and shows the top label and its confidence under it. |
| `ml-webcam/` | Runs MobileNet continuously on your webcam feed and draws the current top label at the bottom of a 640x550 canvas. |

## Run it
- `ml-tutorial` and `ml-test` load an image file, so serve the folder over HTTP instead of opening the file directly (for example `python3 -m http.server` and visit `http://localhost:8000/`).
- `ml-webcam` needs camera access, which requires `localhost` or HTTPS.

## Notes
- `ml-test/` expects a file called `me.jpg`, which is **not included**. Put any JPG image there with that name.
- The libraries are loaded from CDNs with specific versions (ml5 0.4.3 / 0.6.0, p5 0.9.0 / 1.2.0) and were written for that older ml5 API. Newer ml5 releases changed their API.
