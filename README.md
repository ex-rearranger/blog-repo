# blog-repo

Personal blog repo using hexo-butterfly-theme as submodule

## How To
### Initialize Hexo Blog (ex:blog-repo)
```bash
npm install hexo-cli -g
hexo init blog-repo
cd blog-repo
```

### Add Remote Branch (ex:blog-repo.git)
```bash
git init 
git branch -m master main
git remote add origin https://github.com/extreme-rearranger/blog-repo.git
git add .
git commit -m "initialize hexo blog"
git push origin main
```

### Add Theme
#### fork the original theme to apply and create additional branch
#### add the branch as submodule (ex:hexo-theme-butterfly.git -b own-blog)
```bash
git submodule add -b own-blog https://github.com/ex-rearranger/hexo-theme-butterfly.git themes/butterfly
git add .
git commit -m "add butterfly submodule"
git push origin main
```

### Use KaTeX for Math Rendering
```bash
npm un hexo-renderer-marked --save
npm un hexo-renderer-kramed --save
npm install hexo-renderer-markdown-it --save
npm install katex @renbaoshuo/markdown-it-katex --save
```
#### after installing, add the following to _config.yml
```yaml
markdown:
  plugins:
    - '@renbaoshuo/markdown-it-katex'
```

### Use hexo-butterfly-tag-plugins-plus
```
npm install hexo-butterfly-tag-plugins-plus --save
```

#### after installing, add the following to _config.yml (ex:v1.0.17)
```yaml
# tag-plugins-plus
# see https://akilar.top/posts/615e2dec/
tag_plugins:
  enable: true # 활성화
  priority: 5 # 필터 우선 순위
  issues: false # issues 라벨 활성화
  link:
    placeholder: /img/no-image.png #link_card 라벨의 기본 이미지
  CDN:
    anima: https://npm.elemecdn.com/hexo-butterfly-tag-plugins-plus@1.0.17/lib/assets/font-awesome-animation.min.css #动画标签anima的依赖
    jquery: https://npm.elemecdn.com/jquery@1.0.17/dist/jquery.min.js #issues标签依赖
    issues: https://npm.elemecdn.com/hexo-butterfly-tag-plugins-plus@1.0.17/lib/assets/issues.js #issues标签依赖
    iconfont: //at.alicdn.com/t/font_2032782_8d5kxvn09md.js #参看https://akilar.top/posts/d2ebecef/
    carousel: https://npm.elemecdn.com/hexo-butterfly-tag-plugins-plus@1.0.17/lib/assets/carousel-touch.js
    tag_plugins_css: https://npm.elemecdn.com/hexo-butterfly-tag-plugins-plus@1.0.17/lib/tag_plugins.css
```

### Use wordcount
```bash
npm install hexo-wordcount --save
```