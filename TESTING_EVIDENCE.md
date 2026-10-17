# A3 Responsive and Browser Testing Evidence

**Project:** The Red Rose  
**Test date:** 18 October 2026  
**Test environment:** Chromium headless browser; local project HTML/CSS rendered at specified viewport sizes  
**Important limitation:** These screenshots show the project rendered in a browser using the supplied local HTML/CSS and embedded copies of the project's local JPEGs. The live GitHub Pages URL and a second browser were not independently tested in this run. Complete those checks before final submission.

## Responsive viewport checks

| Device category | Viewport | Result | Evidence |
|---|---:|---|---|
| Mobile | 390 × 844 | Pass for local viewport layout | `evidence/mobile.png` |
| Tablet | 768 × 1024 | Pass for local viewport layout | `evidence/tablet.png` |
| Desktop | 1440 × 900 | Pass for local viewport layout | `evidence/desktop.png` |

Automated checks observed at each viewport:
- The document width matched the viewport width (no horizontal overflow).
- All three image elements loaded successfully in the rendered page.
- All navigation anchor targets existed.
- Five main content sections were present.
- No browser page errors were observed during these checks.

## Browser test record

| Browser and version | Device/viewport | Result | Notes |
|---|---|---|---|
| Chromium (headless) | Mobile 390 × 844 | Pass | Local rendered page; screenshot saved |
| Chromium (headless) | Tablet 768 × 1024 | Pass | Local rendered page; screenshot saved |
| Chromium (headless) | Desktop 1440 × 900 | Pass | Local rendered page; screenshot saved |
| Microsoft Edge / Firefox | Not tested | Not tested | Test in another installed browser if available |
| Published GitHub Pages URL | Not tested in this run | Not tested | Open the live website and verify images, navigation and layout after deployment |

## Functional and usability checks

| Test | Expected result | Result | Notes |
|---|---|---|---|
| Page rendering | Website title and content render | Pass | Title: The Red Rose | Beauty & Meaning |
| Navigation targets | Home, About, Meaning, Gallery, Care Tips targets exist | Pass | Verified target elements in rendered DOM |
| Images | Three image elements load | Pass | Each image has non-empty alternative text |
| Horizontal overflow | Document width does not exceed viewport | Pass | Width matched viewport at all three sizes |
| JavaScript/page errors | No page errors in console | Pass | No page errors observed; website does not require JavaScript |
| Live deployment | Live page loads from GitHub Pages | Not tested | Must be checked after uploading updates |
| Other browser compatibility | Works in a second browser | Not tested | Record the browser and actual result after testing |

## HTML validation

1. Open https://validator.w3.org/nu/
2. Upload `index.html` or enter the published page URL after updating GitHub Pages.
3. Fix errors where possible and re-run validation.
4. Save a genuine screenshot of the final validation result in this folder as `html-validation.png`.

**Validation status:** Not yet run in this environment.  
**Evidence filename:** Add `evidence/html-validation.png` after validation.

## Final checks still required before submission
- [ ] Open the published GitHub Pages URL after uploading the updated files.
- [ ] Check all images and navigation on the live site.
- [ ] Test in another browser if available (for example Microsoft Edge or Firefox).
- [ ] Run the W3C Nu HTML Checker and save its actual result.
- [ ] Keep these local responsive screenshots and add any additional live-site screenshots if requested by the lecturer.
