# Sakuga VFX

Shared in [CodeGizm's X post](https://x.com/codegizm/status/2125520261852065854): a free, MIT-licensed set of anime-inspired effects for ordinary UI controls. The live [gallery](https://sakuga-vfx.vercel.app/gallery) demonstrates twelve standalone web components, including buttons, toggles, sliders, checkboxes, tabs, progress, ratings, toasts, and tooltips.

- Upstream: [finktheartist/sakuga-vfx](https://github.com/finktheartist/sakuga-vfx)
- Your individual fork: [benyamin-persia/sakuga-vfx](https://github.com/benyamin-persia/sakuga-vfx)
- Each component can be copied by hand or added via the upstream's shadcn CLI registry; see its README for the exact component commands and API.

Accessibility and layout notes from upstream: `prefers-reduced-motion` turns off the effects, but the project has not yet been tested with a screen reader or on a real phone. Its effects canvas uses a very high z-index and can draw over modals or sticky headers, so check stacking behavior in your app.
