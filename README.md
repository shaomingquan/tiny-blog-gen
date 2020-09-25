## tiny-blog-gen

> make your repo as post db, gen main page

### usage

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

#### advanced

modify `build.js` by yourself :)

### featrues

- group by time, tags
- use `<details>` tag, support collpase and expand
- prefix post md file with `_draft_` for draft featrue

### demos

- demo1, [shaomingquan/articles](https://github.com/shaomingquan/articles/blob/master/README.md#%E6%AC%A2%E8%BF%8E)

--------------- demo2 👇by `build.js`, 👆 is from `HEADER.md` ---------------
<details open>
    <summary>文章 (按时间)</summary>
    <ul>
        <details open>
    <summary>2020年</summary>
    <ul>
        <details open>
    <summary>4月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post4.md">post4</a><span>&nbsp;</span></li></ul>
    </ul>
</details>
    </ul>
</details><details open>
    <summary>2019年</summary>
    <ul>
        <details open>
    <summary>7月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post5.md">post5</a><span>&nbsp;</span></li></ul>
    </ul>
</details><details open>
    <summary>6月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post7.md">post7</a><span>&nbsp;</span></li></ul>
    </ul>
</details><details >
    <summary>4月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post3.md">post3</a><span>&nbsp;</span></li></ul>
    </ul>
</details>
    </ul>
</details><details >
    <summary>2018年</summary>
    <ul>
        <details >
    <summary>12月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post6.md">post6</a><span>&nbsp;</span></li></ul>
    </ul>
</details>
    </ul>
</details><details >
    <summary>2017年</summary>
    <ul>
        <details >
    <summary>12月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post2.md">post2</a><span>&nbsp;</span></li></ul>
    </ul>
</details>
    </ul>
</details><details >
    <summary>2016年</summary>
    <ul>
        <details >
    <summary>8月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post1.md">post1</a><span>&nbsp;</span></li></ul>
    </ul>
</details><details >
    <summary>7月</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post8.md">post8</a><span>&nbsp;</span></li></ul>
    </ul>
</details>
    </ul>
</details>
    </ul>
</details><details >
    <summary>文章 (按标签)</summary>
    <ul>
        <details >
    <summary>javascript</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post4.md">post4</a><span>&nbsp;[2020-4-15]</span></li><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post3.md">post3</a><span>&nbsp;[2019-4-13]</span></li><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post2.md">post2</a><span>&nbsp;[2017-12-2]</span></li><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post1.md">post1</a><span>&nbsp;[2016-8-20]</span></li></ul>
    </ul>
</details><details >
    <summary>nodejs</summary>
    <ul>
        <ul><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post5.md">post5</a><span>&nbsp;[2019-7-6]</span></li><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post7.md">post7</a><span>&nbsp;[2019-6-10]</span></li><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post6.md">post6</a><span>&nbsp;[2018-12-9]</span></li><li><a href="https://github.com/shaomingquan/tiny-blog-gen/blob/master/src/post8.md">post8</a><span>&nbsp;[2016-7-18]</span></li></ul>
    </ul>
</details>
    </ul>
</details>

--------------- demo2 👆 `build.js`, 👇 is from `FOOTER.md` ---------------

> this is footer