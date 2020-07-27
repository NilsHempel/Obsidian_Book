# Obsidian_Book
Them for Obsidian.md that follows classic conventions for printed works

# NH Book
## Idea
Create a theme that respects (*1*) the classic rules of typography for styling and legibility while (*2*) maintaing the usefulness of a digital tool and (*3*) following academic conventions.

## My use case
I made this theme to make research and learning in law as nice as possible. This means that I'm having not only (atomic) notes on specific aspects but also rely heavily on transclusion to create bigger notes that include bot the text of the law (often with the character `§` that needs to look good in the typeface) as well as my notes. In order to highlight specific aspects, I'm using `==mark==`, `*italic*`and `**bold**` to denote specific terminology, negative aspects and positive aspects.  
To accomodate specific cases such as long citations, definitions, etc.

Depending on what I need to to I'm using the markdown files with Obsidian or Hendrik Erz's brilliant [[Zettlr]] with its advantages in citation and output to various formats. These programs get along very well.

## Inspirations
This theme was inspired mainly by:
- Edward [Tufte CSS](https://github.com/edwardtufte/tufte-css)
- The New England Journal of Medicine
- Richard Rutter: [Web Typography](http://www.book.webtypography.net)
- Matthew Butterick: [Practical Typography](https://practicaltypography.com)
- [iA Writer](https://ia.net/writer/blog/a-typographic-christmas)
- [Textus](https://www.textus.io) - unfortunately they didn't seem to make it off the ground.


## Features
### Fonts
To make the distinction between **editing** and **previewing** a file more clear, I chose two markedly different fonts, much like [[iAWriter]]: **Monospaced** for editing and a **serif** font for previewing.  
Ideally, I did want to use free and open-sourced typefamilies only. https://beautifulwebtype.com was an excellent source both for inspiration and downloads.

#### Serif for Preview

- In a serif font I was looking at several factors:
	- how Q and R look
	- ligatures such as fi *fj* æ
	- true **smallcaps**
	- symbols such as § &
	- several localozations to include letters for ß ä and so forth
	- it needs to be dark enough to be comfortably read on-screen
		- i.e. Baskerville is too thin for this reason

- I landed at
	- [Vollkorn](http://vollkorn-typeface.com)
	- [Et Book](https://edwardtufte.github.io/et-book/), like Tufte CSS
		- feel free to change it to [Quadraat](https://www.typeby.com/fonts/quadraat) or *Plantin* if you have access to them. 
		- I didn't set them as the primary fonts as they aren't free and open sourced.

#### Monospaced for Editor

> The typographic rawness of a monospace font tells the writer: “This is not about how it looks, but what it says. Say what you mean and worry about the style later.” Proportional fonts suggest “This is as good as done” and stand in an intimidating contrast to a raw draft.
> <footer> &mdash; Oliver Reichenstein </footer>

- For a monospaced font I wanted several factors
	- visually clearly distinct from the preview font
	- easy to scan
	- looks right with line numbering in the gutter
	- Oliver Reichenstein of iAWriter did a great job of discussing this and designing a great font 
	- [iA Writer Duo](https://github.com/iaolo/iA-Fonts/tree/master/iA%20Writer%20Duospace)
	
### Colors
- Background color: `ivory`
- Main font color: dark grey
	- thus quite a bit more yellow than Tufte CSS
	- in combination with the font the lower contrast helps to reduce eye strain
- Links: in dark blue 
- Mark: background in a lighter shade of the reddish tone used for H2  with corresponding dark brown text

**bold text** 
- rather than a heavy `font-weight`I chose to use a darker color and `style-variant: small-caps`

*italics*
- test


==marked== 
- background in a lighter shade of the reddish tone used for H2  with corresponding dark brown text and border.

#tag
Internal link: [[Art. 1 GG]] 
External Link: http://scriptorium.blog or [Scriptorum](http://scriptorium.blog)
footnote ^[content]
- every item that is clickable is in blue (much like traditional links, albeit in a more subdued shade)

### Headings
I felt that effectively limiting the number of headings to three –like Edward Tufte or Richard Feynman– was a bit constricting. I did define the heading all the way to `h6`, to give you the option to chose them. `h4-h6` are set much smaller and will not use a column span if columns are used.

### Typography
I'm mostly following the guidelines from **Richard Rutter** to set the maximum length of a line to `38em` at `16px`and include all sorts of `hyphenation`. Even longer paragraphs that are `justified` will remain easily legible and look 'neater' than with `align: left` 

`&nbsp;` 
`<br>`

### Columns
Working with columns is not too well supported in many cases. I did include the option to set the body paragraph to two column with `column-span` for headings 1-3. 

### Blockquotes
Several classes of blockquotes are a good way to visually differentiate between content. 

In my case;
1. normal quotes
2. definitions
3. warnings fo typical traps
4. quotes from court ruling
5. quotes form law that I don't want to embed with a tranclusion

#### regular blockquotes

> Blockquotes can use a `<footer>` with `&mdash` to properly display the author's name. They are styled at `font-size: 1.3em` to stand out from the rest of the text and are `position: centered`.
> <footer> &mdash; Max Power (2049) </footer>
	
### Transclusion	
	
I'm using a modified 'naked embed' for transclusions to include the name, which usually is the article of law I'm embedding: 	
	
![[Art. 1 GG]]

---

### Table

The tables have a styled `<caption>`element, so you can properly name them.

|Argument|1.Auffassung|2. Auffassung|
|---|---|---|---|---|
|<th colspan="1">[[Wortlaut]]</th>
|➕||||
|➖
|[[Systematik]]|
|Geschichte|
|[[Normzweck]]|
|[[Normalfall]]|	
<caption><strong>Tab. 1</strong>: Streitstand</caption>	

	
	
### Lists
	
#### Ordered lists

1. First level
	2. Second level
		3. Third level
			4. Fourth level
				5. Fifth level
					6. Sixth level
	2. Second Level
	
#### Unordered lists
	
- First level
	- Second level
		- Third level
			- Fourth level
				- Fifth level
					- Sixth level
	- Second Level
	

