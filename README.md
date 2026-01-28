# Leuzin

Leuzin is an Angular 7 application. It serves as a base project generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.3.5.

## Dependency Updates and Security

This project has been updated to address several security vulnerabilities identified by Dependabot and `npm audit`.

### Changes made:
- Updated direct dependencies to their latest compatible patch versions for Angular 7.
- Added `npm` overrides to force patched versions of transitive dependencies (e.g., `minimist`, `loader-utils`, `socket.io-parser`, `braces`, etc.).
- Replaced the incompatible `node-sass` with `sass` (Dart Sass) to support modern Node.js environments.
- Configured Karma and Protractor for headless Chrome execution to support automated testing environments.

### Remaining Vulnerabilities:
Some high-severity vulnerabilities remain in the core `@angular/*` packages. These cannot be fully resolved without a major upgrade to a newer version of the Angular framework (e.g., Angular 12 or higher), which would require significant code migrations and is currently out of scope.

## Deployment to GitHub Pages

The project is configured for deployment to GitHub Pages.

To deploy the application:
1. Ensure you have the necessary permissions to push to the repository.
2. Run the following command:
   ```bash
   npm run deploy
   ```
This command will build the project for production with the correct `base-href` (`/izoleuzin/`) and use `angular-cli-ghpages` to push the build artifacts to the `gh-pages` branch.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
