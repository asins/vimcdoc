# VIM中文文档(Vim Chinese Documentation) #

## 使用方法 ##

我在`.vimrc/_vimrc`文件中加入以下匹配以方便正确识别

    " 设定doc文档目录
    let helptags=$VIM."/vimfiles/doc"
    set helplang=cn


### 独立安装 ###

将doc文件夹放到`~/.vim`(linux) / `$VIM\vimfiles`(window)目录中，然后在VIM中进行`:helptags ~/.vim/doc`(linux)或者`:helptags $VIM\vimfiles\doc`，完成之后会在doc目录下生成tag以及tag-cn文件。

### Vundle安装 ###

在`.vimrc/_vimrc`文件中加入一句

    Bundle 'asins/vimcdoc'

重启VIM运行`:BundleInstall`即可完成安装，然后重启VIM就能正常使用了，如：

    :help bufexplorer

# 申明 #

文档内容来源于 [http://vimcdoc.sourceforge.net/]()，我只是简单搬过来并加入了些已经被翻译过来的插件中文文档

已加入的插件文档，欢迎大家完善

  - NERD_commenter 提供许多不同的注释操作和风格的代码注释插件
  - CtrlP 模糊的 文件, 缓冲区, 最近最多使用, 标签, ... 检索. v1.79
  - NERD_tree 像妈妈一样体贴的树形插件！
  - bufexplorer Buffer Explorer
  - markdown Markdown 标记语言
  - template 智能加载模板文件


