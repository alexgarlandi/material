# Material Design for AngularJS Apps
[![npm version](https://badge.fury.io/js/angular-material.svg)](https://www.npmjs.com/package/angular-material)
[![Build Status](https://travis-ci.org/angular/material.svg)](https://travis-ci.org/angular/material)
[![Gitter](https://badges.gitter.im/angular/material2.svg)](https://gitter.im/angular/material?utm_source=badge&utm_medium=badge)

[Material Design](https://material.io/archive/guidelines/) is a specification for a
unified system of visual, motion, and interaction design that adapts across different devices. Our
goal is to deliver a lean, lightweight set of AngularJS-native UI elements that implement the
material design specification for use in AngularJS single-page applications (SPAs).

**AngularJS Material** is an implementation of Google's 
[Material Design Specification (2014-2017)](https://material.io/archive/guidelines/material-design/)
for [AngularJS](https://angularjs.org) developers.

For an implementation of the [Material Design Specification (2018+)](https://material.io/design/),
please see the [Angular Material](https://github.com/angular/components) project which is built for
[Angular](https://angular.io) developers.

### <a name="lts"></a> Long Term Support

AngularJS Material has entered a Long Term Support (LTS) period which ends on December 31st, 2021.
This date aligns with the
[AngularJS LTS](https://docs.angularjs.org/misc/version-support-status) period.

We now focus exclusively on providing fixes to bugs, in the 1.2.x branch of the library, that
satisfy at least one of the following criteria:
  - We receive a report of, or detect, a security weakness which is then verified
  - A major browser releases a version that will cause current production applications
    to stop working
  - The [jQuery library](https://jquery.com/) releases a version that will cause
    current production applications to stop working

AngularJS Material 1.1.x will get a new version, if and only if, we verify a new severe security
weakness.

Learn how to report security issues
[here](https://github.com/angular/material/blob/master/SECURITY.md).

![venn diagram](https://cloud.githubusercontent.com/assets/210413/5077572/30dfc2f0-6e6a-11e4-9723-07c918128f4f.png)

AngularJS Material includes a rich set of reusable, well-tested, and accessible UI components.

Quick Links:

*  [API & Demos](#demos)
*  [Contributing](#contributing)
*  [Building](#building)
*  [Installing](#installing)


Please note that using the latest version of AngularJS Material requires the use of
**[AngularJS](https://angularjs.org/) 1.7.2** or higher.

AngularJS Material supports the browser versions defined in the `browserslist` field
of our [package.json](package.json). Find out more on our
[docs site](https://material.angularjs.org/latest/#browser-support).

AngularJS Material supports the screen reader versions listed
[here](https://material.angularjs.org/latest/#screen-reader-support).

## <a name="demos"></a> Online Documentation and Demos

<div style="border: 1px solid #ccc">
  <img src="https://user-images.githubusercontent.com/3506071/93010488-11578980-f55b-11ea-9ea3-c4a7bffd20b9.png" style="display:block;">
</div><br>

- Visit [material.angularjs.org](https://material.angularjs.org/) online to review the API, see the
  components in action via live demos, and to read our detailed guides which include the layout system,
  theming system, typography, and more.
- Or you can build the documentation and demos locally; see
  [Build Docs & Demos](https://github.com/angular/material/tree/master/docs/README.md) for details.


## <a name="releasing"></a> Our Release Processes

To preserve stability with applications currently using AngularJS Material, we do not follow semver.
We have three types of releases:

*  `major` :  major releases will be done in the separate [Angular Material](https://github.com/angular/components) repo.
 This type of release will not be used within AngularJS Material.
*  `minor`:  contain breaking changes in addition to patch release changes.
*  `patch`:  non-breaking changes (no API, CSS, UX changes that will cause breaks in existing AngularJS Material applications).

##### Patch Releases

The patch builds (1.2.1, 1.2.2, etc.) are prepared based on commits in the `master` branch;
which contains only non-breaking changes (I.e. bug fixes, new features, API additions, and minimal
non-breaking CSS changes). We are targeting `patch` releases every 2 weeks.

##### Minor Releases

The minor builds (1.1.0, 1.2.0, 1.3.0) can contain breaking changes to CSS, APIs, and UX.
Our formal release of `minor` builds is much less frequent. The release process for `minor` builds is currently
being re-evaluated.

> For the purposes of AngularJS Material, you *could* think of the patch releases as being *minor* changes,
  and the 'minor' releases as being *major* changes according to semver.

## <a name="contributing"></a> Contributing

Developers interested in contributing should read the following guidelines:

- [Issue Guidelines](.github/CONTRIBUTING.md#submit)
- [Contributing Guidelines](.github/CONTRIBUTING.md)
- [Coding Guidelines](docs/guides/CODING.md)
- [Pull Request Guide](docs/guides/PULL_REQUESTS.md)
- [Software Process](docs/guides/COMMIT_LEVELS.md)
- [Change Log](CHANGELOG.md)

> Please do **not** ask general questions in an issue. Issues are only to report bugs, request
  enhancements, or request new features. For general questions and discussions, use the
  [AngularJS Material Forum](https://groups.google.com/forum/#!forum/ngmaterial).

It is important to note that for each release, the [ChangeLog](CHANGELOG.md) is a resource that will
itemize all:

- Bug Fixes
- New Enhancements
- Breaking Changes

## <a name="building"></a> Building

Developers can build AngularJS Material using NPM and gulp.

First install or update your local project's **npm** dependencies:

```bash
npm install
```

Install Gulp v3 globally:

```bash
npm install -g gulp@3
```

Then run the **gulp** tasks:

```bash
# To build `angular-material.js/.css` and `Theme` files in the `/dist` directory
gulp build

# To build the AngularJS Material Docs and Demos in `/dist/docs` directory
gulp docs
```

For development, use the `docs:watch` **NPM** script to run in dev mode:

```bash
# To build the AngularJS Material Source, Docs, and Demos in watch mode
npm run docs:watch
```

For more details on how the build process works and additional commands (available for testing and
debugging) developers should read the [Build Guide](docs/guides/BUILD.md).

## <a name="installing"></a> Installing Build (Distribution Files)

#### NPM

For developers not interested in building the AngularJS Material library... use **NPM** to install
and use the AngularJS Material distribution files.

Change to your project's root directory.

```bash
# To get the latest stable version, use NPM from the command line.
npm install angular-material --save

# To get the most recent, latest committed-to-master version use:
npm install http://github.com/angular/bower-material#master --save
```

#### Other Dependency Managers

Visit our [distribution repository](https://github.com/angular/bower-material/blob/master/README.md)
for more details on how to install and use the AngularJS Material distribution files within your local
project.

#### CDN

CDN versions of AngularJS Material are available.

With the Google CDN, you will not need to download local copies of the distribution files. Instead,
simply reference the CDN urls to easily use those remote library files. This is especially useful
when using online tools such as [CodePen](http://codepen.io/) or [Plunker](http://plnkr.co/).

```html
  <head>

    <!-- AngularJS Material CSS now available via Google CDN; version 1.2.1 used here -->
   <link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/angular_material/1.2.1/angular-material.min.css">

  </head>
  <body>

    <!-- AngularJS Material Dependencies -->
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular-animate.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular-aria.min.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular-messages.min.js"></script>

    <!-- AngularJS Material Javascript now available via Google CDN; version 1.2.1 used here -->
    <script src="https://ajax.googleapis.com/ajax/libs/angular_material/1.2.1/angular-material.min.js"></script>
  </body>
```

Developers seeking the latest, most-current build versions can use [GitCDN.xyz](https://gitcdn.xyz/) to
pull directly from our [distribution repository](https://github.com/angular/bower-material):

```html
  <head>

    <!-- AngularJS Material CSS using GitCDN to load directly from `bower-material/master` -->
    <link rel="stylesheet" href="https://gitcdn.xyz/cdn/angular/bower-material/master/angular-material.css">

  </head>
  <body>

    <!-- AngularJS Material Dependencies -->
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular-animate.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular-aria.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.0/angular-messages.min.js"></script>

    <!-- AngularJS Material Javascript using GitCDN to load directly from `bower-material/master` -->
    <script src="https://gitcdn.xyz/cdn/angular/bower-material/master/angular-material.js"></script>

  </body>
```

Once you have all the necessary assets installed, add `ngMaterial` and `ngMessages` as dependencies for your
app:

```javascript
angular.module('myApp', ['ngMaterial', 'ngMessages']);
```
