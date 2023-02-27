<!--
  SPDX-License-Identifer: CC0-1.0 OR Unlicense
  SPDX-FileCopyrightText: 2023 Mervin G.

  SPDX-FileType: DOCUMENTATION
  SPDX-FileType: TEXT

  SPDX-FileComment: Overview of project details.
-->

# Answer Notation

**This notation is an approach to taking, sharing, and storing concise notes.**

```json
{
	"title" : "Blue Skies Only",
	"identification" :
	[
		{
			"tag" : "isbn-10",
			"token" : "0000000000"
		},
		{
			"tag" : "isbn-13",
			"token" : "978-0000000000"
		},
		{
			"tag" : "url",
			"token" : "skycolors.edu"
		}
	],
	"dateOfAccess" : "2023.02.25",
	"question" : "Why is the sky blue?",
	"definition" :
	[
		{
			"term" : "sky",
			"hint" : "the thing you see when you look up.",
			"source" : "made it up"
		},
		{
			"term" : "blue",
			"hint" : "portion of the color spectrum lying between green and violet.",
			"source" : "merriam-webster"
		}
	],
	"answer" : "Blue light is scattered more than the other colors because it travels as shorter, smaller waves.",
	"highlight" :
	[
		{
			"section" : "5.1.*",
			"significant" : true,
			"content" : "Sunlight reaches Earth's atmosphere and is scattered in all directions by all the gases and particles in the air"
		},
		{
			"section" : "7.3.0",
			"significant" : false,
			"content" : "Blue skies rock"
		}
	]	
}
```

___

## Elements

`title` : Name, with edition-number, of the work.

`identification` : All ***applicable*** identification of `title`.

+ `tag` : The name, or acronym, of the identification-standard.
+ `token` : The assigned identification-value.

`dateOfAccess` : The date (yyyy.mm.dd) `title` was accessed.

`question` : The focus of `answer`, and the seed of `definition` member(s).

`definition` : Define special-term(s) from `question`, from left-to-right.

+ `term` : The name of the concept being defined.
+ `hint` : Quoted, or paraphrased, version of the definition.
+ `source` : The entity that contributed to the definition.

`answer` : The solution based-on `question`, and the seed of `highlight` member(s).

`highlight` : Snippet(s) of the `title` that contributed to `answer`.

+ `section` : The index, as ***header.fullstop.comma***, of the snippet. 
+ `significant` : True or false, is the snippet crucial to getting the solution?
+ `content` : Quoted, or paraphrased, version the snippet.

## Uses

**When To Use:**

+ If using interactive-note formats (i.e. Cornell notes, Flashcards, etc.)
+ If note-sharing between large-groups, or over long-distances
+ If a machine-readable note-format is required
+ If revisiting notes is common-occurance

**When Not To Use:**

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