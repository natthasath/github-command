## LF will be replaced by CRLF in git

LF (Line Feed) and CRLF (Carriage Return + Line Feed) are two different newline characters used to represent the end of a line in text files. The choice between LF and CRLF line endings depends on the operating system and software conventions. Here's how they would be displayed in a tabular format:

| Abbreviation | Name                             | Code           | Usage                                      |
|--------------|----------------------------------|----------------|--------------------------------------------|
| LF           | Line Feed                        | `\n`           | Unix-like systems (Linux, macOS)           |
| CRLF         | Carriage Return + Line Feed      | `\r\n`         | Windows                                    |

### Warning Message

```
warning: CRLF will be replaced by LF in <file-name>.
The file will have its original line endings in your working directory.
```

### Fix: use git config

```
git config core.autocrlf true
git config --global core.autocrlf true
```

### Fix: use .gitattributes

```
* text=auto eol=crlf
```

**NOTE:** [READ MORE](https://www.aleksandrhovhannisyan.com/blog/crlf-vs-lf-normalizing-line-endings-in-git/)