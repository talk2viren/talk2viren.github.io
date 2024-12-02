## Step-by-Step Guide to Manually Deploy a React App to GitHub Pages
Build Your Project Locally: Make sure you have all your dependencies installed and then run the build command:

Step 1 : Create a build directory containing the production-ready version of your app.

```
npm install
npm run build
```

Step 2 : Create a .nojekyll File: To bypass Jekyll processing, create a .nojekyll file in the build directory:

```
echo "" > build/.nojekyll
```

Step 3 : Initialize Git in the build Directory: If Git is not already initialized in the build directory, you can initialize it:

```
cd build
git init
```
Step 4 : Commit and Push to the gh-pages Branch

```
git add .
git commit -m "Deploy React app to GitHub Pages"
git remote add origin git@github.com:talk2viren/talk2viren.github.io.git
git branch -M gh-pages
git push -u origin gh-pages --force

# Replace your-username and your-repo-name with your actual GitHub username and repository name.
```
Example Commands Recap:
Build the React App:

```
npm install
npm run build
Create .nojekyll:
```

```
echo "" > build/.nojekyll
Initialize Git in build Directory:
```
## Push build folder

```
cd build
git init
Add, Commit, and Push:
```

## Help
```
git add .
git commit -m "Deploy React app to GitHub Pages"
git remote add origin https://github.com/your-username/your-repo-name.git
git branch -M gh-pages
git push -u origin gh-pages --force
```

### Command
```
Correct URL :
git remote -v
git remote set-url origin git@github.com:talk2viren/talk2viren.github.io.git
```
```
Add commit push
cd build
git add .
git commit -m "Deploy React app to GitHub Pages"
git push -u origin gh-pages --force
```
