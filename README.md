Marzena UI
===

UI Library In My Dreams. This is experimental repository to represent a few variants of UI library as platform of shared UI components.

Based on my experience, I worked at least with 2 versions, 2 approaches of how to implement UI components, as library which then shared with different projects.

So this repo represents such versions, at least for information.

The key to success of such UI library is - `UI components` and layout regulated by `UX/Designers`. Design dictates how business should evolve on web. For example Twitter Bootstrap or Semantic UI or Materialize or any similar well known UI libraries. They evolve faster than any business who uses the library. And good designers can persuade VBusiness stakeholders that Design matters.

# V1

- Codebase is `monorep`o. Because it's not expected much of logic change, much of variety of features. UI library is simply VIEW of your DATA, and you CONTROL how and where to put it on your web page.
- `Styling` fo UI components developed strictly in `CSS/SCSS/LESS` and it's expected to NOT have hacks, overrides, harmfully towards component itself.
- But customization or extend is possible, using `themization` or branding. So that every customer would have their set of files ON TOP of basic design. And if anything changed in main design it should not reflect Branding and vs. Potentially JSS or Styled COponents is allowed. TBD.
- Whole repo contains one common `tests` and `storybook` fodlers.

# V2

- Codebase is split repositories or branches or git submodules.
- Every component behaves as independent component, with its own repo, tests, storybook, CI flow, npm publish, etc.
- `Styling` of UI components can be CSS for start, but most probably will end up with JSS/Styled Components.


# Comparison

TBD
