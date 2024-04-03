# blog-repo

Personal blog repo using hexo-butterfly-theme as submodule

## How To
```bash
# Initialize Hexo Blog (name:blog-repo)
npm install hexo-cli -g
hexo init blog-repo
cd blog-repo

# Add Remote Branch (name:blog-repo.git)
git init 
git branch -m master main
git remote add origin https://github.com/extreme-rearranger/blog-repo.git
git add .
git commit -m "initialize hexo blog"
git push origin main

# Add Submodule (name:hexo-theme-butterfly.git -b own-blog)
# create additional branch from the forked theme repo
git submodule add -b own-blog https://github.com/ex-rearranger/hexo-theme-butterfly.git themes/butterfly
git add .
git commit -m "add butterfly submodule"
git push origin main

```