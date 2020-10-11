<p align="center">
    <img width=30% src="demo/static/favicon.svg">
</p>

# Monochrome Hugo Theme

Minimalistic blog theme for Hugo.

[See the documentation for more information](https://lkummer.github.io/Monochrome/).

## Development Guide

After cloning the project, install the required dependencies:

```s
$ yarn install
```

Quick summary of the development scripts:

- `build` - Build the Hugo theme, demo and documentation sites for production.
  Linting the sources in the process. Built artifacts are placed in the `dist`
  folder.
- `build:theme:debug` - Build the Hugo theme unminified with source maps.
- `dev` - Run the demo site development server.
- `dev:doc` - Run the documentation site development server.
- `lint` - Lint all files with ESLint, Stylelint and Prettier.
- `format` - Format all files with ESLint, Stylelint and Prettier.

The scripts can be invoked using `yarn run`:

```s
$ yarn run <script>
```

For example, if we want to build the theme we can use the `build` script:

```s
$ yarn run build
```
