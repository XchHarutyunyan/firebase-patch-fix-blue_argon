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

> [!WARNING]  
> This instruction is for Firebase version ^9.9.2.

> **Note**
> If you are using a different version, follow these instructions.

1. Once you've built the production version of your code, go to your folder and search for files based on content;
2. Search for "Recaptcha" or "enterprise.js";
3. Open the file, and replace the following strings by an empty string (""):

&nbsp; * "https://www.google.com/recaptcha/enterprise.js?render=""
&nbsp; * "[https://apis.google.com/js/api.js?onload=${a}](https://apis.google.com/js/api.js?onload=$%7Ba%7D)"

4. Save your file.


