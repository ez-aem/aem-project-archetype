# AEM Quick Site Template 

1. Build and deploy the AEM project.

```
$ mvn clean install -PautoInstallSinglePackage
```

2. Build and deploy the Quick Site Template.

```
$ git init
$ cd aem-site-template
$ npm i
$ npm run build
$ npm run deploy
```

3. Log into AEM and create a site from template: _Sites_ > _Create_ > _Site (Template)_.
