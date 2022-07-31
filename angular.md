# Angular

Angular is a framework for building web applications with HTML and TypeScript.

## Runbook to create a new project

Prerequisite: You have installed angular with `npm install -g @angular/cli@latest`.

1. Navigate to the directory where you want to create the project.
2. Run `ng new <project-name> --no-strict`
3. CD into the new directory.
4. Run `ng serve` to start the project.
5. Open a browser and navigate to `http://localhost:4200` to see the landing page.
6. To add Bootstrap run `npm install --save bootstrap@3` in the root directory. Note: the @3 after bootstrap signifies the version of bootstrap to install.
7. Update your angular.json file to use bootstrap. Add `node_modules/bootstrap/dist/css/bootstrap.min.css` to the styles section. Restart your server and view styles.css under the Sources tab in the browser Dev Tools to verify you see bootstrap.
8. To generate a component run `ng g c <component-name> --skip-tests` where g is short for generate and c is short for component. Run this in the root directory. Using `--skip-tests` prevents the creation of a testing file.
9. Add references for your new component to the app.module.ts file. Add these references to the imports and declarations sections if they are not already added for you.
