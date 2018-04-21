# Restaurant Reviews: Stage 1
## Responsive Design
- ~~Is the site UI compatible with a range of display sizes?~~
  - ~~All content is responsive and displays on a range of display sizes.~~
  - ~~Content should make use of available screen real estate and should display correctly at all screen sizes.~~
  - ~~An image's associated title and text renders next to the image in all viewport sizes.~~
- ~~Are images responsive?~~
  - ~~Images in the site are sized appropriate to the viewport and do not crowd or overlap other elements in the browser, regardless of viewport size.~~
    - ~~on the index.html (using 128px wide images with similar render on different layouts)~~
    - ~~on the restaurant.html~~
      - ~~360px wide (smartphone + small desktop)~~
      - ~~480px wide (tablet+ medium desktop)~~
      - ~~800px wide (large desktop)~~
  - ~~Are application elements visible and usable in all viewports?~~
  - ~~On the main page, restaurants and images are displayed in all viewports.~~
  - ~~The detail page includes a map, hours and reviews in all viewports.~~
## Accessibility
- ~~Are images accessible?~~
  - ~~All content-related images include appropriate alternate text that clearly describes the content of the image.~~
- Is focus used appropriately to allow easy navigation of the site?
  - Focus is appropriately managed allowing users to noticeably tab through each of the important elements of the page. 
  - Modal or interstitial windows appropriately lock focus.
  - The focus ring is always present and clearly visible
- Are site elements defined semantically?
  - All non-text contents provide text alternatives
  - Elements on the page use the appropriate semantic elements. For those elements in which a semantic element is not available, appropriate ARIA roles are defined.
  - Headings are used properly.
  - Links have a href and title attributes.
  - Make sure all buttons text are descriptives enough (ex: Learn More or More isn't enough).
  - Semantic elements (header, nav, main, section, article, footer, ...) are used properly
  - The website is readable in high contrast mode
  - Contrast is valid according to WCAG AAA standards ([tool](https://webaim.org/resources/contrastchecker/))
  - Add `role="application"` to the div element with id#map
  - The <ul> that is the breadcrumb needs to have the appropriate aria structure. Follow this example https://www.w3.org/TR/wai-aria-practices/examples/breadcrumb/index.html
## Offline Availability
- Are pages that have been visited available offline?
  - When available in the browser, the site uses a service worker to cache responses to requests for site assets. Visited pages are rendered when there is no network access.