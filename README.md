# Angular Docker

Application example built with [Angular](https://angular.io/) 17 and running the image in a [Docker](https://www.docker.com/) container.

This tutorial was posted on my [blog](https://rodrigo.kamada.com.br/blog/criando-e-executando-uma-aplicacao-angular-em-um-conteiner-docker) in portuguese and on the [Substack](https://rodrigokamada.substack.com/p/creating-and-running-an-angular-application) in english.


[![Website](https://shields.braskam.com/v1/shields?name=website&format=rectangle&size=small&radius=5)](https://rodrigo.kamada.com.br)
[![LinkedIn](https://shields.braskam.com/v1/shields?name=linkedin&format=rectangle&size=small&radius=5)](https://www.linkedin.com/in/rodrigokamada)
[![Twitter](https://shields.braskam.com/v1/shields?name=twitter&format=rectangle&size=small&radius=5)](https://twitter.com/rodrigokamada)
[![Instagram](https://shields.braskam.com/v1/shields?name=instagram&format=rectangle&size=small&radius=5)](https://www.instagram.com/rodrigokamada)



## Prerequisites


Before you start, you need to install and configure the tools:

* [git](https://git-scm.com/)
* [Node.js and npm](https://nodejs.org/)
* [Angular CLI](https://angular.io/cli)
* [Docker Engine](https://docs.docker.com/engine/install/)
* IDE (e.g. [Visual Studio Code](https://code.visualstudio.com/))



## Getting started


### Create the Angular application


[Angular](https://angular.io/) is a development platform for building WEB, mobile and desktop applications using HTML, CSS and TypeScript (JavaScript). Currently, Angular is at version 17 and Google is the main maintainer of the project.

**1.** Let's create the application with the Angular base structure using the `@angular/cli` with the server-side rendering (SSR) disabled, the route file and the SCSS style format.

```powershell
ng new angular-docker --ssr false --routing true --style scss
CREATE angular-docker/README.md (1067 bytes)
CREATE angular-docker/.editorconfig (274 bytes)
CREATE angular-docker/.gitignore (548 bytes)
CREATE angular-docker/angular.json (2806 bytes)
CREATE angular-docker/package.json (1045 bytes)
CREATE angular-docker/tsconfig.json (903 bytes)
CREATE angular-docker/tsconfig.app.json (263 bytes)
CREATE angular-docker/tsconfig.spec.json (273 bytes)
CREATE angular-docker/.vscode/extensions.json (130 bytes)
CREATE angular-docker/.vscode/launch.json (470 bytes)
CREATE angular-docker/.vscode/tasks.json (938 bytes)
CREATE angular-docker/src/main.ts (250 bytes)
CREATE angular-docker/src/favicon.ico (15086 bytes)
CREATE angular-docker/src/index.html (299 bytes)
CREATE angular-docker/src/styles.scss (80 bytes)
CREATE angular-docker/src/app/app.component.scss (0 bytes)
CREATE angular-docker/src/app/app.component.html (20884 bytes)
CREATE angular-docker/src/app/app.component.spec.ts (940 bytes)
CREATE angular-docker/src/app/app.component.ts (373 bytes)
CREATE angular-docker/src/app/app.config.ts (227 bytes)
CREATE angular-docker/src/app/app.routes.ts (77 bytes)
CREATE angular-docker/src/assets/.gitkeep (0 bytes)
✔ Packages installed successfully.
    Successfully initialized git.
```

**2.** Now we will run the application with the command below.

```powershell
npm start

> angular-docker@0.0.0 start
> ng serve


Initial Chunk Files | Names         |  Raw Size
polyfills.js        | polyfills     |  82.71 kB | 
main.js             | main          |  23.23 kB | 
styles.css          | styles        |  96 bytes | 

                    | Initial Total | 106.03 kB

Application bundle generation complete. [1.504 seconds]
Watch mode enabled. Watching for file changes...
  ➜  Local:   http://localhost:4200/
```

**3.** Ready! Next, we will access the URL `http://localhost:4200/` and check if the application is working.
