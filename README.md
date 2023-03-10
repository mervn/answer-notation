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
	"question" : "Why is the sky blue?",
	"terminology" :
	[
		{
			"term" : "sky",
			"definition" : "the thing you see when you look up.",
			"source" : null
		},
		{
			"term" : "blue",
			"definition" : "portion of the color spectrum lying between green and violet.",
			"source" : "merriam-webster"
		}
	],
	"answer" : "Blue light is scattered more than the other colors because it travels as shorter, smaller waves.",
	"comment" :
	[
		{
			"what" : "Sunlight reaches Earth's atmosphere and is scattered in all directions by all the gases and particles in the air",
			"who" : "sky-is-beautiful",
			"where" : "chapter-1.properties-of-atmosphere",
			"when" : "2023.02.25",
			"why" : "isbn-13",
			"how" : "978-0000000000"
		},
		{
			"what" : "Blue skies smiling at me",
			"who" : "blue-skies",
			"where" : "0.12",
			"when" : "2023.02.27",
			"why" : "url",
			"how" : "https://www.youtube.com/watch?v=FXMaUnluj40"
		}
	],
	"group" : "notes-from-meteorology-class-1",
	"subgroup" :
	[
		{
			"tag" : "atmosphere",
			"hint" : "This scope of the sky dicussed"
		},
		{
			"tag" : "blue-color",
			"hint" : "This is a by-product of this process"
		},
		{
			"tag" : "light",
			"hint" : "Is interacted with to produce color"
		},
		{
			"tag" : "sky",
			"hint" : "The color of this is discussed"
		}
	]
}
```

> More examples can be found [here](docs/notes).

___

## Composition

`question` : The problem to be solved, and the seed of `terminology` member(s).

`terminology` : Special-term(s) from `question` defined, in left-to-right order.

+ `term` : The word, or phrase.
+ `definition` : Quoted, or paraphrased, version of `term` meaning.
+ `source` : Title of data-table that contained `definition`.

`answer` : The solution based-on `question`, and the seed of `comment` member(s).

`comment` : Snippet(s) of information that contributed to `answer`.

+ `what` : Quoted, or paraphrased, version of the snippet.
+ `who` : Title, with edition-number, of the work that contained `what`.
+ `where` : The location of `what` in `who`, with **'.'** used to narrow scope.
+ `when` : The date (yyyy.mm.dd) `what` was last modified.
+ `why` :  The name, or acronym, of the identification-standard used to verify `what`.
+ `how` : The actualized version of `why`, used to uniquely verify `what`.

`group` : The semantic-origin of the `question`, and the seed of `subgroup` member(s).

`subgroup` : Semantic-collection(s) the `question` is included in, excluding `group`.

+ `tag` : The word, or phrase, represented by the collection.
+ `hint` : The indication, used to validate `tag`.

## Uses

**When To Use:**

+ If using interactive notes (i.e. Cornell notes, Flashcards, etc.)
+ If note-sharing between large-groups, or over long-distances
+ If a machine-readable notation is required
+ If revisiting notes is common-occurance

**When Not To Use:**

+ If the note is short-lived (i.e. bookmarks, reminders, etc.)
+ If most fields of the notation cannot reasonably be given values
+ If the project, or group, is standardizing to another notation
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
