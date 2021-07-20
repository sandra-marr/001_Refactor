# Homework01 - SRM

# 01 HTML, CSS, and Git: Code Refactor

## Summary

The purpose of this project was to review and update the existing code to improve accessibility for web users and readability of the code for any future developers. Generally, the look and functionality of the website was intended to remain unchanged. The user story and acceptance criteria is listed below: 

### User Story

```
AS A marketing agency
I WANT a codebase that follows accessibility standards
SO THAT our own site is optimized for search engines
```

### Acceptance Criteria

```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title
```

## HTML Analysis

The overall structure of the HTML was good, however there was a need for improved semantics. Rather than using only `<div>` elements, I focused on adding in `<header>`, `<nav>`, `<section>`, `<aside>`, and `<footer>` elements where applicable. These changes also made it possible to remove some class attributes (i.e. instead of having a class="header", we could use the `<header>` element).

Without more knowledge of the intent that the business had for the images used in their webpage, it appeared that the images were for visual aesthetics only, so alt tags were added but left blank. 

There was also some clean up on the links internal to this webpage. This was done by adding in id attributes to any sections that were previously missing them.

The content of the page did not change with any of these updates. 

## CSS Analysis

The first round of updates made to the CSS file were related to the semantic updates made in the HTML file.
One example of this was to change class selectors to element selectors. 

Another area of improvement was in the redundant styles in the CSS file. To simplify the CSS, ids and classes were cleaned up in the HTML file, and then the selectors in CSS were updated to reflect those changes. For example, rather than having three identical style blocks for the benefit class headers, now there is only one. 

At each stage in making updates, the webpage was opened, refreshed, and inspected inorder to ensure that the over all look and functionality did not change. 

## Inspect - What a great tool!

The major benefit to this first assignment that I found was the ability to learn how to navigate the inspect tool in chrome. As I was making changes, and getting stuck, the inspect tool really helped me to understand what was happening. I also learned about Lighthouse to assess the accessibility, speed, SOE, etc. That seems like a great learning tool. 

## End Result
Here is a link to the deployed page: https://sandra-marr.github.io/001_Refactor/

If done correctly, the webpage for Horiseon should look like this:

![The Horiseon webpage includes a navigation bar, a header image, and cards with text and images at the bottom of the page.](/assets/01-html-css-git-homework-demo.png)

## MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

&copy;2021 Sandra Marr

