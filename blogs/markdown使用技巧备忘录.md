如果不经常使用 markdown，偶尔还需要用 markdown 写一些文档，可能会忘记一些使用方法，需要现查，所以我整理了一下之前使用时临时搜索的一些 markdown 的功能，作为对常用功能的补充，也希望以后不用重复搜索这些功能了。

我会在以后用到新功能的时候持续补充内容。

## 工具
我使用的文本编辑软件是 webStorm，和我是程序员有关，是现成的工具。webStorm 的 markdown 插件支持编辑编辑+预览两栏显示，使用起来还是比较方便。


## 格式检查工具
 [lint-md](https://github.com/hustcc/lint-md)，可以检查中文 markdown 编写格式并修复。

## 设置插入图片的大小
到目前为止， Markdown 还没有办法指定图片的宽高，需要的话，可以使用普通的 `<img>` 标签。  
eg. 
`<img src="imgUrl" width = "300" height = "200" alt="图片名称" align=center />` 

  <img src="https://images.unsplash.com/photo-1557802891-958ecf3d5992?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60" width = "400" height = "200" alt="图片名称" align=center />  

## 页内跳转|锚链接

  1.定义锚  
     `<span id=”自定义id”>`  
     `<a name="anchor_xxx"></a>`
     
  2.增加跳转链接：`[名称](#anchor_xxx)`

