# Technical Writing

The following is my approach to writing documentation / technical specs.

These principles are also demonstrated in this set of Sample Technical Specs I wrote.

## Principles

The following is generally based on writing specs in Confluence, but the same principles are valuable in general.

- Keep everything D.R.Y. (Don't Repeat Yourself). Each piece of information should be stated only once.
  - This typically means abstracting all common information up to a parent document, then hyperlinking each child document up to the parent.
    - Only hyperlink documents one level up. (If there are no specifics to add in a middle layer, simply pass the reader up to the next layer.)
  - This is important for keeping the specs easy to maintain. If a change must be made later, it will only have to be made in one place.