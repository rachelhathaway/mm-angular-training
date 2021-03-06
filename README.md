## Overview

These exercises are meant to accompany a beginner to intermediate level angularjs course.

## Prerequisites
- [git](http://git-scm.com/)
- [Vagrant](http://vagrantup.com/)
- python

## Get Started
- `git clone https://github.com/rachelhathaway/mm-angular-training.git`
- `cd mm-angular-training`
- `bower install`
- `python -m SimpleHTTPServer`

## Steps
Checkout a step with `git checkout xx` where `xx` is the step number.

### b.00 - Modules
1. Declare app, controllers, services, filters, and directives modules.

### b.01 - DI + simple routing and views
1. Add angular-route.js to the project. Inject it into the app.
2. Add the config() method to the main app.
3. Inject $locationProvider and $routeProvider into the config method.
4. Using $locationProvider, enable html5Mode.
5. Using $routeProvider, add your first route. Set the templateUrl to views/index.html.

### b.02 - Templates, scope, and data binding
1. In views/index.html, add the ng-model attribute to each text field
2. Update the string expression preceding each field to reference its field’s ng-model value
3. Change the heading text on form submission

### b.03 - Managing interactions with controllers
1. Add a new controller, AppCtrl, to controllers.js
2. Inject the controller module into the app module
3. Make your controller available to views/index.html
4. Modifying views/index.html, move the initialization of 'heading' to the controller
5. Move the expression from the form's ng-submit attribute to a function in the controller. Make sure the function is available to the template and is called on ng-submit.
6. Add a new controller, ClockCtrl
7. Using the $interval service, output the time to the view in hours:minutes:seconds format, updating every second

### b.04 - Filters
1. Convert a string into pig latin using a filter.

### b.05 - Directives 1
1. Given a .json file with a set of articles, create an article directive that outputs the title, body, author, and date of each article.
2. Your directive should have isolate scope and use templateUrl.

