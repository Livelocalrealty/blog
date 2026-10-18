# LivingLocal Realty Blog

Static blog for Thomas Moriarty, LivingLocal Realty (Maple Grove, MN), served by GitHub Pages at
https://livelocalrealty.github.io/blog/

No build step. Plain HTML + one stylesheet (`assets/style.css`). `.nojekyll` disables Jekyll.

## Publishing a post (Tue/Fri)
1. Copy `posts/_template.html` to `posts/<slug>.html` and fill every `{{PLACEHOLDER}}`.
2. Change the robots meta from `noindex, nofollow` to `index, follow`.
3. In `index.html`: add a `<li class="post-card">` inside `#post-list` (newest first), remove the `#empty-state` block, and add the post to the Blog JSON-LD `blogPost` array.
4. Add the post URL to `sitemap.xml` (never add `_template.html`).

## Rules
- Every http(s) link: `target="_blank" rel="noopener"` (mailto/tel/#anchors exempt).
- No em dashes in public copy.
- No placeholder or fake posts.
