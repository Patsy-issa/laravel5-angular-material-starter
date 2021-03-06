## Laravel 5.1 Angular Material Starter
> Version 2.3

<a href="https://infinite-dusk-3948.herokuapp.com/" target="_blank">View DEMO</a>

![Laravel & Angular](http://i.imgur.com/ZbLzOPP.jpg)  


##### Table of Contents  
[Overview](#overview)  
[Installation](#installation)  
[Issues, Questions and Feature Requests](#issues)  
[Planned features](#planned_features)  
[Changelog](#changelog)

<a name="overview"></a>
## OVERVIEW
This is a starter project that gives you an out of the box configuration Laravel 5.1 and AngularJS (folder by feature architecture).  
Here are the goodies that you'll get:

* Laravel 5.1
* Angular
* Angular Material
* [JSON Web Token authentication](https://scotch.io/tutorials/token-based-authentication-for-angularjs-and-laravel-apps)
* [Laravel5 Debug Bar](https://github.com/barryvdh/laravel-debugbar)
* [Angular UI router](https://github.com/angular-ui/ui-router) configuration with multiple views
* [Optimized deployment script](https://github.com/jadjoubran/laravel5-angular-material-starter/blob/master/deploy.sh)
* EditorConfig
* JavaScript Code Style (jscs)
* Jshint (rename _jshintrc to .jshintrc if you want to use it. Check [#11](https://github.com/jadjoubran/laravel5-angular-material-starter/issues/11))
* Less
* Elixir
* Angular Material sample code
* Angular Material custom theming
* Sample integration between Restangular & Laravel API endpoint


<a name="installation"></a>
## Installation

    composer create-project jadjoubran/laravel5-angular-material-starter --prefer-dist
    cd laravel5-angular-material-starter
    #fix database credentials in .env
    npm install -g gulp bower
    npm install
    bower install
    gulp && gulp watch
    php artisan serve
* You're ready to go! <a href="http://localhost:8000" target="_blank">http://localhost:8000</a>
* Star the repo and submit your feedback as a new issue or to <a href="https://twitter.com/joubranjad" target="_blank">@JoubranJad</a>
  
<a name="issues"></a>
## Issues, Questions and Feature Requests
Open a new issue, I'd love to help.
  
  
<a name="planned_features"></a>
## Planned features

- toast service + update documentation
- dialog service + update documentation
- redirect to unsupported browser page
- New demo pages: Rest API, loading bar, debugbar, filters
- Update to elixir 3.0 + use elixir.json
- fix gulp bower task
- continue heroku setup (database, migrations, seeding)
- make readme more appealing
- even better support for 5.1 (fork?)
- jwt auth example (with seed)
- artisan generators
- Add tooltips sample
- Speedup gulp watch
- Sample route authentication (via $localStorage)

  
  
<a name="changelog"></a>
## Changelog

### v2.3.1
+ removing development files using post-create-project-cmd
+ added `human_readable` angular filter

### v2.3.0
+ Simplified installation, now using `composer create-project`
+ fix issue with http over https


### v2.2.3
+ now using `artisan serve`
+ now using `artisan key:generate` instead of instructing the user to manually update it

### v2.2.2
+ new documentation page: Theme
+ new documentation page: Deploy
+ update documentation & readme cover

### v2.2.1
+ removed imagemin for now since it's not being used in elixir

### v2.2.0
+ New demo & documentation

### v2.1.2
+ Added [angular-loading-bar](https://github.com/chieffancypants/angular-loading-bar/) which works automatically

### v2.1.1
+ Added angularController to serve app (will be used later on for unsupported browser)

### v2.1.0
+ fixed documentation
+ fixed restangular config
+ added sample restangular API call
+ removed csrf token fix since we disabled CSRF when setting up JWT auth

### v2.0.1
+ fix mdtabs

### v2.0.0
+ Json Web Token authentication based on https://scotch.io/tutorials/token-based-authentication-for-angularjs-and-laravel-apps
+ New improved demo! Using heroku instead of github pages.

### v1.7.1
+ Installer script that installs all the required packages

### v1.7.0
+ removed UI router HTML5 mode because it breaks when refreshing and I don't want to mess up with the routes

### v1.6.1
+ UI-router HTML5 mode urls
+ updated documentation


### v1.6.0
+ added optimized deployment script: [deploy.sh](https://github.com/jadjoubran/laravel5-angular-material-starter/blob/master/deploy.sh)


### v1.5.1
+ jshint is now optional. Rename _jshintrc to .jshintrc. Check [issue #11](https://github.com/jadjoubran/laravel5-angular-material-starter/issues/11)


### v1.5.0
+ Add angular material icons
+ Add SVG-Morpheus for Angular Material Icons
+ Updated demo & gh-pages
+ Updated angular material
+ Add contributor covenant (code of conduct)


### v1.4.2
+ Elixir improvements for Laravel 5.1
+ Removed /resources/.tmp (not used anymore because of Elixir improvements)

### v1.4.1
+ Fixed laravel 5.1 migration issue

### v1.4.0
+ Laravel 5.1 Support
+ Remove CSRF token fix (angular automatically takes care of it http://laravel.com/docs/5.1/routing#csrf-x-xsrf-token)


### v1.3.1

+ Add sample Layout which relies on flexbox
+ Update Angular, Angular ui-router and Angular Material


### v1.3.0

+ Host demo on github pages
+ Add sample Laravel APIs and call them using Restangular


### v1.2.2

+ API response macro (to make API calls more compatible with Restangular)


### v1.2.1

+ Remove unused dependency in package.json
+ Material design custom theming


### v1.2.0

+ Add Angular Material boilerplate for Dashboard
+ Add sample UI Router conf that contains header and footer
+ Sample code for Tabs
+ Add Restangular
+ CSRF integration with Restangular
+ Add Laravel & Angular promo image (from [Laravel News](https://laravel-news.com))


### v1.1.1

+ Add Angular Material boilerplate for Landing
+ Sample code for Toast and Dialog
+ Disable Elixir success notifications
+ Add $localStorage (ngstorage) - will be used later on for sample authentication driver
+ Added basic ui-router for Landing


### v1.1.0

+ Remove Entrust & Repositories since they depend on each user's preference and can be easily installed


### v1.0.3

+ Fix Installation steps
+ Add Changelog
+ Plan future releases


### v1.0.2

+ Rename resources/views/index.php to resources/views/index.blade.php for the blade syntax to work (CSRF token) [PR 3](https://github.com/jadjoubran/laravel5-angular-material-starter/pull/3)


### v1.0.1

+ Remove `composer.lock` in order to pull the latest version of vendor dependencies [issue #1](https://github.com/jadjoubran/laravel5-angular-material-starter/issues/1)


### v1.0.0

+ Laravel5 installation
+ Basic Angular Support with Angular Material and UI Router
+ Laravel 5 debugbar, Entrust and Repositories
+ EditorConfig, jscs, jshint setup
+ Elixir setup