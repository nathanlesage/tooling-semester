# Contract

This contract's aim is to ensure that the resources made available in this repository follow the recommendations as outlined in the [Ljubljana OER Action Plan 2017](https://en.unesco.org/sites/default/files/ljubljana_oer_action_plan_2017.pdf). The reason for this is that due to this we ensure that these resources can -- ideally -- be used regardless of language, culture, gender, infrastructure, region, or other factors. We aim to strike a balance between feasability of creation and access of usage. Therefore, whereas several things are required (so that users can be sure they will find them in the course block), other things are optional (so that users may benefit even further from additional resources in the course block). If you have some technical knowledge, imagine this contract as a human-readable DOCTYPE/protocol specification.

## Introduction

Especially the Ljubljana OER Action Plan 2017 (hereafter: LAP) contains very specific recommendations that we aim to implment to the best of our abilities. According to the UNESCO, ensuring an equal and open access to educational resources aligns with [Goal 4 of the Sustainable Development Goals](https://sustainabledevelopment.un.org/sdg4), agreed upon 2015 in Paris, which should be fulfilled by 2030. The LAP identifies five key areas where improvements are necessary and possible. Among these, three key areas directly affect this repository and our enterprise, while two only affect governments and institutions.

This contract has been devised in order to participate in **capacity building** for OER (key area 1), making sure it aligns with the recommendations on **language and cultural awareness** (key area 2) and ensures **inclusive and equitable access** to OER (key area 3).

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](https://tools.ietf.org/html/rfc2119).

* **Must**: This is a requirement each course fulfills. This exists in every course block.
* **Should**: This is a recommendation, which means: If it exists for a course block, it contains valuable information or resources, but it might be missing for certain course blocks.
* **May**: This indicates that the described feature or document can be added, but its absence does not constitute a lesser value of the course.

## General Requirements for Course Blocks

Each course block that you will find in this repository has some general requirements that apply to every single block. Each block MUST be designed to take 90 minutes to teach. You MAY assign up to 30 minutes to general discussion, if the topic covered is easily covered in less time, but you MUST NOT design a course that is difficult to teach in 90 minutes. If the topic you cover is best taught in a full-day seminar/workshop you MUST split it up into self-contained 90 minutes blocks. You SHOULD indicate for each block that it belongs to a series and how much the learning quality may suffer if not all blocks of your series are taught by the user. Furthermore, each course MUST NOT cover more than one topic. We recognize that it is sometimes difficult to draw borders between different topics, but we urge you to think about what makes sense and what not. Each course block MUST be self-contained in a way that users can -- depending on whether it belongs to a series or not -- also choose to only take one single block of your series.

## Categories and naming of the course blocks

All course blocks MUST be assigned to one category. It MUST NOT belong to two categories. If you have doubts about the categorization, remember that categories can and will change, and feel free to suggest changes as soon as you devise a block that clearly fits either more than one or a non-existing category. You MUST choose a category that the _user_, not you as a contributor, will look at when the user tries to find your block. Therefore, please consult peers and learners for their opinion before assigning a category.

When requesting changes for the categorization, make sure to follow some basic rules. The category names -- new one and changes to existing -- MUST never exceed 5 words and MUST be in English. It MUST NOT contain any letters that may not work on certain file systems (such as forward-slashes and ampersands) to ensure everyone is able to download the course onto their computer for offline usage.

The name of each course block MUST follow the same rules as the category names, with one exception: You MAY but SHOULD NOT exceed 5 words for the name. The course block's name SHOULD be translated into as many languages as possible within the `README.md`-files, so this requirement only affects the folder name.

When translating material into courses, you MUST indicate the language using BCP-47 language tags (e.g. `en-US` or `jp-JP`). These language tags MUST be the last part of the name of the file or folder (for files: before the file extension), and it MUST be in the following format:

- Folder: `my-folder-name.en-US` or `my-folder-name.fr-FR`
- File: `README.jp-JP.md` or `README.fr-FR.md`

## Structure of the course blocks

Each category corresponds to a folder, and each course block MUST be contained by a folder that equals the name of the course block. Each course block consists of several files and folders.

Each course block MUST, on the top-level of the containing folder, contain a `README.md` which contains information that MUST be in English (see below for the requirements of the `README`-file). You SHOULD offer translations for your course materials. The `README.md` is the only file that MUST NOT include a language tag and MUST be in English. You SHOULD link translations of the `README.md` within the file for easy access for people who feel safer with different languages. The links SHOULD be in the language of the linked `README`-file (see below for requirements of the `README.md`).

## Requirements for `README.md`

While we do not want to give specific precedence to English, we recognize its global outreach and therefore its potential to strike a balance between ease of use and ease of access. Therefore, the `README.md` is the only file which MUST NOT include a language-indication. You SHOULD provide as many translations of the `README.md`, indicated with the corresponding language-tags, e.g. `README.fr-FR.md`. If your course is primarily aimed at a non-English speaking audience, you MAY keep the `README.md` to the bare minimum and extend the translation(s) of that file with more information. However, keep in mind that this will limit the outreach of your course for potential other users who do not speak your primary language.

Each `README.md` MUST on its first line contain a heading level 1 in ATX-style containing the course name. You MAY include special characters that are not possible in the course block folder name, such as colons or ampersands here, but the words MUST match the folder name. The translations in language-specific `README`-files, obviously, MUST differ in words, but not in meaning. Examples:

- Good: `A Course Block Introduction` --> `# A Course Block: Introduction`
- Bad: `A Course Block` --> `# A Course Block (some additional info)`

Immediately after the heading, the `README.md` MAY include the original author name, and contributors. But these are not necessary as they can also be listed in the `metadata.yml`-file.

After the heading and the optional author and contributor name(s), the `README.md` SHOULD contain a linked list of translations of the file in list-form. The link text SHOULD be in the language of the respective linked file. Example:

```markdown
# My Course Block Name

* [La README en français](./README.fr-FR.md)
* [Diese README auf Deutsch](./README.de-DE.md)

... additional content of the `README.md`-file
```

Afterwards you MUST include a blockquote (indicated by `>`) containing a concise English description of the anticipated goals of your course block. This should answer what problems your course poses, the preconditions of your course block, and what learners will be able to do after the session. You SHOULD indicate other course blocks that fulfill the corresponding requirements. Examples:

```markdown
> This course offers an introduction to Markdown for beginners. It is aimed at users of traditional Word processors and will enable learners to create documents using basic Markdown syntax.

> This course offers advanced Markdown elements for learners that enable them to create more sophisticated documents including several HTML elements to support the layout. Learners should already be familiar with basic Markdown syntax, as taught in, e.g., the block "Basic Markdown for Beginners."
```

The following requirements apply to your **main `README.md`-file**, which SHOULD be the English one, but which MAY also be one of the other files. The requirements SHOULD be met by all `README`-files, just as all `README`-files SHOULD be identical translations of each other.

Your main `README`-file MUST contain at least one link to each Markdown file that you provide and explain what the user may expect from the file. This does not include assets such as images used in your presentation. It furthermore does not include the required `slides.md` and `notes.md`-files.

It SHOULD provide an exhaustive explanation to the users of how they can use your block to teach their students. Your main `README`-file furthermore MUST indicate the licenses of provided materials so that users know exactly what they can do with the resources, and what not. You SHOULD NOT include non-free resources, but if you have to, you MUST have the written permission by their owner(s) that you are allowed to include the material into this course block and you MUST indicate that fact in a license block at the end that MUST be indicated by a heading level two "Licensing", e.g.: `## Licensing`.

## Requirements of the `metadata.yml` file

Your course block MAY contain a `metadata.yml` file which includes certain information in a machine-readable format, encouraging further spread of the materials by easy indexing of search engines. If you choose to include a `metadata.yml`-file, certain fields are required.

Such a file MUST contain a field `title` that includes the name of the course block and MUST correspond to the `README.md`-file. This file MUST also include the description from the `README.md`-file. furthermore, it MUST include a list of all authors and SHOULD include all collaborators. At least one person listed SHOULD provide an email address for users to pose questions to.

The file SHOULD also include a list of BCP-47-compatible language tags that then MUST correspond to all languages in which the material is sufficiently translated in order to be usable. If only the `README.md` is available in, e.g. French, but a required asset has not been translated into French yet, you MUST NOT include that language tag in this list.

You SHOULD also include the keys `requires` and `enables`, if your course block requires other blocks OR forms the basis of other blocks. This enables machines to reconstruct, e.g., sequential block series that can also be held as full-day seminars/workshops. You MUST include these courses by their fully qualified path (that is: `category/course name`).

Henceforth, a `metadata.yml` file could look like this:

```yaml
title: "My Course block: Introduction"
description: |
  This is the description that appears as such in the README.md file.
authors:
  - Name 1
  - Name 2 <optional@email.tld>
collaborators:
  - Name 1
  - Name 2
languages:
  - en-US
  - it
  - fr-FR
requires:
  - "Scientific Writing/Markdown Basics"
  - "Tools/Pandoc"
enables:
  - "Academic Writing/Collaborating with Git"
```

## Required assets for a course block

Each course block MUST include two required assets. That is first a file `slides.md`, translated in the main language. That means, if the course's main language is English, you MUST include a file `slides.en-US.md`. This file MUST include at least one slide that can be compiled into a valid HTML presentation format (e.g. reveal.js). If your course does not need slides, and you do not wish to create slides, you MUST at least provide a basic slide containing the course block name. Example:

```markdown
# My course block name
```

Furthermore, the course block folder MUST include the file `notes.md` (including the correct BCP-47-compatible language tag), which contains notes the user can refer to when teaching. This file can include more general or specific instructions on how to proceed. You can use this file to simply provide your own notes for the course, but you MUST make sure other users can follow them, that is, it MUST NOT include words or terms that only you know and which are not explained. Remember that courses MUST be self-contained, i.e. ALL necessary resources MUST reside in this folder.

Each course block is based upon required and optional assets. These can be further documents including information for teaching the course block, images, videos, etc. The required assets MUST be included in your folder, the optional assets SHOULD be included. You MAY only include links to (external) optional resources, but all required assets MUST be completely be provided with the folder. This way, the course can be taught offline.

Your course block MAY include one, multiple, or all of the following special folders:

- tasks
- assets
- img
- images
- resources
- videos

If you include tasks for your course that users can solve with their course, you MUST put them in the `tasks`-directory, and you MUST include one document per each task. You MUST NOT include multiple tasks in one document. You MAY name the task documents as you wish, but remember that each task MUST be linked in your main `README.md`.

You can use either one or more of the folders `assets`, `img`, `images`, `videos`, or `resources` to store assets in, but you MUST NOT use both `img` and `images` as these are aliases of each other. Furthermore, you MUST NOT store non-videos in the `videos`-folder and non-images in the `img` or `images`-folder. Each of these folders MAY include a `README.md` file, but it SHOULD NOT. If you decide to include such a file out of certain reasons, that file MUST be in English OR it MUST contain the corresponding language-tag in the filename.

If files or folders are not language-agnostic, their names MUST include the corresponding BCP-47 tags. Depending on the requirements of your course block, you may either include several, e.g., `assets`-folders, named with language tags (e.g. `assets.fr-FR`), or include the language tags within the files. So the following two alternatives are valid:

- `assets.fr-FR/my-image.png`
- `assets/my-image.fr-FR.png`

But you MUST NOT include both a generic `assets` folder with several language-tagged files and a language-tagged `assets`-folder at the same time.

## Optional assets for a course block

Each course block can have optional assets, upon whose existence you can decide based on the requirements of your course. But here are some examples.

Your course block MAY include converted `slides.md` into other formats (including PPTX or ODP) so that you may end up with the following variations of your `slides`:

- `slides.en-US.md`
- `slides.en-US.pptx`
- `slides.en-US.odp`
- `slides.it.md`
- `slides.it.odp`

If your course optionally suggests non-free resources you SHOULD link them in either your `slides`, `notes`, and/or `README` file(s). You MUST NOT include non-free formats in your folder. Furthermore, your course MUST NOT rely on non-free materials -- these may only be optional.
