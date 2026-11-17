# Haechan Park — Academic Website

Personal research website built with HTML, CSS, and JavaScript. Ready for GitHub Pages.

**Theme:** RGB(61, 80, 130) (`#3D5082`)  
**Pages:** Home (research carousel), Haechan Park, Research Interests, Publications, Gallery.

### Publish on GitHub Pages

Follow the Korean step-by-step guide in [GITHUB_PAGES_GUIDE_KO.md](GITHUB_PAGES_GUIDE_KO.md).

In short, upload all files and the `assets/` folder to the root of a public GitHub repository, then open **Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save**. Changes committed to `main` redeploy automatically.

### Editing locations

| Want to change | File |
| --- | --- |
| Home carousel headings, images and descriptions | `index.html` |
| Personal biography and contact | `haechan-park.html` |
| Research descriptions and figures | `research-interests.html` |
| Publication data | `assets/site.js` (`const publications`) |
| Gallery figures and titles | `gallery.html` |
| Theme color, typography and layout | `assets/site.css` (`--accent: #3d5082`) |
| Carousel, menu and gallery interactions | `assets/site.js` |
| Image illustrations / images | `assets/` |

All navigation links and assets are **relative**, so they work on both username-root and project GitHub Pages URLs. Image artwork is conceptual; replace with actual research figures before public release. Please verify biographical, bibliographic and external link details before publishing.

No build command, npm installation, or server is required for deployment.
