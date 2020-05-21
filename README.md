<h1 align="center">
  <a href="https://github.com/posquit0/Awesome-CV" title="AwesomeCV Documentation">
    <img alt="AwesomeCV" src="https://github.com/posquit0/Awesome-CV/raw/master/icon.png" width="200px" height="200px" />
  </a>
  <br />
  Awesome CV
</h1>

<p align="center">
  LaTeX template for your outstanding job application
</p>

<br />

## What is Awesome CV?

**Awesome CV** is LaTeX template for a **CV(Curriculum Vitae)**, **Résumé** or **Cover Letter** inspired by [Fancy CV](https://www.sharelatex.com/templates/cv-or-resume/fancy-cv). It is easy to customize your own template, especially since it is really written by a clean, semantic markup.

Based on [Awesome CV](https://github.com/posquit0/Awesome-CV), I did some layout changes and includes bibtex (see this [PR](https://github.com/posquit0/Awesome-CV/pull/23/files)) for showing publications.

## Preview

#### CV

You can see [PDF](https://raw.githubusercontent.com/pcwang23/Awesome-CV/master/examples/cv.pdf)

| Page. 1 | Page. 2 |
|:---:|:---:|
| (https://raw.githubusercontent.com/pcwang23/Awesome-CV/master/examples/cv-0.png)| (https://raw.githubusercontent.com/pcwang23/Awesome-CV/master/examples/cv-1.png)|

## How to Use

#### Requirements

A full TeX distribution is assumed.  [Various distributions for different operating systems (Windows, Mac, \*nix) are available](http://tex.stackexchange.com/q/55437) but TeX Live is recommended.
You can [install TeX from upstream](http://tex.stackexchange.com/q/1092) (recommended; most up-to-date) or use `sudo apt-get install texlive-full` if you really want that.  (It's generally a few years behind.)

#### Usage

At a command prompt, run

```bash
$ xelatex {your-cv}.tex
$ biber {your-cv}
$ xelatex {your-cv}.tex
```

This should result in the creation of ``{your-cv}.pdf``

#### Issue

You might encounter error shows:
```bash
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
!
! fontspec error: "font-not-found"
! 
! The font "FontAwesome" cannot be found.
! 
! See the fontspec documentation for further information.
! 
! For immediate help type H <return>.
!............................................... 
```
This indicate that `FontAwesome` is not installed in your environment. Go to [**Font-Awesome**](http://github.com/FortAwesome/Font-Awesome/blob/v4.7.0/fonts/FontAwesome.otf) and download this. In mac, you can move it into your application Font Book as installation.

Add a new line in your `cv.tex` for xelax to use this font:
```bash
\usepackage{fontawesome}
```


## Credit

[**LaTeX**](http://www.latex-project.org) is a fantastic typesetting program that a lot of people use these days, especially the math and computer science people in academia.

[**LaTeX FontAwesome**](https://github.com/furl/latex-fontawesome) is bindings for FontAwesome icons to be used in XeLaTeX.

[**Roboto**](https://github.com/google/roboto) is the default font on Android and ChromeOS, and the recommended font for Google’s visual language, Material Design.

[**Source Sans Pro**](https://github.com/adobe-fonts/source-sans-pro) is a set of OpenType fonts that have been designed to work well in user interface (UI) environments.


## See Also

* [Awesome Identity](https://github.com/posquit0/hugo-awesome-identity) - A single-page Hugo theme to introduce yourself.
