macOS 環境で Yu Gothic を使うために以下の作業を行いましょう:

```sh
sudo mkdir -p /usr/local/texlive/texmf-local/fonts/opentype/yu-osx
cd /usr/local/texlive/texmf-local/fonts/opentype/yu-osx
sudo ln -fs "/Library/Fonts/Yu Gothic Bold.otf" YuGo-Bold.otf
sudo ln -fs "/Library/Fonts/Yu Gothic Medium.otf" YuGo-Medium.otf
sudo ln -fs "/Library/Fonts/Yu Mincho Demibold.otf" YuMin-Demibold.otf
sudo ln -fs "/Library/Fonts/Yu Mincho Medium.otf" YuMin-Medium.otf
sudo mktexlsr
sudo updmap-sys --setoption kanjiEmbed yu-osx
```

参考:

* http://tandoori.hatenablog.com/entry/20131117/1384696037
* http://doratex.hatenablog.jp/entry/20161202/1480665692
