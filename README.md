# TART - Tauri Application React Typescript

[](#table-of-contents)

## Table of Contents

1. [About TART](#about-tart 'Learn about TART')
2. [Find and Replace](#find-and-replace-these-values-in-the-entire-project 'How to do your intial setup of the project')
3. [Develop](#how-to-run-in-development-mode 'How to develop in hot-reload mode')
4. [Build local](#how-to-build-local 'How to build the application locally')
4. [Build cross-platform](#how-to-build-cross-platform 'The commands to build a target for a given OS')

[](#about-crate)

## About TART

TART is based on a simple idea: the import part of a tart is the filling.  You make the delicious filling and we'll handle the thing the filling goes into.

TART is an easy way to roll React and Typescript into a hot-reloadable Tauri application to speed up development.

### Prerequisites

You will need [VS Code](https://code.visualstudio.com/download) and [Node.js](https://nodejs.org/en/download/) installed.

[TOC](#table-of-contents 'Jump back to the Table of Contents')

[](#find-and-replace-these-values-in-the-entire-project)

## Find and replace these values in the entire project

To start your project, you should find and replace the following symbols project-wide in VS Code by hitting `crtl-shift-f` _(or `command-shift-f` on macOS)_:

1. `YOUR_GITHUB_USER` => your github username
2. `your-package-name` => your application's npm package name
3. `YOUR_PRODUCT_NAME` => your application's human-readable product name
4. `YOUR_APPLICATION_DESCRIPTON` => your application's human-readable short description
5. `YOUR_NAME` => your human name
6. `YOUR_EMAIL_ADDRESS` => your email address
7. `YOUR_COMPANY_NAME` => your company name
8. `YOUR_REPO_NAME` => your repository name
9. `YOUR_APPLICATION_UPDATER_PUBLIC_KEY` => your application's tauri updater public key

[TOC](#table-of-contents 'Jump back to the Table of Contents')

[](#how-to-run-in-development-mode)

## How to run in development mode

Then if you don't just want to stare at a spinning pastry icon on all 3 platforms you should probably start your project:

1. Run `npm install` to install your dependencies from npm
2. Run `yarn start` to start a hot-reloadable development server in a Tauri application
3. _(Optional, but probably a very good idea)_ Replace all instances of `latest` with actual version numbers in `package.json` to lock your dependency versions

[TOC](#table-of-contents 'Jump back to the Table of Contents')

## How to build for your OS

[](#how-to-build-local)

Run `yarn build` to build a binary compiled for your OS. It will be in the `src-tauri/target/release/bundle` directory.

[TOC](#table-of-contents 'Jump back to the Table of Contents')

## How to build cross platform

[](#how-to-build-cross-platform)

### GitHub Actions

By using the `tauri-actions` GitHub Actions, you can automatically build a distributable installer for all 3 desktop OSes.  This is the recommended way to build a distributable installer.  It's significantly easier than handling the build process manually from any random OS.  You can use the `tauri-actions` [GitHub Actions](https://github.com/tauri-apps/tauri-action) to easily build for linux, macOS, and Windows.  We have chosen not to include these files in the template because not everyone wants or needs to build cross-platform to all platforms, but more importantly because not everyone wants to use GitHub as their git hosting service.

[TOC](#table-of-contents 'Jump back to the Table of Contents')
