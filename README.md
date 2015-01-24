# normality

Normality is a Python micro-package that contains a small set of text
normalization functions for easier re-use. These functions accept a
snippet of unicode or utf-8 encoded text and remove various classes
of characters, such as diacritics, punctuation etc. This is useful as
a preparation to further text analysis.

## Example

```python
# coding: utf-8
from normality import normalize, slugify

text = normalize('Nie wieder "Grüne Süppchen" kochen!')
assert text == 'nie wieder gruene sueppchen kochen'

slug = slugify('My first blog post!')
assert slug == 'my-first-blog-post'
```

## Extended usage

Read the source code, it's twenty lines of stuff.

## License

``normality`` is open source, licensed under a standard MIT license
(included in this repository as ``LICENSE``).
