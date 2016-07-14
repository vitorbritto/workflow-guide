![Workflow Guide Logo](logo-wg.jpg "Workflow Guide")

> This is a work in progress and I will likely add (or replace) more functionality in the future.

# Introduction

Hello there! I'm Vitor Britto, a Full Stack Developer extremely passionate about my work. I discovered the world of code almost two decades ago and kept the same passion from the first day of this discovery. I have worked full time as a freelancer for nearly 4 years developing projects for the web, and I direct part of my time to researchs, collaborative projects, development of personal projects and writing some articles for my blog.

But enough about me! I would like to present this project and why it was created.

**First reason:**

Apply rules and be based on a principle and methodology of process which could maintain the structure of my standards.

**Second reason:**

Not only have a code style guide, but relevant informations about my Workflow. Thus I always keep the same logic process and can initiate the development of my projects without any questions when making a scaffolding, building process, automation rotines, unit testing and others tasks.

**This guide consists in four parts:** :ghost:

1. My workflow context with approaches and methods that I use.
2. Tools that makes my Workflow easy.
3. My own code conventions, which is inspired by what is popular within the community and flavored with some personal opinions.
4. Major dependencies that I use with ~~Grunt~~, Gulp, ~~Bower~~, JSPM, Karma and NodeJS/CLI.

> In the last projects, Grunt shows some unstable performance in my Wofklow. I'm not saying that grunt is worse than Gulp. No! Unfortunately, it doesn't fits on my workflow anymore.

> I've been working a lot with Isomorphic Applications using JavaScript both on client and server-side. Gulp, is programmatically closer to NodeJS. I love the pipe flow at Gulp. It reminds me the UNIX System :heart:.

# Table of Contents

