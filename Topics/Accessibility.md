- https://adamsilver.io/blog/building-an-accessible-autocomplete-control/
- Egghead: Start Building Accessible Web Applications Today
- [What I've learned about motor impairment](http://simpleprimate.com/blog/motor)
- https://a11y-style-guide.com/style-guide/section-forms.html
- https://www.smashingmagazine.com/2021/03/good-better-best-untangling-complex-world-accessible-patterns/
- http://book.inclusive-components.design/
- Tools
    - [Accessibility Support](https://a11ysupport.io/), [Michael Fairchild](https://twitter.com/mfairchild365), a11ysupport.io
    - [HTML5 Accessibility](https://stevefaulkner.github.io/HTML5accessibility/), [Steve Faulkner](https://twitter.com/stevefaulkner)
- Pattern Libraries
    - [Accessibility Project](https://www.a11yproject.com/resources/)
    - [Accessibility Style Guide](https://a11y-style-guide.com/style-guide/)
    - [Accessible Components](https://www.scottohara.me/code/), [Scott O’Hara](https://twitter.com/scottohara)
    - [Accessible drag-and-drop List Reorder Plugin](https://schne324.github.io/dragon-drop/demo/), [Harris Schneiderman](https://twitter.com/theHarrisius)
    - [Deque’s ARIA Pattern Library](https://dequeuniversity.com/library/)
    - [Deque’s Accessible React Library](https://cauldron.netlify.app/)
    - [GOV.UK Design System](https://design-system.service.gov.uk/)
    - [Inclusive Components](https://inclusive-components.design/), [Heydon Pickering](https://twitter.com/heydonworks)
    - [U.S. Web Design System (USWDS)](https://designsystem.digital.gov/documentation/developers/)
    - [Web Accessibility Tutorials](https://www.w3.org/WAI/tutorials/)
- https://developer.mozilla.org/en-US/docs/Web/Accessibility
- https://a11y-with-lindsey.ck.page/products/pre-order-the-bootcampers-guide-to-web
- Inclusive Components by Heydon Pickering on Smashing Magazine
    - https://www.smashingmagazine.com/printed-books/inclusive-components/
- Accessible Typography
    - [Contrast: Tool for WCAG color contrast ratios](https://usecontrast.com/)
    - Backlit screens can increase the contrast between pure black and white, which can be tiring on the eyes, so using a softer black for text or pale grey background can make text more readable.
    - [Snook.ca color contrast checker](https://snook.ca/technical/colour_contrast/colour.html#fg=33FF33,bg=333333)
    - Choosing a font
        - A good web font features
            - consisten stroke weights
            - higher x-heights
            - more open bowls and counters
        - Avoid crazy typefaces, condensed styles and letterforms with thin strokes.
        - Go with something simple and of a standard weight to ensure readability on all devices, especially for long paragraphs of text.
    - Type effects such as shadows or bevels may look great at larger sizes but won’t work on small screens.
    - Setting type
        - Pay attention to paragraph measure; keep them to between 45-75 characters.
        - Provide generous spacing between lines: aim for a minimum line height of 1.5 for body copy.
        - Aim for a slight increase in tracking, to give type room to breathe.
        - Choose a reasonable point size: actual character size varies between fonts, but 16px is a good minimum.
- Accessible HTML
    - HTML Email
        - When using <table> elements for layout in an email, use role="presentation" to keep screen readers from treating them as tables
            - Child tables don't inherit this, you need to declare it in every table
    - Don't use the "placeholder" element
        - placeholder elements are not translated by the browser
        - `<label>` elements should ALWAYS have a `for=""` attribute that matches the input's `id=""` attribute
            - Without for/id pairing, assistive technology can't determine what input is for.
            - Pairing makes clicking or tapping on label place focus on input. Provides extra area for interacting, beneficial to people with motor control issues
        - will disappear when information is entered
            - means guiding language is removed on interaction
        - placeholder text may look like content, confusing user
        - limited to just a string of static text
        - length limited to the width of the input, could be truncated
        - Can have insufficient contrast with background, or be too dark making it look like content

[[Website Accessibility, v2 - Jon Kuperman]]

