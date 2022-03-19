# TART - Tauri Application React Typescript

[](#table-of-contents)

## Table of Contents

1. [About TART](#about-tart 'Learn about TART')
2. [Find and Replace](#find-and-replace-these-values-in-the-entire-project 'How to do your intial setup of the project')
3. [Develop](#how-to-run-in-development-mode 'How to develop in hot-reload mode')
4. [Build Prerequisites](#prerequisites-to-build-some-distributable-installers 'What you need to target specific distribution chanels')
5. [Build for an OS](#how-to-build-distributable-installers-for-specific-platforms 'The commands to build a target for a given OS')
6. [Build for all OSes](#how-to-build-distributable-installers-for-all-platforms 'The commands to build a target for all 3 OSes')

[](#about-crate)

## About TART

TART is based on a simple idea: the import part of a tart is the filling.  You make the delicious filling and we'll handle the thing the filling goes into.

TART is an easy way to roll React and Typescript into a hot-reloadable Tauri application to speed up development.


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
8. `YOUR_APPLICATION_UPDATER_PUBLIC_KEY` => your application's tauri updater public key

[TOC](#table-of-contents 'Jump back to the Table of Contents')

[](#how-to-run-in-development-mode)

## How to run in development mode

Then if you don't just want to stare at a spinning box icon on all 3 platforms you should probably develop your project:

1. Run `npm install` to install your dependencies from npm
2. Run `yarn start` to start a hot-reloadable development server in a Tauri application
3. _(Optional, but probably a very good idea)_ Replace all instances of `latest` with actual version numbers in `package.json` to lock your dependency versions

[TOC](#table-of-contents 'Jump back to the Table of Contents')

[](#prerequisites-to-build-some-distributable-installers)

## How to build cross platform

[](#how-to-build-cross-platform)

### GitHub Actions

By using the `tauri-actions` GitHub Actions, you can automatically build a distributable installer for all 3 desktop OSes.  This is the recommended way to build a distributable installer.  It's significantly easier than handlign the build process manually from any given OS.  You can find the repo for the `tauri-actions` GitHub Actions [here](https://github.com/tauri-apps/tauri-action).  We have chosen not to include this in the core template because not everyone wants or needs to build cross-platform to all platforms, but more importantly because not everyone wants to use GitHub as their git hosting service.

[TOC](#table-of-contents 'Jump back to the Table of Contents')

[](#how-to-build-distributable-installers-for-all-platforms)

[TOC](#table-of-contents 'Jump back to the Table of Contents')