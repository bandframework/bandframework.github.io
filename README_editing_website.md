# Instructions for the BAND Framework website

The website is powered by Jekyll, with all of the content in text files, which are in subdirectories in the bandframework.github.io respository of the bandframework organization. The website is [https://github.com/bandframework/bandframework.github.io](https://github.com/bandframework/bandframework.github.io). 

Note that you can make edits directly on the files in your web browser from the github repository. Just go to the link above, find the file you want to edit, and click on it. You'll see the file contents and a row of icons just above it. Click on the edit icon (looks something like a pencil, just to the left of the trashcan icon). Make your edits, then scroll down to the "Commit Changes" section. Put in a description of what changes you made and press `Commit changes` (or `Cancel` to back out). That's it!

If you want to preview changes locally, see guides such as [Testing your GitHub Pages site locally with Jekyll](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll).

If, after your changes have been made to the respository, you received an email that there was an error in the Jekyll processing that you cannot fix (e.g., you don't understand it), please forward the email to Dick (furnstahl.1@osu.ed).

## General instructions for editing YAML files (which end in `.yml`) 

1. News, Team, and Publications entries are specified in YAML files.
1. YAML stands for "YAML Ain't Markup Language" (it is actually a serialization language, not a markup language, hence the name). 
1. A quick overview of YAML syntax is given [here](https://idratherbewriting.com/documentation-theme-jekyll/mydoc_yaml_tutorial#:~:text=YAML%20is%20a%20format%20that,uses%20of%20YAML%20with%20Jekyll.), but all you really need to know is given in this README.
1. Key points:
    * Indentation matters: use previous entries as a template for your new entry. Do not use tabs.
    * For each new level you indent exactly two spaces. If you use incorrect spacing then the entire file will fail, even if off by just a space.
    * For text that runs over one line you can use `>` after the keyword and then as many lines with linebreaks as you want. But they must be indented. (Note: you can also use `|`.)
    * A new item in a list (e.g., a new team member) starts with a hyphen: `-`.
    * Most of the entries are key-value pairs, which are separated by a colon. E.g., `photo: phillips_cropped.jpg` or `date: July 1, 2020`. The order in which you put the key-value pairs doesn't matter, but for consistency and readability, please follow the order used by the other examples.
    * Do not use Word to edit the files or any other word processor that inserts control sequences.

## Adding or editing News items

1. Open the file `_data/news.yml` in an editor.
1. Start a new item with `- date: September 20, 2020` (using the relevant date!). Note the hyphen starting from the left margin, then one space to `date:`. 
1. Next is `headline: >`, which is indented two spaces.
1. Then just fill in the text, indenting each subsequent line (how much doesn't matter).
1. You can use html markup to put in links (follow the example of other entries).

## Adding or editing Team members

1. Open the appropriate file in `_data` in an editor. Senior investigators are in `team_members.yml`, postdocs are in `postdocs.yml`, graduate students are in `students.yml`, the Band Leader is in `band_leader.yml`.
1. Start a new item with `- name: Ulrich Heinz` (using the relevant name!). Note the hyphen starting from the left margin, then one space to `name:`. 
1. Put the image filename after `  photo:` and the file itself in `images/teampic`. 
1. Fill in the title/affiliation information after `  info:`, using `<br>` to force linebreaks.
1. You can omit the `bio: >` entry, but if you put it in, indent each subsequent line.
1. Don't worry about `number_educ: 0` and `education1:` for now; these are used to put in bulleted entries that might be added later.
1. You can use html markup to put in links (follow the example of other entries).

## Adding or editing Publications

1. Open the file `_data/publist.yml` in an editor.
1. Start a new item with `- title: "Efficient emulators for scattering using eigenvector continuation"` (using the relevant title!). Note the hyphen starting from the left margin, then one space to `title:`. 
1. Put the image filename after `  image:` and the file itself in `images/pubpic`. 
1. Fill in a short abstract/description after `  description: >`.
1. Include the authors after `authors:` using the style of other entries.
1. For the link to the publication itself, use `link:` followed by the `url:` and `display:` entries, which are each indented by two spaces relative to `link:`. See the other entries for examples.
1. If you want the publication to be a highlight, use `highlight: 1`, otherwise use `highlight: 0`. 
1. Ignore `news2:` for now.
1. You can use html markup to put in links (follow the example of other entries).

