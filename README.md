# AngularServiceWorkerIssueRepro

Repro steps:
```
npm i
npx ng build -c production
cd dist
npx http-server -p 4200
```

Then open http://127.0.0.1:4200/ in your browser, wait a few seconds for the SW to initialise and then go offline and refresh the page. You'll see that it fails to load.
