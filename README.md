## WZTheme
用于公司App节日主题更新代码

###使用方式

先在自己项目里给个默认主题的资源文件，如demo里的main.bundle文件
然后在里面放入默认主题的图片，如需从网络下下载新的主题包只要将这个main.bundle文件复制出来然后将新的主题的图片放入里面，在上传到自己公司的服务器，然后通过接口拿到这里链接，接着在代码里下载主题就可以了。代码如下：

设置默认主题代码:

```
    [[WZThemeManger manger] defaultThemeWithBunldeName:@"main" themeName:@"默认主题"];
    
```
下载新主题代码:

```
    [[WZThemeManger manger] downloadThemeFrom:@"https://github.com/hwzss/WZTheme/raw/master/theme.zip" themeName:@"github上新的主题"];
```

最近刚弄这块代码，如果您刚好看到这块代码，有兴趣或者对这代码有什么好的优化方案或者更好的实现方法可以联系我，或者在issue里留言。
