Marzena UI
===

UI Library In My Dreams. This is experimental repository to represent a few variants of UI library as platform of shared UI components.

Based on my experience, I worked at least with 2 versions, 2 approaches of how to implement UI components, as library which then shared with different projects.

So this repo represents such versions, at least for information.

**The key to success** of great UI library is - `UI components` and layout regulated by `UX/Designers`. Design dictates how business should evolve on web. For example Twitter Bootstrap or Semantic UI or Materialize or any similar well known UI libraries. They evolve faster than any business who uses the library. And good designers can persuade VBusiness stakeholders that Design matters.

# V1 - Lightweight Version

- Codebase is `monorep`o. Because it's not expected much of logic change, much of variety of features. UI library is simply VIEW of your DATA, and you CONTROL how and where to put it on your web page.
- `Styling` fo UI components developed in `SCSS/LESS` but bundled in `CSS` only. Because it's expected to NOT have hacks, overrides, harmfully towards component itself. Just usage.
- Packaged as single file with set of CSS code for UI/HTML/React components look-n-feel.
- Any JavaScript or minimal logic bundled as separate JavaScript or TypeScript file(s).
- But customization or extend is possible, using `themization` or branding. So that every customer would have their set of files ON TOP of basic design. And if anything changed in main design it should not reflect Branding and vs. Potentially JSS or Styled Components is allowed. TBD.
- Whole repo contains one common `tests` and `storybook` folders.
- `Ideally`, would be great to have Designers team with at least one UI developer, who could extract CSS from InVision/Sketch/PhotoShop/etc software and convert to CSS files and pushed to repo. Then Business related UI development team, just upgrades CSS file with latest Design changes to their codebase, and doesn't change but just use. They can change logic of their components, or logic in the wrappers around shared UI components, but changing of design should be strictly forbidden.

## V1 alternative.

Reusing Bootstrap or Semantic UI as example of possible reusage of basic components layout and customization for LOB/Business with further upgrades and customizations.

Or BEM-based stub. https://en.bem.info/libraries/classic/bem-core/4.2.0/ + https://github.com/bem/project-stub


# V2 - Complex Version

- Codebase is split repositories or branches or git submodules.
- Every component behaves as independent component, with its own repo, tests, storybook, CI flow, npm publish, etc.
- `Styling` of UI components can be CSS for start, but most probably will end up with JSS/Styled Components.
- `Customization` starts disappearing, because every component can be imported/included independently and so that can be extended in different ways.
- Bundled as CommonJS/AMD or any else modern approach but for proper Component-based architecture of web application based on JavaScript/TypeScript/React/Angular.
- Maybe: Should be exported as universal code with no dependency on main development technology.
- `Ideally`, designers work on initial design, and later Business can suggest some features, taken from another LOB to be common/shared.



# Comparison

- Independence: more in V1
- Maintenance: easier in V1
- Customization: easier in V1, but more flexible in V2.
