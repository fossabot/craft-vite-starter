<img alt="craft-vite" src="header.png"/>
<br />
<div align="center">
<a href="https://packagist.org/packages/smonist/craft-vite-starter" target="_blank">
    <img src="https://badgen.net/packagist/name/smonist/craft-vite-starter" alt="Packagist Package Name" /></a>
</div>
<br />
<div align="center"><strong>Craft CMS 4 infused with Vite, TypeScript and WindiCSS.</strong></div>
<div align="center">Lightning fast development, HMR and a production ready build process 🍃</div>

<br />
<div align="center">
  <sub>Made by</sub><br />
  <sub><a href="https://twitter.com/smonist">Simon Wesp</a></sub><br />
  <sub><a href="https://twitter.com/thomasbendl">Thomas Bendl</a></sub>  
</div>

<br />

## Turbostart 🚀
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsmonist%2Fcraft-vite-starter.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsmonist%2Fcraft-vite-starter?ref=badge_shield)


```sh
bash <(curl -s https://raw.githubusercontent.com/smonist/craft-vite-starter/main/init.sh)
```

## Quickstart

1.  `mkdir my-project && cd my-project`
2.  `ddev config --project-type=craftcms --docroot=web --create-docroot`
3.  `ddev composer create -y smonist/craft-vite-starter`
4.  `make install`
5.  `make dev`

## Tech Stack

- [🔥 **Craft CMS 4**](https://github.com/craftcms/cms)
- [🚢 **DDEV**](https://github.com/drud/ddev)
- [📦 **Vite**](https://github.com/vitejs/vite)
- [🔒 **TypeScript**](https://github.com/microsoft/TypeScript)
- [💨 **WindiCSS**](https://github.com/windicss/windicss)

## Requirements

- DDEV
- Unix-based OS (MacOS, Linux)

### If you are on Windows

Use WSL2 and follow the instructions for Unix-based OS. [DDEV Documentation](https://ddev.readthedocs.io/en/latest/users/install/docker-installation/) is a great starting point.

## Commands

- `make install` - patches the DDEV craft config and installs Craft CMS. Should only be used as a first time setup.
- `make dev` - starts the development server
- `make build` - bundles the assets for production

## Subsequent Use

- `ddev yarn` - for managing frontend packages
- `ddev composer` - for managing backend packages
- `ddev craft` - exposes the [Craft CLI](https://ddev.readthedocs.io/en/latest/users/usage/commands/#craft)

### Critical CSS

To use Critical CSS, you need to manually add the pages that should be pre-rendered to the `criticalPages` array in `vite.config.ts`. The pages will be pre-rendered when building and the generated CSS will be inlined in the HTML.

## The team behind the magic ✨ 🪄 🦄

- https://github.com/smonist
- https://github.com/thomasbendl

## Credits

This repository is based on the official [Craft CMS 4 starter template](https://github.com/craftcms/craft).  
Thanks to Andrew Welch for the great [craft-vite plugin](https://github.com/nystudio107/craft-vite)!


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsmonist%2Fcraft-vite-starter.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsmonist%2Fcraft-vite-starter?ref=badge_large)