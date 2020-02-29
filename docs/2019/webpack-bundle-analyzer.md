### webpack bundle analyzer配置

#### 简介
&emsp;webpack-bundle-analyzer作为一款打包分析插件，我们可以通过它很清楚的查看到项目中引入了哪些模块，以及各个模块的大小。从而根据实际情况，做相应的分割加载，按需优化。

&emsp;先来看一下官方效果图：
![webpack-bundle-analyzer](./webpack-bundle-analyzer.gif)

#### 配置
&emsp;它的使用也很简单，安装插件后，直接引入即可：
```nohighlight
    const BundleAnalyzerPlugin = require('webpack-bundle-analyzer').BundleAnalyzerPlugin;
 
    module.exports = {
        plugins: [
            new BundleAnalyzerPlugin({
                analyzerMode: 'static' //默认为server,建议配置成static
            })
        ]
    }
```
在实际使用中，把analyzerMode配置为：static，方便随时查看分析优化效果。