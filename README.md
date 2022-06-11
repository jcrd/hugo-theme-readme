# hugo-theme-readme

*readme* is a readable, minimalistic [Hugo][hugo] theme for blogging. ([demo][demo])

[hugo]: https://gohugo.io/
[demo]: https://twiddlingbits.net/hugo-theme-readme/

## Features

* Minimalistic appearance and footprint
* Tag and category taxonomy support
* Site logo in header
* Shortcodes:
  * Projects showcase
  * Gravatar avatar
  * Notices
* Analytics, supporting:
    * [goatcounter][goatcounter]

[goatcounter]: https://www.goatcounter.com/

## Configuration

This theme utilizes the following theme-specific configuration options:

* `commitURL` (*string*): URL for linking to commit of most recent change
* `highlight` (*boolean*): Whether to highlight code
* `projectsPhrase` (*string*): Phrase used to label `technologies` key in
  [projects showcase](#projects-showcase) shortcode
* `analytics`
    * `goatcounter` (*string*): Dashboard URL
* `logo`
    * `file` (*string*): Path to logo file
    * `width` (*integer*): Width of logo
    * `height` (*integer*): Height of logo
    * `title` (*boolean*): Whether to include the site title alongside logo
* `vanityFooter` (*boolean*): Whether to show vanity footer (hugo/theme info)
* `supportURL` (*string*): URL for linking to support/donation page

### Menu

This theme utilizes the [`main` menu][hugo-menu] with the following [params][hugo-menu-params]:

* `icon` (*boolean*): Whether to include an icon alongside name

  Supports these identifiers: `about`, `categories`, `tags`

[hugo-menu]: https://gohugo.io/content-management/menus/
[hugo-menu-params]: https://gohugo.io/content-management/menus/#params

## Shortcodes

### Projects showcase

Usage:
```
{{< projects >}}
```

This shortcode depends on a [data file][hugo-data] named `projects`.

For example, `projects.yml` would look like this:
```
- name: hugo-theme-readme
  description: This very blog theme
  url: https://github.com/jcrd/hugo-theme-readme
  technologies:
    - html
    - css
```

[hugo-data]: https://gohugo.io/templates/data-templates/

### Gravatar avatar

Usage:
```
{{< gravatar
email="youremail@domain.com"
link="https://github.com/yourusername"
>}}
This text is displayed to the right side of your avatar.
{{< /gravatar >}}
```

### Notices

Usage:
```
{{< notice label="Note" color="blue" >}}
Notice this notice.
{{< /notice >}}
```

The color parameter must be one of:
* gray
* red
* yellow
* green
* blue
* indigo
* purple
* pink

## License

This project is licensed under the MIT License (see [LICENSE](LICENSE)).

## Acknowledgements

Icons provided by:
  * [heroicons][heroicons] ([LICENSE][heroicons-license])
  * [bootstrap icons][bi] ([LICENSE][bi-license])

[heroicons]: https://heroicons.com/
[heroicons-license]: https://github.com/tailwindlabs/heroicons/blob/master/LICENSE
[bi]: https://icons.getbootstrap.com/
[bi-license]: https://github.com/twbs/icons/blob/main/LICENSE.md
