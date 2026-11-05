# Bhavyansh Rathore — Portfolio

This is a lightweight static site. It runs locally with Python and deploys directly to Vercel with no build step.

## Run locally

From this folder, run:

```sh
python3 -m http.server 4173
```

Then open <http://localhost:4173>.

## Video showcase

The first three showcase cards contain the supplied videos in `media/`. The video frames use a 16:9 layout while preserving each original video’s portrait framing. Two illustrated project slots remain available.

To replace or add a video, put an MP4 in `media/` and update a project card in `index.html`:

```html
<video class="project-video" controls playsinline preload="metadata">
  <source src="media/project-04.mp4" type="video/mp4">
</video>
```

Update the project title, description and duration beside it. Keep the `project-video` class to retain the 16:9 frame.

## Deploy to Vercel

Import this folder as a Vercel project. Choose **Other** as the framework preset and leave the build command and output directory empty. Vercel serves `index.html` as a static site. `vercel.json` enables clean URLs.

