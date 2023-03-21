# HTML & CSS clean code guide
_Source: Google HTML & CSS guide_[^1]
[^1]: > https://google.github.io/styleguide/htmlcssguide.html

Rule|Example
-|-
[Comment](#comment)|Explain code as needed, where possible
[HTML5](#html5)|Use HTML5 as text/html
[HTTPS](#https)|Use HTTPS for embedded resources where possible
[Indent](#indent)|Indent by 2 spaces at a time
[Lowercase](#lowercase)|Use only lowercase
[TODO](#todo)|Mark todos and action items with `TODO`
[UTF-8](#utf-8)|Use UTF-8 (no BOM)
[Validity](#validity)|Use valid HTML code
[Void elements](#void-elements)|Do not close void elements
[Whitespace](#whitespace)|Avoid trailing whitespace(s)
**Semantics**

## HTTPS
> [<<<](#)
- Use HTTPS for embedded resources where possible
> HTML:
```
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.0/jquery.min.js"></script>
```

## Indent
> [<<<](#)
- Indent by 2 spaces at a time (don’t use tabs or mix tabs and spaces for indentation)
> HTML:
```
  <ul>
    <li>Fantastic
    <li>Great
  </ul>
```
> CSS:
```
  .example {
    color: blue;
  }
```

## Lowercase
> [<<<](#)
- Use only lowercase
> HTML:
```
  <img src="google.png" alt="Google">
```
> CSS:
```
  color: #e5e5e5;
```

## Whitespace
> [<<<](#)
- Avoid trailing whitespace(s)

## UTF-8
> [<<<](#)
- Use UTF-8 (no BOM[^2])
[^2]: The UTF-8 BOM is a sequence of bytes at the start of a text stream (_0xEF, 0xBB, 0xBF_) that allows the reader to guess a file as being encoded in UTF-8.
> HTML:
```
  <meta charset="utf-8">
```

## Comment
> [<<<](#)
- Explain code as needed, where possible
> HTML:
```
  <!-- TODO: remove optional tags -->
```

## TODO
> [<<<](#)
- Mark todos and action items with `TODO` only (not other common formats, like @@)
- Append a contact (username or mailing list) in parentheses as with the format `TODO(contact)`
- Append action items after a colon as in `TODO: action`
> HTML:
```
  <!-- TODO: remove optional tags -->
```
> CSS:
```
  {# TODO(john.doe): revisit centering #}
```

## HTML5
> [<<<](#)
- Use HTML5 content as text/html (before HTML5: `<meta http-equiv="Content-Type" content="text/html>`)
> HTML:
```
  <!DOCTYPE html>
  <meta charset=UTF-8">
```

## Void elements
> [<<<](#)
- Do not close void elements
> HTML:
```
  <!-- Use <br> instead of <br /> -->
  <br>
```

## Validity
> [<<<](#)
- Use valid HTML code
- Use tools such as the [W3C HTML validator](https://validator.w3.org/nu/) to test
