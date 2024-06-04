# Hugo Sphere Theme

This is a Hugo port of [Orbit](//github.com/xriley/Orbit-Theme) - great looking resume/CV template designed for developers by Xiaoying Riley.

It leverages Hugo's multilingual mode to allow you to manage multiple CV variants.
By using the "translation by file name" method your content files can life side-by-side.

Imagine you want to rephrase one of your experiences.
You can find the files for all variants and languages right next to each other.

```
.
├── content
│   ├── experiences
│   │   ├── employer1.de.md
│   │   ├── employer1.en.md

```

This should make it quite simple to apply changes across all variants and languages.

Additionally, the theme is optimized for print and ships prepared for `pagedjs` which helps you to export your CV as a PDF.

## Screenshot

![Sphere screenshot](/images/screenshot.jpg)

## Demo

TODO

You can see it in action on [Hugo Themes site](http://themes.gohugo.io/theme/hugo-sphere-theme/).

## Contents

- [Installation](#installation)
- [Getting started](#getting-started)
    - [Copying files](#copying-files)
    - [Configuring](#configuring)
    - [Test your site](#test-your-site)
    - [PDF export](#pdf-export)
- [License](#license)


## Installation

Grab the latest [`release`](//github.com/simne7/hugo-sphere-theme) and put it into the themes folder of your Hugo project.

For more information read the official [setup guide](//gohugo.io/overview/installing/) of Hugo.

## Getting started

After installing the theme successfully it requires just a few more steps to get your resume running.

### Copying files

Take a look inside the [`exampleSite`](//github.com/simne7/hugo-sphere-theme/tree/main/exampleSite) folder of this theme.
You'll find a file called [`config.toml`](//github.com/simne7/hugo-sphere-theme/blob/main/exampleSite/config.toml).
To start just copy the `config.toml` into the root folder of your Hugo site.

Or you copy the whole `exampleSite`, install the theme and adjust it to fit your curriculum vitae.

### Configuring

Open your just-copied `config.toml` and fill it with your data.
All other page content may be managed through dedicated content files.

For a detailed description of content management see the [documentation](//github.com/simne7/hugo-sphere-theme/blob/main/docs/index.md).

### Test your site

In order to see your site in action, run Hugo's built-in local server.

    $ hugo server -w

Now enter `localhost:1313` in the address bar of your browser.

### PDF export

Simply click the print icon in the top-right corner.
The print dialog of your browser will open.
Select the "Print to file" option and save it.


## License

The original template is released under the Creative Commons Attribution 3.0 License. Please keep the original attribution link when using for your own project. If you'd like to use the template without the attribution, you can check out other license options via template author's website: themes.3rdwavemedia.com

As for Hugo port you may rewrite the "Ported for..." line with setting your name at the end of `config.toml`

```toml
	[params.footer]
        copyright = "your name"
```

The port itself is released under the MIT license.


## Credits

- Xiaoying Riley - originally designed the theme [Orbit](//github.com/xriley/Orbit-Theme)
- Pavel Kanyshev - developed another Hugo port of the original theme [Hugo Orbit Theme]( https://github.com/aerohub/hugo-orbit-theme) which served as a nice inspiration for this theme
