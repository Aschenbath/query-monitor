# Query Monitor log selection evidence

Real WordPress 7.1.5, PHP 8.3.37 and Google Chrome 158 on Windows.
The repository Docker Compose acceptance environment generated a synthetic log message.
Both screenshots show the same mouse double-click in the first word.

- Before: develop@b284bffc4d6ad1966802c4323a508e0cf29a225d selects the entire message.
- After: removing the logger's user-select: all rule selects only Select (plus the normal trailing space on Windows).

The final acceptance regression fails before the CSS removal and passes afterward.
Logger, Basic, HtmlBlock and ThirdPartyPanel acceptance specs: 10 passed.
Screenshots are unedited full-page captures of the local synthetic test installation.
