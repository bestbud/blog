
#### 安装 shadowsocks 支持科学上网，再慢慢安装其他软件
- Chrome 浏览器
- [iterm2](https://www.iterm2.com/)： 相关的命令行工具好多，可以专门写一篇了
- 搜狗输入法
- 为知笔记
-----------
#### 一些确实好用的收费软件
可以购买正版，也可以求助万能的淘宝

- Alfred: 聚焦搜索升级版，有更多强大功能，超好用，网上有很多推荐文章，也值得好好写一下
- Zoom
- Moom   
  窗口大小管理工具
- iStat Menus

-----------
#### App Store 安装
- 微信 WeChat
- Xcode
- MindNode 或 Xmind

----------

#### 安装软件包管理软件 **homebrew**
有好多软件可以通过 brew install 安装，非常方便，需要先安装 homebrew   
我按照官网安装说明安装失败了,安装过程遇到挺多问题，可参考以下安装步骤：      
1. 如果没有安装 Xcode 先安装 xcode，并打开 Xcode, 勾选同意协议
2. 运行`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

>如果遇到问题 /usr/local/homebrew/.git: Permission denied Failed during: git init -q    
可以运行： `sudo chown -R $(whoami) /usr/local` 解决   
refer to https://gist.github.com/irazasyed/7732946    



#### 使用 homebrew 安装一些有用的软件
- z 命令行跳转工具，只需要前期运行几次 `z cd + 常用目录`，即可一劳永逸的使用 `z 目录关键词` 跳转的该目录    
  ps. d 查看历史目录对应的数字，输入数字跳转也很方便
- bat：cat 的高亮升级版，更好用
- fd：find 的升级版
- ripgrep： grep 的升级版，更快更好用，rg [关键词] 搜索当前文件夹
- exa：ls 的升级版， `exa -T` 显示目录树

--------------

#### **[oh-my-zsh](https://ohmyz.sh)** 一个非常好用的管理 zsh 配置的工具
zsh 默认已经安装，设置 zsh 默认 shell `chsh -s $(which zsh)`，使用 `echo $SHELL` 确认是否设置成功  
[安装 oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH):    
运行 `sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
~/.zshrc 设置内容，`exec $SHELL` 生效   

oh-my-zsh 含很多实用插件和主题, 网上有很多配置相关的文章可以参考   
- 主题：本人比较喜欢 apple

- 插件：
  - Zsh-syntax-highlighting  
    命令检查，高亮提示，错误显示为红色，正确显示为绿色，超实用。    
    需要手动安装 `cd ~/.oh-my-zsh/custom/plugins && git clone https://github.com/zsh-users/zsh-syntax-highlighting`， 并将 zsh-syntax-highlighting 添加到 .zshrc 文件的 plugins list

  - Zsh-autosuggestions    
    自动补全命令工具，会根据历史命令给出命令建议，点击 → 可以补全命令，超实用。   
    安装方式同 Zsh-syntax-highlighting   
    `cd ~/.oh-my-zsh/custom/plugins && git clone https://github.com/zsh-users/zsh-autosuggestions`， 并将 zsh-autosuggestions 添加到 .zshrc 文件的 plugins list
  - Colored-man-pages：高亮显示 man pages 内容
- alias: 为一些常用命令定义别名可以少输入一些字符，非常方便    
  - 后缀别名 suffix alias，基于文件扩展名的指定代开文件的工具。   
    使用 `alias -s` 定义，eg.   
    `alias -s {yml,yaml}=vim`  用 vim 打开后缀为 yml,yaml 文件
  - 全局别名 global alias, 使您可以创建在命令行中的任何位置扩展的别名，对于替换常见文件名或管道命令非常有用    
    使用 `alias -g` 定义，eg.   
    `alias -g G='| grep -i'` 可以在输入管道命令的任何位置 输入`G [关键词]` 搜索关键词  
    `ls G xxx` 会输出含 xxx 的文件

   

> 推荐阅读
>  - [jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide](https://www.freecodecamp.org/news/jazz-up-your-zsh-terminal-in-seven-steps-a-visual-guide-e81a8fd59a38/)
>  - [5 tips to improve productivity with zsh]( https://opensource.com/article/18/9/tips-productivity-zsh)          

-----------

#### 软件开发

- webStorm
- n： node 版本管理工具 `brew install n`
- explainshell 查看命令的含义
- Codelf(变量命名搜索)

-----------

#### mac 入门需知
- 录屏功能 ⌘ + ⇧ + 5: 可以截图录屏，非常方便

- 预览编辑: 选中文件按下 space 显示预览，再次按下 space 键关闭预览   
  安装额外的[预览插件](https://github.com/sindresorhus/quick-look-plugins)可以支持预览代码、json、markdown，查看图片信息等    
  使用以下命令安装多个插件    
  `brew cask install qlcolorcode qlstephen qlmarkdown quicklook-json qlimagesize webpquicklook suspicious-package quicklookase qlvideo`
  
- 输入特殊字符：按 ⌘ + ⌃ + Space 能够快捷调出「显示表情与符号」对话框，供我们快速选择表情或者符号输入


------------

#### 一些提高工作效率的简单命令

- `open ./ -a webStorm` ，可以直接用 webStorm 打开当前目录


------------

#### iterm2 高效实用建议
- 设置为默认 Term: 打开 iTerm，在默认菜单中选择"Make iTerm2 Default Term"
- show/hide 快捷键设置，⌃ +  ⌥ + ⌘ + space
- 快捷键 ⇧ + ⌘ + h，快速显示复制内容的历史记录，很方便。
- ⌘ + enter,可以快速实现全屏与正常窗口大小的切换。
- ⌘ + u, 切换背景是否支持透明度，可以设置一个较大的透明度，只在需要看窗口覆盖内容的时候切换为支持透明度
- shell integration    
  菜单栏点击 iTerm2 -> install shell integration, 弹出对话框选择 install Shell Integration & Utilities   
  安装后就可以使用以下命令，很实用   
  - `imgcat [filename]`
    在命令行中显示图片
  - `imgls`
    列出当前目录下所有图片的缩略图
  - `it2copy [filename]`
    将文件内容 copy 至剪贴板




---------------

#### Alfred 
聚焦搜索快捷键改为 **⌥ + space**，修改快捷键为 Alfred 快捷键为 **⌘ + space**

alfred ⌥⌘C 剪切板历史

// todo  整理 Web Search 和 workflow

https://explainshell.com/ 


-------------- 
 

 






