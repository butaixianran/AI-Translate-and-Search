# 重要说明
## 请前往Chrome扩展版本的项目池。User Script脚本版本不再更新

## 由于Chrome迁移到manifest v3带来的一系列改变，User Script版本已经被淘汰，请前往Chrome扩展版本的项目池，使用Chrome扩展版本。

[Chrome扩展版本项目池](https://github.com/butaixianran/Chrome-Extension-AI-Translate-and-Search)  


# AI-Translate-and-Search
划词AI翻译+搜索：
* **AI翻译按质量和热度综合排序。调用：** 金山翻译，有道翻译，阿里翻译，百度翻译，搜狗翻译，腾讯翻译，彩云小译，DeepL，沪江日语词典等。
* **搜索包含：** 知乎，b站，微博，百科, wiki，youtube，twitter等。
* **设置：** 展开后，点击“Setting”可以调整 排序 和 是否显示。

# 预览图
**选择一段文本后：**  
![ShortMode](https://github.com/butaixianran/AI-Translate-and-Search/blob/main/res/img/ShortMode.jpg)

**展开后：**  
![FullMode](https://github.com/butaixianran/AI-Translate-and-Search/blob/main/res/img/FullMode.jpg)


# 安装
Chrome扩展版本：
https://chrome.google.com/webstore/detail/ai%E7%BF%BB%E8%AF%91%E5%92%8C%E6%90%9C%E7%B4%A2/hgccnmjdlfakepijceijgkbicglomcoa

User Script版本：  
https://greasyfork.org/zh-CN/scripts/420649-ai-translate-and-search

Chrome类浏览器需要先安装Tampermonkey扩展，才能安装用户脚本。  
https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo

github地址：  
https://github.com/butaixianran/AI-Translate-and-Search

# 创作说明
根据barrer发布的用户脚本改编。  
https://github.com/barrer/tampermonkey-script  

**修改说明：**  
* 添加阿里翻译，阿里云翻译，腾讯翻译，彩云小译
* 重新排序，翻译按照质量和热度综合排序
* 修改百度翻译为自动识别语言
* 修改沪江英语词典为沪江日语词典
* 增加搜索：知乎，b站，微博，百科，中日英3语wiki，youtube，twitter等
* 去掉大量不常用词典

# AI翻译服务质量
AI翻译服务，质量差异主要体现在：词汇量 和 语言通畅程度 两个方面。尤其是非英语翻译，比如日语翻译。  

综合来看，质量比较好的，是 阿里云翻译 和 金山翻译。然而，通过脚本调用翻译页面，实现无须API的免费翻译时，则各有不便。各翻译服务问题列举如下： 
* **金山翻译：**  翻译质量高，且 单词 翻译提供详细字典。但长文翻译时，通过脚本调用无法分段落。
* **阿里翻译：** 阿里云翻译，质量曾经很好，但后来似乎更换AI引擎重新学习，质量一落千丈。默认是把内容翻译成英文，需要手动选一下中文。
* **有道翻译：** 翻译质量比金山差，和百度各有千秋，但排版更好，脚本调用便利
* **腾讯翻译：** 词汇量和阿里云翻译一致，但语言组织不如阿里通畅。
* **搜狗翻译：** 语言通畅程度和阿里云一致，但词汇量略少。
* **百度翻译：** 做得久，名气大，然而质量一般。只是其他AI翻译服务都是刚起步，均未宣传而已。
* **DeepL：** 语言流畅程度和阿里云相当，但日语等语种的词汇量小。而且它是把所有语言先翻译成德语，再把生成的德语翻译成目标语言，因此出错率更高，甚至出现无法翻译的情况。
* **彩云小译：**  日语词汇量较大，能准确翻译 烧卖、美人鱼等其他翻译服务经常翻译错误的娱乐领域词汇。详情参见：<a href="https://github.com/lmk123/crx-selection-translate/issues/466#issuecomment-743978724" target="_blank">彩云小译的日文词汇量优势</a>
* **Google翻译：** 质量稀烂。Google也是AI翻译，但是，他是把所有语言，先翻译成英语，再把机器翻译的英语，翻译成目标语言。英语是个非常不严谨的语言，于是大量的多义词和语境，在二次转换后，全部翻译错误。质量烂到难以忍受。给google翻译提交建议的时候，被官方社区的管理人员反复踢皮球。可见这个翻译产品，今后也是不可能做好的。因此，这里不予添加。


# 更新说明
## v0.7
脚本改名，改为中文名，方便greasyfork搜索

## v0.6
因为阿里翻译更新后已经包含阿里云的语种，因此移除阿里云

## v0.5
把跳出新页面，改为新标签页

## v0.4
忘了

## v0.3
* 金山翻译恢复URL地址调用，因此本脚本也恢复直接跳转到翻译结果页面

## v0.2
* 金山翻译关闭直接通过URL地址调用，如今必须手动按一下回车。修改脚本适应，并降低金山翻译优先级。
* 修复“复制为纯文本”后，导致普通复制失效的问题
