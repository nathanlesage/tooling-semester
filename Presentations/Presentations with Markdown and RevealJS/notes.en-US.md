# Notes

This course depends upon the slides and this file contains notes to be read/presented during the presentation. The course block also offers several tasks that will familiarize the students with using this.

## Introduction

- In the academic world, presenting is one of the essential key-skills
- Most only ever user proprietary software such as Keynote, PowerPoint, or traditional Open Source-programs such as LibreOffice/OpenOffice
- This course offers an additional solution: Markdown based presentations

## Slide: Problems of traditional presentations

- Most presentation formats require the corresponding program to be installed on the presentation computer, such as Microsoft PowerPoint, Apple Keynote, or LibreOffice.
- But you don't necessarily know in advance if it's available or not
- If we think: What is the only software that we can be absolutely sure about that it is installed on every computer? Answer: A web browser

## Slide: Web Browser

- A web browser is being used to surf the web.
- It includes features that enable advanced layouting -- every page looks different, some more beautiful, some less so.
- Also, it includes means to make a website "interactive", that is: You can click around and things happen dynamically as you interact with the page
- But a web browser not necessarily needs to access websites on the internet. It can also display files on your computer.

## Slide: HTML-files

- HTML files contain the structure of a website, its appearance, and interactive contents (note: CSS + JavaScript can also be external)
- The idea: Why not create a "website" that re-defines what your browser is good for? If you imagine a website that only contains of one page, and add some interactivity so that you can press the arrow keys to navigate it, then you actually have a presentation.
- There are several tools to create such HTML-presentations, but today we focus on reveal.js

## Slide: Reveal.js

- Reveal.js is a framework by Hakim el-Hattab that takes a basic HTML file, and by using a style-file (CSS) and the JavaScript-file containing the program (reveal.js) turns it into a presentation.
- We do not need to understand the exact structure of reveal.js here, because:
- Pandoc actually includes a writer that reads in a Markdown file, and outputs a full, working reveal.js presentation!

## Slide: Markdown + Reveal.js

- However, the Markdown needed for reveal.js must look different than the ordinary Markdown file you write
- Additionally, you cannot use some advanced features of reveal.js, such as nested slides
- But for almost every presentation, what you can achieve suffices

_Note: Here you can direct your students to already create a file "slides.md" (or similar)._

## Slide: The reveal-Markdown

- Problem: How do you tell Pandoc "This slides goes from here to there?"
- First solution: Use headings. And it actually works! Using headings level 1 and 2 creates new slides automatically.
- But sometimes you don't want headings, or need something else to declare a page-change. How do you do this? Answer: horizontal rules (e.g. `***` or `---`)
