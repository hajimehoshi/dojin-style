macOS 環境で Yu Gothic を使うために以下の作業を行いましょう (実はいらないかもしれない):

```sh
sudo tlmgr update --self --all
sudo cjk-gs-integrate --link-texmf --force
sudo mktexlsr
sudo updmap-sys --setoption kanjiEmbed yu-osx
```

参考:

* http://doratex.hatenablog.jp/entry/20151008/1444310306
* http://abenori.blogspot.jp/2015/10/el-capitantexplatex-dvipdfmxpdflatexmac.html
* http://doratex.hatenablog.jp/entry/20161202/1480665692
