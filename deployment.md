Step-by-Step Guide to Manually Deploy a React App to GitHub Pages
Build Your Project Locally: Make sure you have all your dependencies installed and then run the build command:
```
sh
npm install
npm run build
This will create a build directory containing the production-ready version of your app.
```
Create a .nojekyll File: To bypass Jekyll processing, create a .nojekyll file in the build directory:

sh
echo "" > build/.nojekyll
Initialize Git in the build Directory: If Git is not already initialized in the build directory, you can initialize it:

sh
cd build
git init
Commit and Push to the gh-pages Branch: Add, commit, and push the contents of the build directory to the gh-pages branch:

sh
git add .
git commit -m "Deploy React app to GitHub Pages"
git remote add origin https://github.com/your-username/your-repo-name.git
git branch -M gh-pages
git push -u origin gh-pages --force
Replace your-username and your-repo-name with your actual GitHub username and repository name.

Example Commands Recap:
Build the React App:

sh
npm install
npm run build
Create .nojekyll:

sh
echo "" > build/.nojekyll
Initialize Git in build Directory:

sh
cd build
git init
Add, Commit, and Push:

sh
git add .
git commit -m "Deploy React app to GitHub Pages"
git remote add origin https://github.com/your-username/your-repo-name.git
git branch -M gh-pages
git push -u origin gh-pages --force


Correct URL :
git remote -v
git remote set-url origin https://github.com/your-username/your-correct-repo-name.git

Add commit push
cd build
git add .
git commit -m "Deploy React app to GitHub Pages"
git push -u origin gh-pages --force

