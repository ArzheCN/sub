# 随机诗词接口

## 一言

### 简介

#### 古诗词·一言API是一个可以随机返回一句古诗词名句的接口。具有以下特点：

* 快：使用 Vert.x Java 全异步框架开发，毫秒级稳定响应
* 全：支持 svg / txt / json / png 调用，满足你在任何地方的调用需求
* 多：收录将近10000条古诗词名句
* 准：可以根据你的喜好，在指定的分类中进行随机返回

### 使用

**API举例**

* [https://v1.jinrishici.com/all.json](https://v1.jinrishici.com/all.json)
* [https://v1.jinrishici.com/all.svg](https://v1.jinrishici.com/all.svg)
* [https://v1.jinrishici.com/shuqing/libie.png](https://v1.jinrishici.com/shuqing/libie.png)
* [https://v1.jinrishici.com/rensheng.txt](https://v1.jinrishici.com/rensheng.txt)

**API地址格式(仅支持https)**

`https://v1.jinrishici.com/{一级分类}/{二级分类(可选)}.{返回格式(可选)}`

查看所有目前支持的分类：[https://v1.jinrishici.com/](https://v1.jinrishici.com/)

目前支持的后缀：.svg .txt .png .json 不加后缀默认返回 json

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-cover data-type="files"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td></td><td>官网</td><td></td><td><a href="../../.gitbook/assets/{8FF002F8-5330-445F-A534-CFFA646269F3} (1).png">{8FF002F8-5330-445F-A534-CFFA646269F3} (1).png</a></td><td><a href="http://gushi.ci/">http://gushi.ci/</a></td></tr></tbody></table>

## 今日诗词

### 通用简单安装代码 <a href="#json-fast-easy" id="json-fast-easy"></a>

在 HTML 中需要加载诗词的地方放置以下加载代码即可,和 **网站统计** 的安装方法一致。

```
<span id="jinrishici-sentence">正在加载今日诗词....</span>
<script src="https://sdk.jinrishici.com/v2/browser/jinrishici.js" charset="utf-8"></script>
```

### 通用高级安装代码 <a href="#json-fast-custom" id="json-fast-custom"></a>

如果你有其他需求（如获取作者、朝代等），可以调用我们提供的加载函数 `jinrishici.load` 并传入回调函数，每调用一次，会传入一个新的诗词

```
<script src="https://sdk.jinrishici.com/v2/browser/jinrishici.js" charset="utf-8"></script>
<script type="text/javascript">
  jinrishici.load(function(result) {
    // 自己的处理逻辑
    console.log(result)
  });
</script>
```

一个高级版的使用例子，可以复制到一个 HTML 文件用浏览器打开查看效果：

```
<script src="https://sdk.jinrishici.com/v2/browser/jinrishici.js" charset="utf-8"></script>
<div id="poem_sentence"></div>
<div id="poem_info"></div>
<script type="text/javascript">
  jinrishici.load(function(result) {
    var sentence = document.querySelector("#poem_sentence")
    var info = document.querySelector("#poem_info")
    sentence.innerHTML = result.data.content
    info.innerHTML = '【' + result.data.origin.dynasty + '】' + result.data.origin.author + '《' + result.data.origin.title + '》'
  });
</script>
```

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-cover data-type="files"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td></td><td>官网地址</td><td></td><td><a href="../../.gitbook/assets/{8B8B4BC0-6723-49EE-8923-931C96AD2666}.png">{8B8B4BC0-6723-49EE-8923-931C96AD2666}.png</a></td><td><a href="https://www.jinrishici.com/">https://www.jinrishici.com/</a></td></tr></tbody></table>

## 一句

一句API返回随机一句古诗词，通过调用一句API，您可以在您的网站上、APP内随时方便快速地显示、获取古诗词句。

&#x20;注：一句API目前不保证完全稳定，请勿用于严肃用途！ 希望在您的APP、网站等项目内使用时注明API来自一句！&#x20;

### 开发帮助文档&#x20;

直接返回纯本文 `http://yijuzhan.com/api/word.php`&#x20;

JSON方式调用(2018.08.23新增) `http://yijuzhan.com/api/word.php?m=json`&#x20;

JSON数据示例：

`{"content":"有谁知我此时情，枕前泪共阶前雨，隔个窗儿滴到明。","source":"聂胜琼《鹧鸪天·别情》"}`&#x20;

content：诗句内容 ｜ source：诗句作者 HTML + JS方式调用 在网页HTML中您想显示的地方加入以下代码： 显示作者(风格1)：

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th><th data-hidden data-card-cover data-type="files"></th></tr></thead><tbody><tr><td></td><td>官网地址</td><td></td><td><a href="https://yijuzhan.com/help/yiju_api.html">https://yijuzhan.com/help/yiju_api.html</a></td><td><a href="../../.gitbook/assets/{10D7FAD9-8E43-40FA-A790-F1CA48BB28AF}.png">{10D7FAD9-8E43-40FA-A790-F1CA48BB28AF}.png</a></td></tr></tbody></table>
