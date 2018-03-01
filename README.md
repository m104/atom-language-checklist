# language-checklist
Atom syntax highlighting for checklist (`*.check`, `*.checklist`) files.

## Checklist Syntax

Checklist files are organized into line items in various states. Items may be nested at any depth with
indentation (two spaces recommended). Each line item's state depends on the first character of the
line, followed by a space:

* `-` Unchecked/pending item
* `+` Checked/completed item
* `?` Question yet to be answered
* `*` Informational item or answered question

Tags may be applied to any item by adding `[TagName]`.

## Example

![Example Screenshot](/examples/screenshot.png?raw=true "Example Screenshot")

```
Reading List
  Fantasy
    - Scadrial Series [Sanderson]
      + The Alloy of Law
      - Shadows of Self
      - The Bands of Mourning
      - The Lost Metal - Fall 2019
    ? Warbreaker [Sanderson]
    - The Grishaverse Series [Bardugo]
      * https://www.goodreads.com/series/69714-the-grishaverse
      - Shadow and Bone
      - Seige and Storm
      - Ruin and Rising

  Sci-Fi
    - Remembrance of Earth’s Past [Liu]
      + The Three-Body Problem
      - The Dark Forest
      - Death’s End
```

## Development

- Open with grammar reloading:
  - Add the project to Atom's packages `apm link .`
  - Open the project in development mode `atom --dev .`
  - Create a `scratch.checklist` file to check highlighting

## License

MIT
