# tiny-blog-gen

> make your repo as post db, gen main page

## usage

### getting started

1. prepare
    1. fork this repo
    2. clone, `npm ci`
2. write something
    1. write posts under `./src`
    2. write meta data for every post, `date` and `tags`
    3. write `HEADER.md` and `FOOTER.md` for layout of `README.md`
3. build
    1. modify repo conf under `build.js` `const REPO = 'shaomingquan/articles'`
    2. `node build`, new `README.md` file born
    3. git add commit and push...

### rebuild

you don't need when modify a post, otherwise run `node build.js` to rebuild.

### advanced

modify `build.js` by yourself :)

## featrues

- group by time, tags
- use `<details>` tag, support collpase and expand
    - auto expand recently posts, config by `const MAX_EXPAND_CONTENT = 3` under `build.js`
- prefix post md file with `_draft_` for draft featrue

## demos

- demo1, [shaomingquan/articles](https://github.com/shaomingquan/articles/blob/master/README.md#%E6%AC%A2%E8%BF%8E)

--------------- demo2 👇by `build.js`, 👆 is from `HEADER.md` ---------------
