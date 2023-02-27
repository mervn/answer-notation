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
			"highlight" : "Sunlight reaches Earth's atmosphere and is scattered in all directions by all the gases and particles in the air",
			"modified" : "2023.02.25",
			"signature" : "Blue Skies",
			"affix" : "Chapter1:Sky",
			"authType" : "isbn-13",
			"authToken" : "978-0000000000"
		},
		{
			"highlight" : "Blue Skies are very nice",
			"modified" : "2023.02.27",
			"signature" : "Declaration Of Independence",
			"affix" : null,
			"authType" : null,
			"authToken" : null
		}
	]	
}
```

___

## Elements

`question` : The focus of `answer`, and the seed of `terminology` member(s).

`terminology` : Define special-term(s) from `question`, in left-to-right order.

+ `term` : The name of the concept being defined.
+ `definition` : Quoted, or paraphrased, version of the definition.
+ `source` : The data-table that contributed the definition.

`answer` : The solution based-on `question`, and the seed of `comment` member(s).

`comment` : Snippet(s) of information that contributed to `answer`.

+ `highlight` : Quoted, or paraphrased, version the snippet.
+ `modified` : The date (yyyy.mm.dd) `highlight` was last modified.
+ `signature` : Title, with edition-number, of `highlight` source.
+ `affix` : The location of `highlight` in `signature`, use **':'** to delimit sections.
+ `authType` :  The name, or acronym, of the identification-standard used to verify `signature`.
+ `authToken` : The value of `auth-type`, used to uniquely verify `signature`.


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
