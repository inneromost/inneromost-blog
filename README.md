# inneromost blog

Jekyll blog published at [inneromost.com](https://inneromost.com) with GitHub Pages.

## Manage from pi.home

The working copy lives at `~/inneromost-blog` on `inneromost@pi.home`.

```bash
ssh inneromost@pi.home
cd ~/inneromost-blog
git pull --ff-only
```

Add posts to `_posts/` using the filename format `YYYY-MM-DD-title.md`. Preview a
change with:

```bash
bundle install
bundle exec jekyll serve --host 0.0.0.0
```

Publish by committing and pushing to `main`:

```bash
git add _posts
git commit -m "Add post: title"
git push
```

The GitHub Actions workflow builds, checks, and deploys each push.
