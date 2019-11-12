## `brew` 更新/下载缓慢 切换国内镜像源

[原文链接(中科大源)](https://lug.ustc.edu.cn/wiki/mirrors/help/brew.git)

替换:

```
替换 brew.git:
cd "$(brew --repo)"
git remote set-url origin https://mirrors.ustc.edu.cn/brew.git

替换 homebrew-core.git:
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://mirrors.ustc.edu.cn/homebrew-core.git

替换 Bottles (假设是 zsh):
echo 'export HOMEBREW_BOTTLE_DOMAIN=https://mirrors.ustc.edu.cn/homebrew-bottles' >> ~/.zshrc
source ~/.zshrc
```

重置:

```
重置 brew.git:
cd "$(brew --repo)"
git remote set-url origin https://github.com/Homebrew/brew.git

重置 homebrew-core.git:
cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"
git remote set-url origin https://github.com/Homebrew/homebrew-core.git

重置 Bottles:
删掉配置文件的那一行重启 zsh 即可
```

*[清华源链接](https://mirrors.tuna.tsinghua.edu.cn/help/homebrew/)*

