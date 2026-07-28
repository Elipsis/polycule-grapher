# Welcome to the GitHub Polycule Grapher!

The GitHub Polycule Grapher is designed to create a single source of truth to share and update with your polycule.  All you need to do, collaboratively, is maintain a text file!

## The Technology

The GitHub Polycule Grapher is powered by [Graphviz](https://graphviz.org/) and relies on [GitHub Actions](https://github.com/features/actions) to update the graph renders upon a successful push to the `DOT/*.dot` directory.

## Privacy and Consent

The Polycule Grapher runs on the internet, and as such all information placed in this repository is visible to the public.  GitHub also keeps a history of previous versions of files, which means removing relationships, individuals, or other information from the source files will not completely scrub it from record.

**Obtain consent from everyone involved before putting their name on a public facing polycule graph!**  Consider the use of aliases, first name only, or even blank circles to protect the identities of those who are not comfortable being openly named as poly.

Lastly, while I would love to see many other GitHub users adding their own .DOT files - only do so if you are comfortable with this activity appearing in your contribution history.

## Usage

Create a PR which adds or updates a .DOT file containing your unique polycule info.  Once merged, a graph will appear in the corresponding directory.

The example found in `DOT/Sample Lesbian Quad.dot` shows how simple the file format can be.

```
graph SampleLesbianQuad {
    layout=circo

	Alice -- Beatrix
	Alice -- Carol
	Alice -- Eve
	Beatrix -- Eve
	Beatrix -- Carol
	Carol -- Eve
}
```

This produces the following graph:

![screenshot of rendered graph](https://github.com/Elipsis/polycule-grapher/blob/main/Renders/Sample%20Lesbian%20Quad.svg)

which is visible in `Renders/Sample Lesbian Quad.svg`.  You can share this with your sample polycule with [a permanent link](https://raw.githubusercontent.com/Elipsis/polycule-grapher/refs/heads/main/Renders/Sample%20Lesbian%20Quad.svg) to the rendered .SVG file.

## Creating Fancier Graphs

Sites such as [GraphViz Online](https://dreampuf.github.io/GraphvizOnline/?engine=circo#graph%20SampleLesbianQuad%20%7B%0A%20%20%20%20layout%3Dcirco%0A%0A%09Alice%20--%20Beatrix%0A%09Alice%20--%20Carol%0A%09Alice%20--%20Eve%0A%09Beatrix%20--%20Eve%0A%09Beatrix%20--%20Carol%0A%09Carol%20--%20Eve%0A%7D) allow you to create and test Graphviz files online.  Here you can create and preview your polycule maps before you upload a persistent version to this repository.
