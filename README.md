# MyFlixAngularClient

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.3.5.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

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

## Description
The aim of this project is to  build the client-side for an application called myFlix using Angular based on its existing server-side code (REST API and database), with supporting documentation.

### User Stories
* As a user, I want to be able to receive information on movies, directors, and genres so that I can learn more about movies I’ve watched or am interested in.
* As a user, I want to be able to create a profile so I can save data about my favorite movies.

### Key Features
* Welcome view where users are able to either log in or register an account
* Upon authentication, display a view of all Movies
* Upon clicking on a particular movie, users will be taken to a single movie view, where
additional movie details will be displayed. The single movie view will contain the following additional features:
  * A button that when clicked takes a user to the ​director view,​ where details about the director of that particular movie will be displayed.
  * A button that when clicked takes a user to the ​genre view,​ where details about that particular genre of the movie will be displayed.


### What technology did I use and why?

I chose to create the application using **Angular** due to the following considerations:


### What challenges did I face, what did I learn?
TBD

## Development Process for the chat application
### Install Angular
1. Check if Angular is already installed on device
```bash
ng --version
```

2. If not, install Angular
```bash
npm install -g @angular/cli
```

### Create a new Angular project
1. Navigate to folder and create project
```bash
ng new my-project-name
```

2. Navigate to project folder to run project
```bash
ng serve --open
```

### Set up app to load data from movie API
1. Set up Angular HttpClient
  1.1. Go to app.module.ts and add
  ```bash
  import { HttpClientModule } from '@angular/common/http';
  ```

  1.2. Add HttpClientModule to the imports of @NgModule

2. Create Angular Service for Consuming REST API 
  2.1 Create a new Service inside app folder
  ```bash
  ng generate service fetch-api-data
  ```

  2.2. Add import statements to fetch-api-data.service.ts file
  ```bash
  import { catchError } from 'rxjs/internal/operators';
  import { HttpClient, HttpHeaders, HttpErrorResponse } from '@angular/common/http';
  import { Observable, throwError } from 'rxjs';
  import { map } from 'rxjs/operators';
  ```

3. Implement services logic to make API calls








