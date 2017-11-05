# Getting started

Getting started with this gitbook template is easy. You will need a couple of things installed on your machine:

 - Node 
 - Git

Also, basic understanding of how git and github work is required.

Clone this repo to your local file system in a directory called `my-awesome-book`:
```
git clone https://github.com/Zaid-Ajaj/gitbook-template.git my-awesome-book
```

`cd` your way to the created directory:
```
cd my-awesome-book
```

At this point you have the template as a git repo on your machine pointing to the original git repo of the template. You don't want this, you want the local repo to point to one of your repos on github, so the to do this, you follow these steps:

 - Create an empty git repo on github, don't include anything yet
 - Create an empty `gh-pages` branch from github
 - On your local repo, delete the `.git` directory
 - `git init`
 - `git remote add origin YOUR_REPO_URL`

Now add the files to your repo:

```
git add --all
git commit -m "Initial commit"
git push --set-upstream origin master
```
Now that have your backend setup, you can start using gitbook but first you need to install the developement dependencies from from npm using:

```
npm install
```

After that you will have three commands you will use:
- Building the gitbook
- Serve gitbook and watch/reload on every change
- Publish your gitbook output to github pages (gh-pages branch)

You run these commands as npm scripts:
```
npm run build
npm run serve
npm run publish
```

Notice that `npm run publish` requires you set up the repo information in your package.json file, for example, the `repo.url` option is retrieved from package.json. 