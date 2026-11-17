# Haechan Park — Publications update (Nov 18, 2026)

## What changed
- `publications.html`: 11 verified journal publications (2022–2026) featuring Haechan Park.
- Complete author lists: no `et al.`; bold Haechan Park, † equal contribution, * corresponding authors.
- Three publication filters and live item counts retained.
- `index.html`: home still only shows the 2-paper carousel, but the Publications CTA mentions the complete list.
- Other pages remain unchanged.

## Upload to GitHub Pages
Extract this zip, open your existing GitHub repository, and use Add file > Upload files to upload and replace the five HTML files in the repository ROOT (not a nested folder). Commit the change. If you prefer, only `index.html` and `publications.html` need replacing. Wait until Actions > pages build and deployment succeeds; hard-refresh the browser.

## Sources and notes
Google Scholar profile (user=w9Lw_o8AAAAJ) was inaccessible to automated retrieval during update. Author names and corresponding-author marks were cross-checked against the official SIMS Lab publications page (https://sites.google.com/view/sims-lab/publications), publisher pages (Nature, RSC, ACS, AAAS, Elsevier), and public indexing for the newly published Nov 2026 ACS Applied Polymer Materials article. The 2026 ACS Applied Polymer Materials paper is included based on the publisher record even if Google Scholar has not indexed it yet. The site does not fetch Google Scholar dynamically.

To edit future publications: edit the `const publications` JavaScript array near the bottom of `publications.html`. Use a comma-separated full author list; append * to corresponding authors and † to equally contributing first authors. The page will format markers automatically.
