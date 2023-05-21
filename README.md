# Blog

```bash
jekyll -v
jekyll new blog
cd blog
```

This create a new folder **blog** with some files
* `Gemfile`
* `Gemfile.lock`
* `_config.yml`
* `index.markdown`
* `about.markdown`

and a `_posts` folder.

Add required gems to Gemfile
```bash
gem "webrick", "~> 1.7"
gem "jekyll-include-cache"
gem "minimal-mistakes-jekyll"
```

install gems, rewrite Gemfile.lock
```bash
bundle update
```

Run jekyll
```bash
bundle exec jekyll serve --livereload
```

Open browser at `http://127.0.0.1:4000/` you should see the blog with a sinmple *Welcome to Jekyll!* post.

Add/replace in `_config.yml`:
```bash
theme                 : "minimal-mistakes-jekyll"
minimal_mistakes_skin : "default" # "air", "aqua", "contrast", "dark", "dirt", "neon", "mint", "plum", "sunrise"

