# Position test

```bash
git clone https://github.com/black-desk/lsp-position-test
cd lsp-position-test
go build
nvim ./README.md
```

ağb

> A position inside a document (see Position definition below) is expressed as a zero-based line and character offset. The offsets are based on a UTF-16 string representation. So a string of the form ağb the character offset of the character a is 0, the character offset of ğ is 1 and the character offset of b is 3 since ğ is represented using two code units in UTF-16.

https://microsoft.github.io/language-server-protocol/specifications/specification-current/#textDocuments

Hover on `b`, then coc will report a Position with Character equals 2.
