# AEM Quick Site Template 

1. Create a Maven archetype project and ensure `includeQuickSiteTemplate` is enabled (`y`). 

```
$ mvn -B archetype:generate \
 -D archetypeGroupId=com.adobe.aem \
 -D archetypeArtifactId=aem-project-archetype \
 -D archetypeVersion=28-SNAPSHOT \
 -D appTitle="My Site" \
 -D appId="mysite" \
 -D groupId="com.mysite" \
 -D includeQuickSiteTemplate=y
```

2. Build and deploy the AEM project.

```
$ cd mysite
$ mvn clean install -PautoInstallSinglePackage
```

3. Build and deploy the Quick Site Template.

```
$ cd aem-site-template
$ git init
$ npm i
$ npm run build
$ npm run deploy
```

4. Log into AEM and create a site from template: _Sites_ > _Create_ > _Site (Template)_.
