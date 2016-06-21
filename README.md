![Workflow Guide Logo](logo-wg.jpg "Workflow Guide") [![Stack Share](http://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](http://stackshare.io/vitorbritto/vb-web-studio)

> This is a work in progress and I will likely add (or replace) more functionality in the future.


## Introduction

Hello there! I'm Vitor Britto, a Full Stack Developer extremely passionate about my work. I discovered the world of code almost two decades ago and kept the same passion from the first day of this discovery. I have worked full time as a freelancer for nearly 4 years developing projects for the web, and I direct part of my time to researchs, collaborative projects, development of personal projects and writing some articles for my blog.

But enough about me! I would like to present this project and why it was created.

**First reason:**

Apply rules and be based on a principle and methodology of process which could maintain the structure of my standards.

**Second reason:**

Not only have a code style guide, but relevant informations about my Workflow. Thus I always keep the same logic process and can initiate the development of my projects without any questions when making a scaffolding, building process, automation rotines, unit testing and others tasks.

**This guide consist with four parts:** :ghost:

1. My workflow context with approaches and methods that I use.
2. Tools that I use in my Workflow.
3. My own code conventions, which is inspired by what is popular within the community and flavored with some personal opinions.
4. Major dependencies that I use with Grunt, Gulp, Bower, Karma and Node/CLI.

## Table of Contents

- [Workflow](#workflow)
- [Tools](#tools)
    - [Strategy and Management](#strategy-and-management)
    - [Blueprint and Visual](#blueprint-and-visual)
    - [Scaffolding and Build](#scaffolding-and-build)
    - [Frameworks, Supersets and Transpilers](#frameworks-supersets-and-transpilers)
    - [Lint and Code Style Checker](#lint-optimize-and-style-checker)
    - [Debug and Inspection](#debug-and-inspection)
    - [Metrics and Performance](#metrics-and-performance)
    - [Tests](#tests)
    - [Automation](#automation)
    - [Package Managers](#package-managers)
    - [Database](#database)
    - [Documentation](#documentation)
    - [Deployment](#deployment)
    - [Versioning](#versioning)
    - [PaaS](#paas)
    - [BaaS](#baas)
    - [CI and Code Coverage](#ci-and-code-coverage)
    - [Post-project](#post-project)
- [Guides](#guides)
- [General Notes](#general-notes)
- [References](#references)


## Workflow

This is a simple table with aproaches and methods that I use at my Workflow.

| Strategy    | Blueprint      | Visual         | Develop     | Build         | Deploy     |
|-------------|----------------|----------------|-------------|---------------|------------|
| Research    | Sitemap        | Concepting     | Scaffolding | Lint          | Test       |
| Observe     | Wireframe      | Presentation   | Libraries   | Concatenate   | Optimize   |
| Understand  | Prototype      | Refine         | Templates   | Minify        | **LAUNCH** |
| Analyze     | Style Guide    | Approval       | Frameworks  | Compile       |            |
| Timeline    | Usability      |                | Database    |               |            |

**[⬆ back to top](#table-of-contents)**


## Tools

Following is the list of the main tools and resources that I use in my workflow.

### Strategy and Management

- [Trello](https://trello.com/) - _Task Management_
- [Evernote](https://evernote.com) - _Organize Thoughts_
- [Wunderlist](https://www.wunderlist.com/pt/) - _Daily Tasks_
- [On the Job](http://stuntsoftware.com/onthejob/) - _Track time and Expenses_
- [TicTac](https://github.com/vitorbritto/tictac) - _A kind of Pomodoro methodology_
- [Google Drive](https://drive.google.com/) - _Share documents and files_
- [Dropbox](https://www.dropbox.com/) - _Share documents and files_
- [Wakatime](https://wakatime.com) - _Quantify my coding_

**[⬆ back to top](#table-of-contents)**

### Communication

- [Skype](http://www.skype.com) - _Business Conferences and chats_
- [Slack](https://slack.com/) - _Internal Team Messaging_
- [Gitter](https://gitter.im/) - _Open Source Communications_

**[⬆ back to top](#table-of-contents)**

### Blueprint and Visual

- [Axure RP](http://www.axure.com/) - _Prototyping and Wireframes_
- [Sketch](https://www.sketchapp.com/) - _Professional digital design_
- [Photoshop](http://www.photoshop.com/products/photoshop)
- [Illustrator](http://www.adobe.com/products/illustrator)

**[⬆ back to top](#table-of-contents)**

### Scaffolding and Build

- [Boilerplates](https://github.com/vitorbritto/boilerplates)

**[⬆ back to top](#table-of-contents)**

### Frameworks, Supersets and Transpilers

#### Front-End

**HTML**
- Jade
- EJS

**CSS**
- Sass
- Stylus
- PostCSS (Rucksack, Autoprefixer and CSS Nano)

**JavaScript**
- AngularJS
- VueJS
- Babel

#### Back-End

**JavaScript**
- Express

**Ruby**
- Rails

**PHP**
- Laravel
- Slim

**[⬆ back to top](#table-of-contents)**

### Lint, Optimize and Style Checker

- [SassLint](https://github.com/sasstools/sass-lint)
- [CSSLint](https://github.com/CSSLint/csslint)
- [JSHint](http://jshint.com/)
- [ESLint](http://eslint.org/)
- [JSCS](http://jscs.info/)
- [Rubocop](http://batsov.com/rubocop/)
- [PHPfmt](http://www.cirello.org/php.tools/)

**[⬆ back to top](#table-of-contents)**

### Debug and Inspection

- [DevTools](https://developer.mozilla.org/en-US/docs/Tools)
- [JSFiddle](http://jsfiddle.net/)
- [Plunker](https://plnkr.co)

**[⬆ back to top](#table-of-contents)**

### Metrics and Performance

- [JSPerf](http://jsperf.com/)
- [Page Speed](https://developers.google.com/speed/pagespeed/insights/)

**[⬆ back to top](#table-of-contents)**

### Tests

**Unit**
- [Mocha](https://github.com/visionmedia/mocha)
- [Chai](http://chaijs.com/)
- [PHPUnit](https://phpunit.de/)
- [RSpec](http://rspec.info/)

**REST/API**
- [Superagent](https://github.com/visionmedia/superagent)
- [Supertest](https://github.com/visionmedia/supertest)
- [Postman](https://www.getpostman.com/)
- [cURL](http://curl.haxx.se/)

**Cross-Devices/Browsers and Interfaces**
- [Browser-sync](http://browsersync.io/)
- [Capybara](https://jnicklas.github.io/capybara/)

**Performance**
- [JSPerf](http://jsperf.com/)
- [OpenBeat](opbeat.com)
- [New Relic](newrelic.com)

**Load/Stress**
- [Gremlins](https://github.com/marmelab/gremlins.js)

**Integration**
- [Pioneer](http://pioneerjs.com/)

**E2E**
- [DalekJS](http://dalekjs.com/)

**Regression**
- [BackToStopJS](https://garris.github.io/BackstopJS/)

**[⬆ back to top](#table-of-contents)**

### Automation

- [Just](http://vitorbritto.github.io/just/)
- [Makefy](http://vitorbritto.github.io/makefy/)
- [Gulp](http://gulpjs.com/)
- [Rake](http://rake.rubyforge.org/doc/rakefile_rdoc.html)
- [Make](http://en.wikipedia.org/wiki/Make_(software))

**[⬆ back to top](#table-of-contents)**

### Package Managers

- [Bower](https://bower.io/)
- [NPM](https://www.npmjs.org/)
- [JSPM](http://jspm.io/)
- [Bundler](http://bundler.io/)
- [RubyGems](https://rubygems.org/)
- [Composer](https://getcomposer.org/)

**[⬆ back to top](#table-of-contents)**

### Database

- [MySQL WorkBench](https://www.mysql.com/products/workbench/)
- [Sequel Pro](http://www.sequelpro.com/)
- [Robomongo](http://robomongo.org/)
- [CouchDB](http://couchdb.apache.org/#download)
- [PSequel](http://www.psequel.com/)

**[⬆ back to top](#table-of-contents)**

### Documentation

- [RAML](http://raml.org/)
- [api Blueprint](https://apiblueprint.org)
- [ESDoc](https://esdoc.org/)
- [JSDoc](http://usejsdoc.org/)
- [ngDoc](https://github.com/angular/angular.js/wiki/Writing-AngularJS-Documentation)
- [SassDoc](http://sassdoc.com/)
- [PHPDocumentor](http://www.phpdoc.org/)

**[⬆ back to top](#table-of-contents)**

### Deployment

- [Capistrano](http://capistranorb.com/) - _used for remote server automation too_
- [Surge.sh](https://surge.sh/)

**[⬆ back to top](#table-of-contents)**

### Versioning

- [Bitbucket](http://www.bitbucket.com/)
- [Github](http://github.com)

**[⬆ back to top](#table-of-contents)**

### PaaS

- [Heroku](https://www.heroku.com/)
- [OpenShift](https://www.openshift.com/)

**[⬆ back to top](#table-of-contents)**

### BaaS

- [Firebase](https://www.firebase.com)

**[⬆ back to top](#table-of-contents)**

### CI and Code Coverage

- [Travis CI](https://travis-ci.org/)
- [Code Climate](https://codeclimate.com/)
- [CodeShip](https://codeship.com)
- [Coveralls](https://coveralls.io/)
- [Wercker](wercker.com)

**[⬆ back to top](#table-of-contents)**

### Post-Project / SEO

- [MailChimp](http://mailchimp.com)
- [Mandrill](https://www.mandrill.com/)
- [Google AdWords Editor]()
- [Google Analytics]()

**[⬆ back to top](#table-of-contents)**


## Guides

- [HTML](guides/html.md)
- [CSS](guides/css.md)
- [JavaScript](guides/javascript.md)
- [AngularJS](https://github.com/johnpapa/angular-styleguide/blob/master/a1/README.md)
- [NodeJS](guides/nodejs.md)
- [Ruby](guides/ruby.md)
- [Rails](guides/rails.md)
- [Git](guides/git.md)
- [Shell](guides/shell.md)

**[⬆ back to top](#table-of-contents)**


## General Notes

- **[STRATEGY]**: use the [GTD](http://pt.wikipedia.org/wiki/Getting_Things_Done) and [Scrum](http://scrummethodology.com/) methods.
- **[DEVELOPMENT]**: use the [SOLID](http://en.wikipedia.org/wiki/SOLID_(object-oriented_design)) principles.
- **[BUILD]**: these files has two spaces for indentation: `*.styl`, `*.jade`, `*.sass`, `*.haml`, `*.rb`, `*.json`.

**Be Consistent**

> The point of having style guidelines is to have a common vocabulary of coding
> so people can concentrate on what you're saying rather than on how you're
> saying it. We present global style rules here so people know the vocabulary,
> but local style is also important. If code you add to a file looks
> drastically different from the existing code around it, it throws readers out
> of their rhythm when they go to read it. Avoid this.

[Google C++ Style Guide](http://google-styleguide.googlecode.com/svn/trunk/cppguide.xml)

**[⬆ back to top](#table-of-contents)**


## References

- [Code Guide by @mdo](https://github.com/mdo/code-guide)
- [idiomatic CSS](https://github.com/necolas/idiomatic-css/)
- [idiomatic.js](https://github.com/rwldrn/idiomatic.js/)
- [jQuery JavaScript Style Guide](http://contribute.jquery.org/style-guide/js/)
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- [Google JavaScript Style Guide](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)
- [jQuery Core Style Guidelines](http://docs.jquery.com/JQuery_Core_Style_Guidelines)
- [Annotated ECMAScript 5.1](http://es5.github.com/)
- [Douglas Crockford's Code Conventions for JavaScript](http://javascript.crockford.com/code.html)
- [Principles of Writing Consistent, Idiomatic JavaScript](https://github.com/rwldrn/idiomatic.js/)
- [Naming this in nested functions](https://gist.github.com/4135065) - Christian Johansen
- [Conditional Callbacks](https://github.com/airbnb/javascript/issues/52)
- [Popular JavaScript Coding Conventions on Github](http://sideeffect.kr/popularconvention/#javascript)
- [Understanding JavaScript Closures](http://javascriptweblog.wordpress.com/2010/10/25/understanding-javascript-closures/) - Angus Croll
- [Basic JavaScript for the impatient programmer](http://www.2ality.com/2013/06/basic-javascript.html) - Dr. Axel Rauschmayer
- [You Might Not Need jQuery](http://youmightnotneedjquery.com/) - Zack Bloom & Adam Schwartz
- [ES6 Features](https://github.com/lukehoban/es6features) - Luke Hoban
- [Airbnb Ruby Style Guide](https://github.com/airbnb/ruby)
- [Bozhidar Batsov Style Guide](https://github.com/bbatsov/ruby-style-guide)
- [Github Ruby Style Guide](https://github.com/styleguide/ruby)
- [The Rails 3 Way](http://www.amazon.com/Rails-Way-Addison-Wesley-Professional-Ruby/dp/0321601661)
- [Ruby on Rails Guides](http://guides.rubyonrails.org/)
- [The RSpec Book](http://pragprog.com/book/achbd/the-rspec-book)
- [Everyday Rails Testing with RSpec](https://leanpub.com/everydayrailsrspec)

**[⬆ back to top](#table-of-contents)**


## License

[MIT License](http://vitorbritto.mit-license.org/) © Vitor Britto
