# VIM中文文档(Vim Chinese Documentation) #

## 使用方法 ##

我在`.vimrc/_vimrc`文件中加入以下匹配以方便正确识别

    " 设定doc文档目录
    let helptags=$VIM."/vimfiles/doc"


### 独立安装 ###

将doc文件夹放到`~/.vim`(linux) / `$VIM\vimfiles`(window)目录中，然后在VIM中进行`:helptags ~/.vim/doc`(linux)或者`:helptags $VIM\vimfiles\doc`，完成之后会在doc目录下生成tag以及tag-cn文件。

### Pathogen 安装 ###

在终端(命令提示符)下执行以下语句

Linux:

    cd ~/.vim/bundle && \
    git clone git://github.com/asins/vimcdoc.git

Windows:

    cd (你的 Vim 配置文件目录)\bundle
    git clone git://github.com/asins/vimcdoc.git

重启VIM即可完成安装并正常使用了，如：

    :help bufexplorer

### Vundle 安装 ###

在`.vimrc/_vimrc`文件中加入一句

    Plugin 'asins/vimcdoc'

重启VIM运行`:PluginInstall`即可完成安装，然后重启VIM就能正常使用了，如：

    :help bufexplorer

### NeoBundle 安装 ###

在`.vimrc/_vimrc`文件中加入一句

    NeoBundle 'asins/vimcdoc'

重启VIM运行`:NeoBundleInstall`即可完成安装，然后重启VIM就能正常使用了，如：

    :help bufexplorer

# 申明 #

文档内容来源于 [http://vimcdoc.sourceforge.net/]()，我只是简单搬过来并加入了些已经被翻译过来的插件中文文档

已加入的插件文档，欢迎大家完善

  - NERD_commenter 提供许多不同的注释操作和风格的代码注释插件
  - NERD_tree 像妈妈一样体贴的树形插件！
  - bufexplorer Buffer Explorer
  - CtrlP 模糊检索文件, 缓冲区, 最近最多使用, 标签等的 Vim 插件
  - markdown Markdown 标记语言
  - matchit 扩展 "%" 的匹配功能
  - template 智能加载模板文件


