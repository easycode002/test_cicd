npm create vite@latest
cd demo_cicd
npm install
npm run dev
-- add git hub page

```
npm install gh-pages --save-dev
```

add it to package.json

```
"homepage": "http://{username}.github.io/{repo-name}"
like this
"homepage": "https://easycode002.github.io/test_cicd"
```

- add this to script
```
"predeploy":"npm run build",
"deploy":"gh-pages -d build"
```
