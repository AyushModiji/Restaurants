# Research notes and implementation references

Research was limited to publicly indexed repository documentation and official standards pages; this was not an exhaustive review of all online tutorials or every source file in either repository.

- [uiuxlabz/restaurant-html-template](https://github.com/uiuxlabz/restaurant-html-template) — repository documentation describes a framework-free restaurant site, custom design tokens, responsive layouts, and reduced-motion support. Used as general inspiration for editorial hospitality structure; its code/assets were not copied into this project.
- [heyitzamjad/foodverse-premium](https://github.com/heyitzamjad/foodverse-premium) — repository documentation describes a vanilla HTML/CSS/JS responsive restaurant landing page, menu grid and navigation patterns. Used as a high-level reference only.
- [MDN: `color-scheme`](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/Properties/color-scheme) — informs browser-native form controls and page colour-scheme handling.
- [MDN: `prefers-color-scheme`](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/%40media/prefers-color-scheme) — informs system appearance detection.
- [W3C ARIA Authoring Practices Guide](https://www.w3.org/WAI/ARIA/apg/) — informs semantic controls, keyboard support and accessible names.
- [W3C Forms Tutorial](https://www.w3.org/WAI/tutorials/forms/) — informs visible labels and helpful validation feedback.

Implementation choices: plain HTML/CSS/vanilla JS, CSS custom properties, separate appearance and brand palette preferences, `localStorage` for local drafts, and JSON export/import for static-hosting publishing. No external framework or paid API is required.
