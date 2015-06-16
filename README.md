## bxSlider 5.0.0 Beta

Feature Rich [jQuery](http://jquery.com/) plugin that lets you create touch enabled sliders. 

### Please understand that this project is still in beta. 

The current status of the milestones can be found [here](https://github.com/Tidal-Wave/bxSlider/milestones). 

If you want to use the [latest development](https://github.com/Tidal-Wave/bxSlider/archive/develop.zip) version, see the [building](#building) below.

## Quick start

#### Step 1 - Download

Start by downloading the [latest release](https://github.com/Tidal-Wave/bxSlider) of bxSlider. There are two prefered methods of download:

###### Git
```bash
git clone git@github.com:Tidal-Wave/bxSlider.git
```

###### Bower
```bash
bower install bxslider
```

#### Step 2 - Setup

Once you have downloaded bxSlider, put the required stylesheet in the head of your markup:

```html
<link rel="stylesheet" href="bxSlider/bxslider.min.css" />
```

Then, put the main javascript file at the bottom, right after jQuery:

```html
<script src="jquery.min.js"></script>
<script src="bxSlider/bxslider.min.js"></script>
```

You can use any element, such as `li`, `img`, `a`, `div`,or `span`,  for you slides. Wrap your slider elements with a container, such as a `div,` or `ul` element.

```html
<div class="bxslider">
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
  <div> Your Content </div>
</div>
```

#### Step 3 - Initialize

Call the [plugin](http://learn.jquery.com/plugins/) function and your slider is ready.

```javascript
$(document).ready(function(){
  $('.bxslider').bxSlider();
});
```

## Documentation

The slider documentation is included in this repo, and is built with [Assemble](http://assemble.io/). It is also publicly available at http://bxslider.tidalwaveagency.com.

## Building

This package uses [Grunt](http://gruntjs.com/) and [Bower](http://bower.io/) for its build process, which you will need to customize bxSlider or contribute to the project. The following tasks are available:

  * `default` compiles the CSS and JS for the plugin into `/dist` and builds the documentation.
  * `dist` compiles the CSS and JS for the plugin only into `/dist`.
  * `watch` watches all plugin and documentation source files, and builds them automatically whenever you save a change.
  * `test` runs all [JSHint](http://www.jshint.com/) and [QUnit](http://qunitjs.com/) tests headlessly using [PhantomJS](http://phantomjs.org/).

To customize bxSlider, define which plugins to build into the distribution by editing `/_config.json` to fit the needs of your build.

## Contributing

The gitub [issue tracker](https://github.com/Tidal-Wave/bxSlider/issues) is the preferred channel for bug reports, features requests, and submitting pull requests.

#####Please, do NOT use the issue tracker for personal support requests. Stack Overflow ([`bxslider`](http://stackoverflow.com/questions/tagged/bxslider)) is a much better place to get help, and will generally be a lot quicker too.

### Bug reports

A bug is a **demonstrable problem** that is caused by the code in the repository. Good bug reports are very helpful, but please be sure to follow these Guidelines when making bug reports:

  1. Use the GitHub issue search feature to check if the issue has already been reported.

  2. Check to see if the issue has been fixed by trying to reproduce it using the latest `develop` branch in the repository.

  3. Isolate the problem and create a reduced test case example. Please use a service such as [JSFiddle](http://jsfiddle.net/) or [JS Bin](http://jsbin.com/) for these cases.

  4. When reporting the error, please include the browser/OS in which it occurs. If applicable, include any steps required to reproduce the bug. Also include any lines of code that you have identified as the cause of the bug, any potential solutions, and your opinions on the merits of those solutions.

### Feature requests

Feature requests are welcome, but take a moment to find out whether your idea fits within the scope of the project. It's up to you to make a strong case concerning the merits of this feature request. Provide as much detail and context as possible for your request.

### Pull requests

A good pull request is a such a huge help. Please be sure they remain focused in scope, tidy, and don't contain any unrelated commits.

#####Important
**Please ask first** before embarking on any significant pull request (e.g. implementing features, refactoring code, porting to a different language), otherwise you risk spending a lot of time working on something that the project's developers might not want to merge into the project.

Adhering to the following process is the best way to get your work included in the project:

  1. [Fork](http://help.github.com/fork-a-repo/) the project, clone your fork, and configure the remotes:

    ```bash
    git clone https://github.com/<your-username>/bxSlider.git
    cd bxSlider
    git remote add upstream https://github.com/Tidal-Wave/bxSlider/bxSlider.git
    ```

  2. If you cloned the project a while ago, get the latest changes from upstream:

    ```bash
    git checkout develop
    git pull [--rebase] upstream develop
    ```

  3. Create a new topic branch (off the main project `develop` branch) to contain your feature, change, or fix:

    ```bash
    git checkout -b <topic-branch-name>
    ```

  4. Build the distribution before committing to ensure your changes follow the coding standards and all build files are up to date.

    ```bash
    grunt dist
    ```

  5. Commit your changes in logical chunks. Please adhere to these [guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html). Use Git's [interactive rebase](https://help.github.com/articles/interactive-rebase) feature to tidy up your commits before making them public.

  6. Locally merge (or rebase) the upstream development branch into your topic branch:

    ```bash
    git pull [--rebase] upstream develop
    ```

  7. Push your topic branch up to your fork:

    ```bash
    git push origin <topic-branch-name>
    ```

  8. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/) with a clear title and description against the `develop` branch.

**By submitting a patch, you agree to allow the project owner to
license your work under the terms of the [MIT License](LICENSE).**

## License

The code and the documentation are released under the [MIT License](LICENSE).