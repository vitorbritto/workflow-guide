<p align="center">
<img src="https://github.com/vitorbritto/workflow-guide/raw/master/source/logo.jpg" alt="Workflow Guide" width="450">
</p>

> This is a work in progress and I will likely add (or replace) more functionality in the future.

# Introduction

Hello there! I'm Vitor Britto, a Full Stack Developer extremely passionate about my work. I discovered the world of code almost two decades ago and kept the same passion from the first moment of this discovery. I have worked full time as a freelancer for nearly 4 years developing projects for the web, and I focus part of my time on researchs, collaborative projects, personal projects and writing some articles for my blog.

But, enough about me! I would like to present you this project.


## What this is about?

1. My workflow context with approaches and methods that I use.
2. Tools that makes my Workflow easy.
3. My own code conventions, which is inspired by what is popular within the community and flavored with some personal opinions.
4. Major dependencies that I use.


## Why was it created?

**Reason #01**

Apply rules and be based on a principle and methodology of process which could maintain the structure of my standards.

**Reason #02**

Not only have a code style guide, but relevant informations about my Workflow. Thus I always keep the same logic process and can initiate the development of my projects without any questions when making a scaffolding, building process, automation rotines, unit testing and others tasks.

--------------------------------------------------------------------------------

# Table of Contents

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

- [Trello](https://trello.com/) - _Task Management for Old Projects only_
- [Google Drive](https://drive.google.com/) - _Share documents and files_
- [Wakatime](https://wakatime.com) - _Quantify my coding_
- [Skype](http://www.skype.com) - _Business Conferences and Chats_
- [Google Meet](https://meet.google.com/) - _Business Conferences and Chats_
- [Slack](https://slack.com/) - _Team Messaging_

**[⬆ back to top](#table-of-contents)**

## Blueprint and Visual

- [Adobe XD](https://www.adobe.com/br/products/xd.html) - _Prototyping and Wireframes_
- [Miro](https://miro.com) - _Online collaborative whiteboard_

**[⬆ back to top](#table-of-contents)**

## Development

### Scaffolding

Check the [Kickstarts](https://github.com/kickstarts/kickstarts) organization where I organize and setup my stacks for every kind of project. It's a initial structure and configuration where I can start coding in a few minutes.

### Coding

**Front-End:**

- HTML5
- CSS3
- JavaScript

**Back-End:**

- NodeJS
- PHP

**Database**

- MySQL
- PostgreSQL
- Redis
- MongoDB

### Editors

- [Visual Studio Code](https://code.visualstudio.com/) - _Code editing_
- MacVim

### Build

Frameworks   | Libraries | Template Engine | Supersets     | Others
------------ | --------- | --------------- | ------------- | -----------
React Native | React     | Pug             | Sass          | WordPress
Angular      | jQuery    | EJS             | PostCSS       | WooCommerce
Ionic        |           |                 | Typescript    | Strapi
AdonisJS     |           |                 |               | GraphQL
Gatsby       |           |                 |               | AWS
NextJS       |           |                 |               | Vercel
Express      |           |                 |               | 
Laravel      |           |                 |               |
Lumen        |           |                 |               |
Slim         |           |                 |               |

... [and much more](http://stackshare.io/vitorbritto/vb-web-studio)!


**[⬆ back to top](#table-of-contents)**

--------------------------------------------------------------------------------

# Guides

For web projects in which I work from planning to delivery, I use the guides below. If I am on a team that already has established guides, I'll follow the rules already adopted.already adopted. No bullshit, just follow the rules.

- [HTML](guides/html.md)
- [CSS](guides/css.md)
- JavaScript
  - [ES5](guides/es5.md) - *used in obsolete projects*
  - [ES6](guides/es6.md)
- [ReactJS](guides/reactjs.md)
- Angular - *work in progress*
- [NodeJS](guides/nodejs.md)
- [Git](guides/git.md)
- [Shell](guides/shell.md)

**[⬆ back to top](#table-of-contents)**

# General Notes

- **[STRATEGY]**: Kanban and/or [Scrum](http://scrummethodology.com/) method.
- **[DEVELOPMENT]**: use the [SOLID](http://en.wikipedia.org/wiki/SOLID_(object-oriented_design)) principles.
- **[BUILD]**: all javascript files must have two spaces (soft tab) and PHP files musta have four spaces (soft tab) FOR INDENTATION.

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
