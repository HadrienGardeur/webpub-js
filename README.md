# Web Publication JS

This project is a proof of concept for handling Web Publications and the [Web Publication Manifest](https://github.com/HadrienGardeur/webpub-manifest) in a browser.

In its current state, it can already be re-used, as long as a publication links to:

- a Web Publication Manifest using a `<link>` element in the document
- a Web App Manifest that points to a Web Publication Manifest using `publication`

It is meant to be embedded in the resources of the publication, this project is not a Web App meant to display Web Publications. 

For the Web App use case, check [Dave Cramer's ACME Publishing](https://github.com/dauwhe/epub-zero/tree/gh-pages/acme-publishing).

##Current Features

The current version of the Web Publication JS supports the following features:

- resources from the publication are cached and served offline by a Service Worker using a network first then cache policy
- navigation between documents is injected in the current document using a `<nav>` element

##Potential Features

A separate Wiki page is available with a list of potential features that are relevant in Web Publications: https://github.com/HadrienGardeur/webpub-manifest/wiki/Web-Publication-JS-Features

##Live Demo

A live demo of a Web Publication is available at: https://hadriengardeur.github.io/webpub-manifest/examples/MobyDick/index.html

The manifest for this demo is available at: https://hadriengardeur.github.io/webpub-manifest/examples/MobyDick/manifest.json
