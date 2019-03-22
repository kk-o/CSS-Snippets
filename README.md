# CSS-Snippets

<a href="https://github.com/kk-o/CSS-Snippets" target="_blank">![logo](https://i.imgur.com/2ZcxSA3.png)</a>
[![License](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](https://github.com/kk-o/CSS-Snippets/LICENSE) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![Insight.io](https://img.shields.io/badge/insight.io-Ready-brightgreen.svg)](https://insight.io/github.com/kk-o/CSS-Snippets/tree/master/?source=0)

A curated collection of useful CSS snippets for UI/UX designers. Just a few hundred lines of pure CSS using no external libraries/JavaScript help. Designed to be bite-sized and easy to understand in a minute or less.

http://kikoestrada.com

### View online

https://kk-o.io/CSS-Snippets/

## Table of Contents

<details>
  <summary>View contents</summary>

- [`CSS Resets`](#resets)
- [`Swiss Army Clearfix`](#clearfix)
- [`Selective Rounded Corners`](#corners)
- [`Complex Drop Shadow`](#shadow)
- [`Concise Media Queries`](#queries)
- [`Modern Font Stacks`](#fonts)
- [`SEO Logo Optimization`](#logos)
- [`Vintage Photo Border`](#borders)
- [`Universal Transparency`](#transparency)

</details>

## Contents

### ↪️ Resets

Reset code snippet for all browsers, definitely a must have as it:

- Keeps images responsive
- Sets all core elements to border-box
- Ensures that all margins and padding measurements are aligned properly

<details>
<summary>View Snippet</summary>

```css
* {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
  outline: none;
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
```

</details>

---

### 🌐 Swiss Army Clearfix

This snippet clears up any issues you may be having with floats: any element that comes after a container and its (floating) children will not float but instead be pushed down.

- Effectively clears your floats
- Works in all modern browsers, including legacy I.E. 6-8

<details>
<summary>View Snippet</summary>

```css
clearfix:before, .container:after { content: ""; display: table; }
.clearfix:after { clear: both; }

/* IE 6/7 */
.clearfix { zoom: 1; }
}
```

</details>

---

### 📍 Selective Rounded Corners

Ever wondered how to target and style individual corners of an element?

- Selectively targets an element's top, left, right, bottom corners
- Sets that elements style accordingly
- Works universally

<details>
<summary>View Snippet</summary>

```css
#container {
  -webkit-border-radius: 4px 3px 6px 10px;
  -moz-border-radius: 4px 3px 6px 10px;
  -o-border-radius: 4px 3px 6px 10px;
  border-radius: 4px 3px 6px 10px;
}
```

</details>

---

### 🌚 Complex Drop Shadow

Mimic the elegant shadow used by Google's Material UI

- Utilizes rgba for a more realistic shadow
- Cross-browser support

<details>
<summary>View Snippet</summary>

```css
.card-1 {
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

.card-1:hover {
  box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
}
```

</details>

---

### 📞 Concise Media Queries

Use this snippet as an elegant solution for any of your tablet/mobile needs

- Templates media queries for smartphones, tablets, laptops & desktops
- Works universally across all browsers

<details>
<summary>View Snippet</summary>

```css
/* Smartphones (portrait and landscape) ----------- */
@media only screen and (min-device-width: 320px) and (max-device-width: 480px) {
  /* Styles */
}

/* Smartphones (landscape) ----------- */
@media only screen and (min-width: 321px) {
  /* Styles */
}

/* Smartphones (portrait) ----------- */
@media only screen and (max-width: 320px) {
  /* Styles */
}

/* Tablets (portrait and landscape) ----------- */
@media only screen and (min-device-width: 768px) and (max-device-width: 1024px) {
  /* Styles */
}

/* Tablets (landscape) ----------- */
@media only screen and (min-device-width: 768px) and (max-device-width: 1024px) and (orientation: landscape) {
  /* Styles */
}

/* Tablets (portrait) ----------- */
@media only screen and (min-device-width: 768px) and (max-device-width: 1024px) and (orientation: portrait) {
  /* Styles */
}

/* Desktops and laptops ----------- */
@media only screen and (min-width: 1224px) {
  /* Styles */
}
```

</details>

---

### ✏️ Modern Font Stacks

Here's an assortment of stylish, versatile, fonts and most importantly free fonts to use in your projects:

<details>
<summary>View Snippet</summary>

```css
/* Times New Roman-based serif */
font-family: Cambria, "Hoefler Text", Utopia, "Liberation Serif",
  "Nimbus Roman No9 L Regular", Times, "Times New Roman", serif;

/* A modern Georgia-based serif */
font-family: Constantia, "Lucida Bright", Lucidabright, "Lucida Serif", Lucida,
  "DejaVu Serif," "Bitstream Vera Serif", "Liberation Serif", Georgia, serif;

/*A more traditional Garamond-based serif */
font-family: "Palatino Linotype", Palatino, Palladio, "URW Palladio L",
  "Book Antiqua", Baskerville, "Bookman Old Style", "Bitstream Charter",
  "Nimbus Roman No9 L", Garamond, "Apple Garamond", "ITC Garamond Narrow",
  "New Century Schoolbook", "Century Schoolbook", "Century Schoolbook L",
  Georgia, serif;

/*The Helvetica/Arial-based sans serif */
font-family: Frutiger, "Frutiger Linotype", Univers, Calibri, "Gill Sans",
  "Gill Sans MT", "Myriad Pro", Myriad, "DejaVu Sans Condensed",
  "Liberation Sans", "Nimbus Sans L", Tahoma, Geneva, "Helvetica Neue",
  Helvetica, Arial, sans-serif;

/*The Verdana-based sans serif */
font-family: Corbel, "Lucida Grande", "Lucida Sans Unicode", "Lucida Sans",
  "DejaVu Sans", "Bitstream Vera Sans", "Liberation Sans", Verdana,
  "Verdana Ref", sans-serif;

/*The Trebuchet-based sans serif */
font-family: "Segoe UI", Candara, "Bitstream Vera Sans", "DejaVu Sans",
  "Bitstream Vera Sans", "Trebuchet MS", Verdana, "Verdana Ref", sans-serif;

/*The heavier "Impact" sans serif */
font-family: Impact, Haettenschweiler, "Franklin Gothic Bold", Charcoal,
  "Helvetica Inserat", "Bitstream Vera Sans Bold", "Arial Black", sans-serif;

/*The monospace */
font-family: Consolas, "Andale Mono WT", "Andale Mono", "Lucida Console",
  "Lucida Sans Typewriter", "DejaVu Sans Mono", "Bitstream Vera Sans Mono",
  "Liberation Mono", "Nimbus Mono L", Monaco, "Courier New", Courier, monospace;
```

</details>

---

### 🔍 SEO Logo Optimization

Search engines can crawl your website for logo text, but will fail to find anything if you're using an image as a logo (like many do). This approach creates invisible logo text for the search engine robots to pull data from.

- Effectively creates a pure text version of your logo
- This logo is invisible and won't appear anywhere
- Works against all browsers

<details>
<summary>View Snippet</summary>

```css
h1 {
  text-indent: -9999px;
  margin: 0 auto;
  width: 320px;
  height: 85px;
  background: transparent url("images/your_logo.png") no-repeat scroll;
}
```

</details>

---

### 🖼️ Vintage Photo Border

Use this snippet for a Polaroid-like border effect for your images

- Mimics the classic white frame found in polaroid photos
- Universal support out of the box

<details>
<summary>View Snippet</summary>

```css
h1 {
  text-indent: -9999px;
  margin: 0 auto;
  width: 320px;
  height: 85px;
  background: transparent url("images/your_logo.png") no-repeat scroll;
}
```

</details>

---

### 👀🚫 Cross-Browser Transparency

Stop worrying about transparency issues because, when applied, any element will be completely invisible

- Works across all browsers

<details>
<summary>View Snippet</summary>

```css
h1 {
  text-indent: -9999px;
  margin: 0 auto;
  width: 320px;
  height: 85px;
  background: transparent url("images/your_logo.png") no-repeat scroll;
}
```

</details>

<br>[⬆ Back to top](#contents)
