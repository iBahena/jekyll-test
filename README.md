# jekyll-test

This is an example to deploy Jekyll to GitHub Pages from a subdirectory. Custom commands are specified in the .gitconfig file.

#### Example
The following commands have been turned into a one line command:
```
git checkout master
git subtree split --prefix dist -b gh-pages
git push -f origin gh-pages:gh-pages
git branch -D gh-pages
```

Deploying to gh-pages command using the default output directory:
```
git gh-deploy
```
By default, the output directory is called 'dist.' This can be replaced with your own output directory name by entering an optional input parameter.
```
git gh-deploy $optionalOutputDirName
```

<a href='https://ibahena.github.io/jekyll-test/'>>> Preview here <<</a>
