# firebase-patch-fix-blue_argon
Solution when Google's Blue Argon error occurs

**npm**

`npm i patch-package`

**In package.json**

```
"scripts": {
  +  "postinstall": "patch-package"
}
```

And add a ***patches*** folder to your application, after each installation of packages the Firebase package will be updated.


