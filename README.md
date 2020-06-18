#  为GitHub README.md 生成目录

使用过GitHub 的应该知道README.md 并不支持 [TOC]  来自动生成目录

GitHub 使用的 Markdown 是 Github Flavored Markdown，简称 GFM

于是找到一个开源的生成 GFM 目录的工具：https://github.com/ekalinin/github-markdown-toc

## macOS安装：

```
$ curl https://raw.githubusercontent.com/ekalinin/github-markdown-toc/master/gh-md-toc -o gh-md-toc
$ chmod a+x gh-md-toc
```

远端GitHub README.md 

```
$ ./gh-md-toc https://github.com/wenyhooo/insurance/blob/master/README.md
```

如果是clone到本地

```
$ ./gh-md-toc 本地README.md 路径
```

生成如下：

<img src="https://tva1.sinaimg.cn/large/007S8ZIlly1gfwa11f4wrj31gi0u0k2q.jpg" alt="QQ20200618-112211@2x" style="zoom:30%;" />

然后将========下方内容，复制到你的README.md 文件中

然后就像https://github.com/wenyhooo/insurance 一样完美支持了目录

GitHub Wiki 也同样操作哦   https://github.com/wenyhooo/insurance/wiki