- [Candidate Tools](#candidate-tools)
- [Workflow](#workflow)

  - [Strategy and Management](#strategy-and-management)
  - [Blueprint and Visual](#blueprint-and-visual)
  - [Development](#development)

    - [Scaffolding](#scaffolding)
    - [Building](#build)
    - [Coding](#coding)
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

--------------------------------------------------------------------------------

# Candidate Tools

## [Zapier](https://zapier.com)

The first tool in the list and a strong candidate to get into my workflow. So far, I'm comfortable with the free plan. I really like the way to trigger actions between apps.

## [Buddy](https://buddy.works)

Buddy is a powerful Git Hosting with Continuous Delivery tools. I create an account on the platform, but I have not tested yet.

## [Stamplay](https://stamplay.com)

With Stamplay I can chain together APIs as if they are Lego blocks arranging them into service based apps. If can automate tasks, connection some tools and triggering actions to build a data flow on Back-End. So, you can "create web applications without writing tons os backend codes".

## [Hotjar](https://www.hotjar.com/)

An amazing all-in-one tool for Analytics & Feedback. Hotjar combines 7 tools in one to deliver more user insight for less.

I started to use this tool about 1 month. You can understand what your website users do and don't do, and why. You cant track every action.

**[⬆ back to top](#table-of-contents)**

--------------------------------------------------------------------------------

# Workflow

> You can find a complete list of applications, utilities, DevOps and Business Tools here: [![Stack Share](http://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](http://stackshare.io/vitorbritto/vb-web-studio)

This is a simple table with approaches and methods that I use at my Workflow.

Strategy   | Blueprint   | Visual       | Develop     | Build       | Deploy
---------- | ----------- | ------------ | ----------- | ----------- | ----------
Research   | Sitemap     | Concepting   | Scaffolding | Lint        | Test
Observe    | Wireframe   | Presentation | Libraries   | Concatenate | Optimize
Understand | Prototype   | Refine       | Templates   | Minify      | **LAUNCH**
Analyze    | Style Guide | Approval     | Frameworks  | Compile     |
Timeline   | Usability   |              | Database    |

**[⬆ back to top](#table-of-contents)**

## Strategy and Management

- [Trello](https://trello.com/) - _Task Management_
- [Wunderlist](https://www.wunderlist.com/pt/) - _Daily Tasks_
- [On the Job](http://stuntsoftware.com/onthejob/) - _Track time and Expenses_
- [Forest](http://www.forestapp.cc/) - _Stay focused on tasks_
- [Google Drive](https://drive.google.com/) - _Share documents and files_
- [Dropbox](https://www.dropbox.com/) - _Share documents and files_
- [Wakatime](https://wakatime.com) - _Quantify my coding_
- [Skype](http://www.skype.com) - _Business Conferences and Chats_
- [Slack](https://slack.com/) - _Team Messaging_
- [Gitter](https://gitter.im/) - _Open Source Communications_

**[⬆ back to top](#table-of-contents)**

## Blueprint and Visual

- [Axure RP](http://www.axure.com/) - _Prototyping and Wireframes_
- [Sketch](https://www.sketchapp.com/) - _Professional digital design_
- [Photoshop](http://www.photoshop.com/products/photoshop)
- [Illustrator](http://www.adobe.com/products/illustrator)

**[⬆ back to top](#table-of-contents)**

## Development

### Scaffolding

The **Boilerplates** repository is my personal Yeoman. I organize and setup my stacks for every kind of project. It's a kick start structure and configuration. With this guy, I can start coding in a few minutes.

- [Boilerplates](https://github.com/vitorbritto/boilerplates)

### Building

Transpilers | Compilers | Frameworks | Libraries | Template Engine | CSS Supersets | Others
----------- | --------- | ---------- | --------- | --------------- | ------------- | -----------
Babel       | Electron  | AngularJS  | jQuery    | Pug             | Sass          | WordPress
TypeScript  | Cordova   | BackboneJS | ReactJS   | ERB             | Stylus        | WooCommerce
            |           | Ionic      |           | Haml            | PostCSS       | Sinatra
            |           | Express    |           | EJS             |               | Rack
            |           | Slim       |           |                 |               |
            |           | Laravel    |           |                 |               |

... [and much more](http://stackshare.io/vitorbritto/vb-web-studio)!

### Coding

**Front-End:**

- HTML5
- CSS3
- JavaScript

**Back-End:**

- NodeJS
- Ruby
- PHP

### Lint, Optimize and Style Checker

- [StyleLint](http://stylelint.io/)
- [SassLint](https://github.com/sasstools/sass-lint)
- [JSHint](http://jshint.com/)
- [ESLint](http://eslint.org/)
- [JSCS](http://jscs.info/)
- [Rubocop](http://batsov.com/rubocop/)
- [PHPfmt](http://www.cirello.org/php.tools/)
- [PHPCS](http://pear.php.net/package/PHP_CodeSniffer)

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

- [Karma](http://karma-runner.github.io/)
- [Mocha](https://github.com/visionmedia/mocha)
- [Jasmine](http://jasmine.github.io/)
- [Protactor](http://www.protractortest.org/)
- [PHPUnit](https://phpunit.de/)
- [RSpec](http://rspec.info/)

**REST/API**

- [Superagent](https://github.com/visionmedia/superagent)
- [Supertest](https://github.com/visionmedia/supertest)
- [Postman](https://www.getpostman.com/)
- [cURL](http://curl.haxx.se/)

**Cross-Devices/Browsers and Interfaces**

- [Browser Sync](http://browsersync.io/)
- [Capybara](https://jnicklas.github.io/capybara/)

**Performance**

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

**Mobile**

- [GenyMotion](https://www.genymotion.com/) - Android
- [XCode Simulator](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/iOS_Simulator_Guide/Introduction/Introduction.html) - iOS

**[⬆ back to top](#table-of-contents)**

## Automation

- [Just](http://vitorbritto.github.io/just/)
- [Makefy](http://vitorbritto.github.io/makefy/)
- [Grunt](http://gruntjs.com/)
- [Gulp](http://gulpjs.com/)
- [Rake](http://rake.rubyforge.org/doc/rakefile_rdoc.html)
- [Make](http://en.wikipedia.org/wiki/Make_(software))

**[⬆ back to top](#table-of-contents)**

## Modules (bundle/load/manage)

- [Bower](https://bower.io/) - _deprecated_
- [NPM](https://www.npmjs.org/)
- [JSPM](http://jspm.io/)
- [Webpack](https://webpack.github.io/)
- [Bundler](http://bundler.io/)
- [RubyGems](https://rubygems.org/)
- [Composer](https://getcomposer.org/)

**[⬆ back to top](#table-of-contents)**

## Database

- [MySQL WorkBench](https://www.mysql.com/products/workbench/)
- [Sequel Pro](http://www.sequelpro.com/)
- [Mongotron](http://mongotron.io)
- [CouchDB](http://couchdb.apache.org)
- [PSequel](http://www.psequel.com/)

**[⬆ back to top](#table-of-contents)**

## Documentation

- [RAML](http://raml.org/)
- [Blueprint](https://apiblueprint.org)
- [ESDoc](https://esdoc.org/)
- [JSDoc](http://usejsdoc.org/)
- [ngDoc](https://github.com/angular/angular.js/wiki/Writing-AngularJS-Documentation)
- [SassDoc](http://sassdoc.com/)
- [PHPDocumentor](http://www.phpdoc.org/)

**[⬆ back to top](#table-of-contents)**

## Deployment

- [Capistrano](http://capistranorb.com/) - _used for remote server automation too_
- [Surge.sh](https://surge.sh/)

**[⬆ back to top](#table-of-contents)**

## Versioning

- [Bitbucket](http://www.bitbucket.com/)
- [Github](http://github.com)

**[⬆ back to top](#table-of-contents)**

## PaaS

- [Heroku](https://www.heroku.com/)
- [OpenShift](https://www.openshift.com/)

**[⬆ back to top](#table-of-contents)**

## BaaS

- [Firebase](https://www.firebase.com)

**[⬆ back to top](#table-of-contents)**

## Continuous Integration and Code Coverage

- [Travis CI](https://travis-ci.org/)
- [Code Climate](https://codeclimate.com/)
- [CodeShip](https://codeship.com)
- [Coveralls](https://coveralls.io/)
- [Wercker](wercker.com)

**[⬆ back to top](#table-of-contents)**

## Post-Project / SEO

- [MailChimp](http://mailchimp.com)
- [Mandrill](https://www.mandrill.com/)
- Google AdWords
- Google Analytics

**[⬆ back to top](#table-of-contents)**

--------------------------------------------------------------------------------

# Guides

- [HTML](guides/html.md)
- [CSS](guides/css.md)
- JavaScript
  - [ES5](guies/es5.md)
  - [ES6](guies/es6.md)
- ReactJS - _work in progress_
- AngularJS
  - [ES5](guides/angularjs-es5.md)
  - [ES6](guides/angularjs-es6.md)
- [NodeJS](guides/nodejs.md)
- [Ruby](guides/ruby.md)
- [Git](guides/git.md)
- [Shell](guides/shell.md)

**[⬆ back to top](#table-of-contents)**

# General Notes

- **[STRATEGY]**: a mix of [GTD](http://pt.wikipedia.org/wiki/Getting_Things_Done) and [Scrum](http://scrummethodology.com/) methods.
- **[DEVELOPMENT]**: use the [SOLID](http://en.wikipedia.org/wiki/SOLID_(object-oriented_design)) principles.
- **[BUILD]**: all files must have two spaces (soft tab) for indentation.

**Be Consistent**

> The point of having style guidelines is to have a common vocabulary of coding so people can concentrate on what you're saying rather than on how you're saying it. We present global style rules here so people know the vocabulary, but local style is also important. If code you add to a file looks drastically different from the existing code around it, it throws readers out of their rhythm when they go to read it. Avoid this.

[Google C++ Style Guide](http://google-styleguide.googlecode.com/svn/trunk/cppguide.xml)

**[⬆ back to top](#table-of-contents)**

# References

- [Code Guide by @mdo](https://github.com/mdo/code-guide)
- [Airbnb CSS Style Guide](https://github.com/airbnb/css)
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- [John Papa Angular Style Guide](https://github.com/johnpapa/angular-styleguide)
- [Todd Motto Angular Style Guide](https://github.com/toddmotto/angular-styleguide)
- [Douglas Crockford's Code Conventions for JavaScript](http://javascript.crockford.com/code.html)
- [Felix Geisendörfer Node.js Style Guide](https://github.com/felixge/node-style-guide)
- [Airbnb Ruby Style Guide](https://github.com/airbnb/ruby)
- [Bozhidar Batsov Style Guide](https://github.com/bbatsov/ruby-style-guide)
- [Github Ruby Style Guide](https://github.com/styleguide/ruby)

**[⬆ back to top](#table-of-contents)**

# License

[MIT License](http://vitorbritto.mit-license.org/) © Vitor Britto
