jekyll-tldr
===========

A jekyll documentation theme inspired by readthedocs and sphinx.

Supports documentation via:

- standard pages with a psuedo sub nav based on section headings
- advanced pages organized via a docs collection (collections rendered in page or individual page), query by category, pseudo nav or nav with links to rendered docs
- nested navigation
- sub nav or table of contents with anchor links or links to collections
- sort nav by weight
- sort docs collection by name or weight

### Example Side Nav

- Standard (page)
    - ## heading (anchor)
        - ### sub heading (anchor)
    - ## heading (anchor)
- Advanced w/collection (page)
    - ## Collection Name 1 (anchor)
        - ### sub heading (anchor)
    - ## Collection Name 2 (anchor)
- Advanced w/collection Nested (page)
    - Collection Name 1 (page)
        - ## sub heading (anchor)
            - ### sub sub heading (anchor)
    - Collection Name 2(page)
        - ## sub heading (anchor)

### Notes

For now, the advanced page navigation has to be either anchor link based or linked based (collections are rendered as full html pages), and not a combination of the two. This is because a Collections output can only be set on `_config.yml` and not through the collection document via something like `published: false`. Tracking over at [jekyll/jekyll/issues/2863](https://github.com/jekyll/jekyll/issues/2863)
