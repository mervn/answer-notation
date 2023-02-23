<!--
  SPDX-License-Identifer: CC0-1.0 OR Unlicense
  SPDX-FileCopyrightText: 2023 Mervin G.

  SPDX-FileType: DOCUMENTATION
  SPDX-FileType: TEXT

  SPDX-FileComment: Overview of project details.
-->

# An-swer

**This format serves to be a portable, non-proprietary, way to share concise notes
on a topic.**

___

## Format

```json
{
	"title" : "name of book, music, topic, etc",
	"identification" :
	[
		"ean",
		"isbn",
		"ismn",
		"url",
		"etc."
	],
	"dateOfAccess" : "yyyy.mm.dd",
	"section" : "chapter.sub-chapter.subsection.etc",
	"question" : "question this note will answer (i.e. Why is the sky blue?)",
	"definition" :
	[
		{
			"term" : "sky",
			"definition" : "the thing you see when you look up.",
			"source" : "ad hoc"
		},
		{
			"term" : "blue",
			"definition" : "portion of the color spectrum lying between green and violet.",
			"source" : "dictionary"
		}
	],
	"answer" :
	[
		"Blue light is scattered more than the other colors because it travels as shorter, smaller waves.",
		"Sunlight reaches Earth's atmosphere and is scattered in all directions by all the gases and particles in the air."
	],
	"noteFrom" :
	[
		0,
		1,
		5,
		10,
		25
	]
}
```

## Format Breakdown

`title` : Name of the work, include edition numbers.

> Intended for personal-recognition in a local-collection.

`identification` : Standardized identification tags, include **all** applicable IDs.

> A book may have more than one ISBN. Include all of them, unless there's a reason not to.

`dateOfAccess` : The date the work was acquired (i.e. bought, downloaded, recorded, etc.). 

> For dynamic-content, like a URL, use the last date-of-interaction.

`section` : The location, denoted by headers, in the work relevant to the upcoming question.

> For consistent results, all section-names should follow [this][MDLINK] format. If the target-location is inside of another location, use a period - for example, "chapter12.bottle.cap".

`question` : Question to be answered, **this is the focal-point of the note**.

> "Why", and "How", questions tend to be most valuable.

`definition` : Meaning of key-term(s) in the question, terms should be listed in the order they appear left-to-right.

>The only valid values for `source` are "ad hoc" (yourself), "dictionary" (external), "glossary" (from the work).

`answer` : Answer to the question, broken into stages of context. 

> The first entry should directly answer the question, with no explanation. If further explanation is needed, add one short-entry for **each** point.

`noteFrom` : Segments from the section that led to the answer, these are effectively the notes that were taken.

> The only valid value is an integer; where the first-line of the section is '0', and is only incremented when a colon, comma, period, or semicolon is passed.

## Uses

### When To Use:

+ If using interactive-note formats (i.e. Cornell notes, Flashcards, etc.)
+ If note-sharing between large-groups, or over long-distances
+ If a machine-readable note-format is required
+ If revisiting notes is common-occurance

### When Not To Use:

+ If an entry for the work already exists; add to the entry instead.
+ If the project, or group, is standardizing to another note-format
+ If "skimming" the work
+ If the work is an instruction, or syntax, manual

___

## License

This project is dual-licensed under CC0-1.0 OR Unlicense.
<br>
To use this project, you must comply with either license.

```
SPDX-License-Identifier: CC0-1.0 OR Unlicense
SPDX-FileCopyrightText: 2023 Mervin G.
```

> Some files may have different licensing-requirements.
>
> To find the file's applied license,
> search for `SPDX-License-Identifier` with(in) file.
> <br>
> Every license present in this project is listed [here](LICENSES).

<!-- Links -->

[MDLINK]: https://docs.gitlab.com/ee/user/markdown.html#header-ids-and-links