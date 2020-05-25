#Requirements 

* eslint 5.16

#Instalation

 `npm i https://github.com/Paul-Petrash/linter.git`
 
 `create file .eslintrc with the following content inside your root project folder`
 
  ```{
      "extends": "./index.js",
      "rules": {
        // disable requiring trailing commas because it might be nice to revert to
        // being JSON at some point, and I don't want to make big changes now.
        "comma-dangle": 0,
      },
      "env": {
        "browser": true,
        "node": true,
        "jasmine": true
      }
    }
``` 
 

#SETUP WEBSTORM

1) go to Setting(Preferences) -> JS -> Code quality tools -> ESlint 
2) set checkbox enabled
3) select used at project node version
4) select installed eslint module (use eslint version 5 for IDE version lower when 2019.2)
5) select Use specific config file and select .eslintrc file inside your root project folder
