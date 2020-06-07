# Helpers

Small helpers that make stuff a little easier

## Setup

Clone the repository and add it to your `PATH`

## Tools

### pdfcat

A tiny wrapper around `pdftotext` which expects a pdf as a first argument and prints the text to stdout.
Useful for git diff of pdf, by adding

```
*.pdf diff=pdfdiff
```

to `.gitattributes` of a project repo, and

```
[diff "pdfdiff"]
	textconv = pdfcat
```

to `~/.gitconfig`
