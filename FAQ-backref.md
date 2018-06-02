---
title: References from the bibliography to the citation
category: bibliographies
tags: citations
permalink: /FAQ-backref
date: 2014-06-10
---

A link (or at least a page reference), from the bibliography to the
citing command, is often useful in large documents.

Two packages support this requirement, [`backref`](https://ctan.org/pkg/backref) and
[`citeref`](https://ctan.org/pkg/citeref).  [`Backref`](https://ctan.org/pkg/Backref) is part of the
[`hyperref`](https://ctan.org/pkg/hyperref) bundle, and supports hyperlinks back to the citing
command.

[`Citeref`](https://ctan.org/pkg/Citeref) is the older, and seems to rely on rather simpler
(and therefore possibly more stable) code; it produces a list of page
references, only.  It doesn't interact well with other citation
packages (for example, [`cite`](https://ctan.org/pkg/cite)), which probably reflects its
antiquity (it's derived from a LaTeX 2.09 package).

Neither collapses
lists of pages (`5, 6, 7` comes out as such, rather than as
`5-7`), but neither package repeats the reference to a page that
holds multiple citations.  (The failure to collapse lists is of course
forgiveable in the case of the [`hyperref`](https://ctan.org/pkg/hyperref)-related
[`backref`](https://ctan.org/pkg/backref), since the concept of multiple hyperlinks from the
same anchor is less than appealing.)

