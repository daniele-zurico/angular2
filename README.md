- Install
    - npm install -g jspm@beta live-server
    - jspm init (transpiler: typescript)
    - jspm install npm:reflect-metadata npm:zone.js npm:angular2
    - "typescriptOptions": {"emitDecoratorMetadata": true, "experimentalDecorators": true} to config.js
- Run a server
    live-server
-Access to your browser
    http://localhost:8082/first/index.html
    
- BUILD FOR PRODUCTION
    jspm bundle-sfx --minify reflect-metadata + zone.js + app/main.js build/bundle.js