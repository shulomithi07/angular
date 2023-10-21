Angular is a Javascript framework which allows you to create reactive Single-Page-Applications (SPA's)
How is single page actually happening?
Javascript changes the dom during the run time and everything seems to happen in single page.
Internally in the same html file the content is changed.

# Angular vs Angular 2 vs Latest Angular Version

AngularJS -> This was the first angular version and angular team understood that this is not future proof So they decided to change it

Angular 2 -> Then came the Angular 2 The team has completely re-written the code changed alot of things this is completely different from Angular JS

From then on multiple versions came into picture the team has skipped Angular 3 due to some internal reasons.
Curretly Angular 14 is the latest version.
Angular releases a new version every 6 months
These releases are not very major in terms of the code you write it is only for the enhancement of the framework.
It is pretty stable.

# Installation

- First download the latest version of NodeJs in your system
- Later install npm globally on your system 
- `npm install -g npm`  (If on mac/linux use sudo before the command)
- If angular was previously installed then uninstall it globally
- `npm uninstall -g angular-cli @angular/cli`  (If on mac/linux use sudo before the command)
- Then verify npm cache (This will show the contents of the cache folder and if any unneeded data is there)
- `npm cache verify` (If on mac/linux use sudo before the command)
- If unneeded data is there then you can do `npm cache clean --force` (this will delete the entire cache) (This is not compulsory step depends on your system cache)
- Then install angular latest version
- `npm install -g @angular/cli@latest`  (If on mac/linux use sudo before the command)


# New Project Creation
- A project can simply be created with a simple command
- `ng new projectName (If on mac/linux use sudo before command)`
- To start the project after it is created
- `ng serve command can be used`
- For other commands checkout scripts key [package.json](../firstProject/package.json)


# Came across something called as ngModel and single interpolation
- `string interpolation`: It is like getting data from typescript we use {{variable}} The variable should be declared in typescript already to be used in html.
- `ngModel`: It is two way binding so the data can be updated from the html to typescript and from typescript to html directly it can be written like this `<input type="text" [(ngModel)]="title">` and the title variable should be declared in typescript.
    To visualize the change we can use string interpolation on a p tag like this
- `<p>{{title}}</p>`


## Structure
- The Basics
- Components & DataBinding
- Directives
- Services & Dependency Injection
- Routing
- Observables
- Forms
- Pipes
- Http
- Authentication
- Optimizations & NgModules
- Deployment
- Animation & Testing