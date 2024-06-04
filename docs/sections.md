**Table of Contents**

- [Profile](#profile)
    - [Contact](#contact)
    - [Education](#education)
    - [Languages](#languages)
    - [Interests](#interests)
- [Motivation / Cover letter](#motivation--cover-letter)
- [Summary](#summary)
- [Experiences](#experiences)
- [Skills](#skills)
- [Projects](#projects)

## Profile

Basic profile information is managed in `content/profile/_index.md`.

Frontmatter variables:

| Key       | Description                |
|-----------+----------------------------|
| `name`    | Your name                  |
| `tagline` | (Optional) Profile summary |
| `picture` | Filename for picture       |

Either put the referenced picture into the `profile` content folder or into the global `static` folder.
Pictures from the `profile` are automatically resized to fit 96x96 pixels while static images need to be manually edited (or they will be resized by the browser).

### Contact

Contact information is managed in `content/profile/contact.md`.

Frontmatter variables:

| Key      | Description                                |
|----------|--------------------------------------------|
| `icon`   | Put a MaterialDesignIcons icon name here.  |
| `title`  | This will become the visible contact item. |
| `url`    | (Optional) HTML `href` URL.                |

For `url` values `mailto:` and `tel:` links will work as expected.

If titles for some URL, like e.g. a LinkedIn URL do not wrap nicely consider inserting a space in the link title.

```toml
- icon: mdi-linkedin
  title: linkedin.com/in/ johndaviddoe # note the space before "john"!
  url: //linkedin.com/in/johndaviddoe
```

### Education

Information on your education is managed in `content/profile/education.md`.

You can specify the heading of the sidebar section by setting the `title` parameters.

The Frontmatter lists items for the `education` array:

| Key       | Description                                                 |
|-----------|-------------------------------------------------------------|
| `degree`  | Title for the education item, e.g. "B.Sc. computer science" |
| `college` | Where the education took place, e.g. "Oxford University"    |
| `dates`   | Timeframe when the education started/ended                  |

### Languages

You can specify the heading of the sidebar section by setting the `title` parameters.

You can add the languages you speak to `content/profile/languages.md`.

| Key     | Description          |
|---------|----------------------|
| `lang`  | Name of the language |
| `level` | Knowledge level      |

### Interests

You can specify the heading of the sidebar section by setting the `title` parameters.

Your hobbys etc. go into `content/profile/interests.md`.


## Motivation / Cover letter

Put your cover letter into `content/motivation.md`.

Frontmatter variables:

| Key          | Description                                         |
|--------------|-----------------------------------------------------|
| `location`   | You can put some location and date information here |
| `salutation` | Greeting                                            |

Content can contain Markdown.

## Summary

`content/summary.md` contains a summary of your career, skills and profile.

Frontmatter variables:

| Key     | Description                   |
|---------|-------------------------------|
| `title` | Text for the section heading  |
| `icon`  | MaterialDesignIcons icon name |

Content can contain Markdown.

## Experiences

You can list your career stages and professional background in `content/experiences`.

Use `content/experiences/_index.md` to edit the section title and icon.

| Key     | Description                   |
|---------|-------------------------------|
| `title` | Text for the section heading  |
| `icon`  | MaterialDesignIcons icon name |

Content of `content/experiences/_index.md` will be displayed right after the section heading.

Every other file should contain one career stage, e.g. `content/experiences/google.md`.

| Key        | Description                      |
|------------|----------------------------------|
| `weight`   | Used to sort your experiences    |
| `position` | Title of your role               |
| `dates`    | Start/end date of the employment |
| `company`  | Employer name                    |

Content can contain Markdown.

## Skills

You can visualize your skills through nice progress bars.
The data goes into `content/skills.md`.

| Key       | Description                   |
|-----------|-------------------------------|
| `title`   | Text for the section heading  |
| `icon`    | MaterialDesignIcons icon name |
| `skills`  | Array of skills               |

Each skill item has two params:

| Key       | Description |
|-----------|-------------|
| `skill`   | Skill name  |
| `level`   | Skill level |


## Projects

You can manage your private (non-business) projects in `content/projects`.

See [Experiences](#Experiences).

