# Getting Started With Angular
getting started with angular official docs

## Requirements
1. node 	```node -v```
2. npm 		```npm -v```
3. ```npm install -g @angular/cli```

## Create New Project
```
ng new my-app
```

Run the app using

```
ng serve --open
```

ng serve launches the server, watches the files and rebuilds the app as we make changes.
```--open``` automatically opens the app in browser at ```localhost:4200```

## Edit First Angular Component
The page you are seeing is rendered from ```my-app/src/app/app.component.ts``` So we are going to change the ```title``` of our app. Change ```my-app``` to ```My First Angular App```

```
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'My First Angular Project';
}
```

Save the file and if you see in the console, the app is rebuild and the browser window 
reloads automatically reflecting your changes.

We can even add some styling by modifying ```./src/app/app.component.css```

```
h1 {
  color: #369;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 250%;
}
```

You can look at the changes in the browser.
