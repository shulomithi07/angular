The page that is shown on the ui is index.html

And the main component that is called in index.html is <app-root></app-root>
the selector name is taken from the app.component.ts file

So basically the first file which is served to the user is index.html.

HOW is angular getting triggered and how is app-root getting replaced with the new data.

So inside the index.html file angular cli directly adds js script links in html file.
Which internally generates the js bundels
And calls the main.ts files

Inside main.ts file we have something called as bootstrap which internally calls the required data

platformBrowserDynamic().bootstrapModule(AppModule)
  .catch(err => console.error(err));

The appmodule is called in main.ts --> here we are saying to angular that you have to look at appComponent module.

And when the control goes to app.module.ts in the bootstrap array we'll have the appModule, We are saying that nen angular starts when booting it we want angular to know that appModule exists. And inside app module we have something called as app-root.
You need to handle app-root as you know where this app root selector comes from. This information must be displayed on the UI