# VIM 中文文档 (Vim Chinese Documentation)

## 注意

从 6.3 版开始，Vim 加入了对翻译文档的支持。因而本仓库仅适用于 Vim 6.3 及以后的版本。如果你使用的是 Vim 6.2 或以前的版本，建议升级到 6.3 或更高版本。


## 使用方法

我在`.vimrc/_vimrc`文件中加入以下匹配以方便正确识别

```viml
" 设定 doc 文档目录
let helptags=$VIM."/vimfiles/doc"
set helplang=cn
```

## 安装

### vim-plug 安装

在`.vimrc/_vimrc`文件中加入一句
```viml
Plug 'asins/vimcdoc'
```
运行`:PlugInstall`完成安装

### NeoBundle 安装

在`.vimrc/_vimrc`文件中加入一句
```viml
NeoBundle 'asins/vimcdoc'
```
运行`:NeoBundleInstall`完成安装

### Vundle 安装

在`.vimrc/_vimrc`文件中加入一句
```viml
Plugin 'asins/vimcdoc'
```
运行`:PluginInstall`完成安装

### Pathogen 安装

在终端（命令提示符）下执行以下语句

Linux:
```bash
cd ~/.vim/bundle && \
git clone git://github.com/asins/vimcdoc.git
```
Windows:
```bash
cd （你的 Vim 配置文件目录）\bundle
git clone git://github.com/asins/vimcdoc.git
```
重启 VIM 即可正常使用

### 独立安装

将 doc 文件夹放到`~/.vim`(linux) / `$VIM\vimfiles`(window) 目录中，然后在 VIM 中进行`:helptags ~/.vim/doc`(linux) 或者`:helptags $VIM\vimfiles\doc`，完成后会在 doc 目录下生成 tag 以及 tag-cn 文件。

## 插件文档

文档中也整合了已翻译的常用插件，方便随时查询，也欢迎大家完善，已加入：

- [NERD_commenter][2] 提供许多不同的注释操作和风格的代码注释插件
- [NERD_tree][4] 像妈妈一样体贴的树形浏览插件！
- bufexplorer Buffer Explorer
- CtrlP 模糊检索文件，缓冲区，最近最多使用，标签等的 Vim 插件
- markdown Markdown 标记语言
- matchit 扩展 "%" 的匹配功能
- template 智能加载模板文件
- ag 快速搜索工具


## 申明

- Vim 中文文档来源于 [http://vimcdoc.sourceforge.net/][1]
- Vim 英文文档 [https://github.com/vim/vim/tree/master/runtime/doc][3]

  [1]: http://vimcdoc.sourceforge.net/
  [2]: https://github.com/scrooloose/nerdcommenter
  [3]: https://github.com/vim/vim/tree/master/runtime/doc
  [4]: https://github.com/scrooloose/nerdtree

