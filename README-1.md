# Our Boighar — file storage #1

Overflow file storage for [Our Boighar](https://mdtowfiqul.github.io/our-boighar/)
(MDTowfiqul/our-boighar). This repo only hosts ebook files — another 1 GB of
free GitHub Pages space — for when the main repo's book files grow too large.

Book files live in `books/`. The main site links to them with full URLs like:

```
https://mdtowfiqul.github.io/our-boighar-files-1/books/<filename>.epub
```

In the main repo, a book whose file lives here gets this in its
`_books/<slug>.md` front matter instead of a local path:

```yaml
file: "https://mdtowfiqul.github.io/our-boighar-files-1/books/<filename>.epub"
```

GitHub Pages serves these files with `Access-Control-Allow-Origin: *`, so the
main site's online reader and downloads work across the two repos.
