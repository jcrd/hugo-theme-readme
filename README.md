# hugo-theme-readme

*readme* is a readable, minimalistic [Hugo][hugo] theme for blogging. ([demo][demo])

See it in action [here][site].

[hugo]: https://gohugo.io/
[demo]: https://twiddlingbits.net/hugo-theme-readme/
[site]: https://twiddlingbits.net/

## Features

* Minimalistic appearance and footprint
* Tag and category taxonomy support
* Site logo in header
* Shortcodes:
  * Projects showcase
  * Gravatar avatar
* Analytics, supporting:
    * [goatcounter][goatcounter]

[goatcounter]: https://www.goatcounter.com/

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
text="This text is displayed to the right side of your avatar."
link="https://github.com/yourusername"
>}}
```
## License

This project is licensed under the MIT License (see [LICENSE](LICENSE)).

## Acknowledgements

* Icons provided by [heroicons][heroicons] ([LICENSE][heroicons-license]).

[heroicons]: https://heroicons.com/
[heroicons-license]: https://github.com/tailwindlabs/heroicons/blob/master/LICENSE
