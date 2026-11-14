# Nandakishore Ravi | Engineering Portfolio

A portfolio of my work in laboratory automation, materials science, electrochemical engineering, and experimental instrumentation.

**[View the portfolio](https://nkishoreofficecode.github.io/Portfolio/)** · **[LinkedIn](https://www.linkedin.com/in/nandakishore-ravi/)** · **[Email](mailto:nkishoreoffice@gmail.com)**

## About

I am a Ph.D. candidate at the University of Houston, advised by Dr. Xiaonan Shan, with expected completion in 2027. My work combines hardware integration, experimental design, process development, and data analysis.

## Featured work

- **Laboratory automation:** Co-development of an autonomous catalyst synthesis and screening platform integrating robotics, liquid handling, and electrochemical measurements.
- **Nanodiamond quantum sensing:** Integration of optical, microwave, and measurement instruments for NV-center sensing and optically detected magnetic resonance (ODMR).
- **AEM electrolyzers:** Electrolyzer prototyping, catalyst development, and performance evaluation.
- **Raman spectroscopy:** Time-resolved in-situ experiments correlated with electrochemical measurements.
- **Thin-film processing:** Metal deposition, thermal processing, and adhesion development on ITO substrates.
- **FTIR gas analysis:** Laboratory instrumentation and gas-sampling setups.
- **Presentations and exhibitions:** Technical talks, poster presentations, and live hardware demonstrations.

The site includes captioned photo galleries, expandable photo collections, and an embedded automation demonstration video.

## Repository files

| File or folder | Purpose |
| --- | --- |
| `index.html` | Page content, project descriptions, galleries, and video embeds |
| `styles.css` | Responsive layout, typography, colors, and gallery styling |
| `images/` | Optimized project photos and thumbnails, grouped by project |
| `NANDU1.jpg` | Profile photograph |
| `gallery-data.json` | Photo paths, dimensions, and captions for reference |
| `.github/workflows/static.yml` | GitHub Actions workflow for GitHub Pages deployment |
| `README.md` | Project overview and maintenance instructions |

This is a static HTML and CSS website. No package installation or build command is required. Styles and photos are stored locally; the embedded YouTube video requires an internet connection.

## Preview locally

1. Download the repository and extract the ZIP, or clone it.
2. Open `index.html` in a browser.
3. Keep `styles.css`, `NANDU1.jpg`, and the `images/` folder alongside `index.html` so the relative paths resolve.

After editing a file, save it and refresh the browser. YouTube embedding may behave differently when opened directly from a local file; use the accompanying YouTube link if playback is unavailable.

## Update photos and captions

The photo folders are `automation`, `electrolyzer`, `ftir`, `h2-expo`, `presentations`, `quantum-sensing`, `raman`, and `thin-films`.

1. Add a browser-compatible image, such as JPEG, to the appropriate folder in `images/`. Convert HEIC files before using them on the website.
2. Use descriptive lowercase filenames with hyphens. Match filename capitalization exactly in HTML paths.
3. Prepare a larger image and a smaller thumbnail. The current gallery uses images up to 1600 pixels on the longest edge and thumbnails up to 640 pixels.
4. In the relevant gallery in `index.html`, copy an existing `<figure>` and update its image link, thumbnail path, dimensions, alternative text, and caption.
5. Update the corresponding entry in `gallery-data.json` for consistency. If adding photos to an expandable collection, also update the photo count in its `<summary>`.
6. Preview the gallery and check that the larger image opens correctly.

**The page does not load `gallery-data.json` dynamically.** Editing that file alone will not change the website; gallery markup and captions must also be updated in `index.html`.

Use captions that describe what is shown and distinguish individual contributions from collaborative work. Include only photos and research information cleared for public sharing.

## Add YouTube videos

Upload the video to YouTube, then add an embed to the relevant project section in `index.html`. Replace `VIDEO_ID` and the descriptive title below:

```html
<iframe
  src="https://www.youtube.com/embed/VIDEO_ID"
  title="Descriptive title of the project demonstration"
  loading="lazy"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
</iframe>
<p>
  <a href="https://www.youtube.com/watch?v=VIDEO_ID">
    Watch the demonstration on YouTube
  </a>
</p>
```

Use the `/embed/VIDEO_ID` URL for the iframe, rather than a normal YouTube watch-page URL. Include a direct video link as a playback fallback.

## Publish updates

The included workflow deploys the repository to GitHub Pages on pushes to `main`. It also supports a manual run through GitHub Actions.

To upload through GitHub:

1. Open the repository and choose **Add file → Upload files**.
2. Upload the updated files and folders directly into the repository root. Do not nest them inside an extra `Portfolio-main` folder.
3. Keep `.github/workflows/static.yml` and all unchanged assets.
4. Commit the changes to `main`.
5. Check the deployment result in the repository's **Actions** tab, then refresh the live portfolio.

When publishing the photo update, include `index.html`, `styles.css`, the complete optimized `images/` folder, `gallery-data.json`, and this `README.md`. Keep `NANDU1.jpg` at the root. There is no need to delete the repository before uploading replacements.

## Before publishing

- Check image paths and navigation links.
- Review captions, dates, project contributions, and publication status.
- Check the layout on a phone and a desktop browser.
- Test the email, LinkedIn, and video links.
- Confirm that the uploaded photos are appropriate for public release.
