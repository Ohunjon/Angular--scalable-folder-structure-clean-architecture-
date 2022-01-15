# AngularScalableFolderStructure

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.2.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

## Folder Structure
   ## Core folder
   - The CoreModule is responsible for providing the application-wide and singleton services, interceptors or guards .... overal things which we use in app
   ## Shared folder 
  - SharedModule consists  reuseble (dump) components (uis)
   ## Feature folder
    Business logic. Contains modules, components, services, and other angular building blocks (if required) for a particular business feature.
  - Consists from features (app modules) - for example settings module (feature)  
     - services, pipes, directives created in this folder should use only for this module
    if we need for any base functionality - we can use from core 
    - components - dump components
    - contenier - smart components
    - classes folder consists from enums, interfaces, models which used only for this module
  ## templates folder 
 - Here we can declare like footer, header ui templates, (beacause of there are static ui templates not declared in shared) 
  ## Pages folder
  - Routed components with lazy loaded modules
  -Page controllers have no business logic. They are merely the presenter and orchestrates components from business feature modules.
  
