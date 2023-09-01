## Linguist

This library is used on GitHub.com to detect blob languages, ignore binary or vendored files, suppress generated files in diffs, and generate language breakdown graphs. [language.yml](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)

### Change Language

- Create file `.gitattributes` in empty directory

```
* linguist-detectable=false
*.yml linguist-detectable=true
```

**NOTE:** [READ MORE](https://dev.to/katkelly/changing-your-repo-s-language-in-github-5gjo)