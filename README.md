# AI-Translate-and-Search
划词AI翻译+搜索：
* **AI翻译按质量排序。调用：** 金山词霸，阿里翻译，百度翻译，搜狗翻译，腾讯翻译，彩云小译，DeepL，沪江日语词典等。
* **搜索包含：** 知乎，b站，百科，youtube，twitter等。去掉了原作者提供的大量不常用词典。

# 预览图
**选择一段文本后：**  
![ShortMode](https://github.com/butaixianran/AI-Translate-and-Search/blob/main/res/img/ShortMode.jpg)

**展开后：**  
![FullMode](https://github.com/butaixianran/AI-Translate-and-Search/blob/main/res/img/FullMode.jpg)


可以通过点击“Setting”调整 排序 和 是否显示。


# 安装
github地址：  
https://github.com/butaixianran/AI-Translate-and-Search

脚本安装地址：  
https://greasyfork.org/zh-CN/scripts/420649-ai-translate-and-search

Chrome类浏览器需要先安装Tampermonkey扩展，才能安装用户脚本。  
https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo


# 创作说明
根据barrer发布的用户脚本改编。  
https://github.com/barrer/tampermonkey-script  

**修改说明：**  
* 添加阿里翻译，阿里云翻译，腾讯翻译，彩云小译
* 重新排序，翻译按照质量排序
* 修改百度翻译为自动识别语言
* 修改沪江英语词典为沪江日语词典
* 增加搜索：知乎，b站，百科，中日英3语wiki，youtube，twitter等
* 去掉大量不常用词典

# AI翻译服务质量
AI翻译服务，质量差异主要体现在：词汇量 和 语言通畅程度 两个方面。尤其是非英语翻译，比如日语翻译。  

综合来看，质量比较好的，是 阿里云翻译 和 金山翻译。然而，通过脚本调用翻译页面，实现无须API的免费翻译时，则各有不便。各翻译服务问题列举如下： 
* **金山翻译：**  翻译质量高，且 单词 翻译提供详细字典。但长文翻译时，通过脚本调用无法分段落。
* **阿里云翻译：**  翻译质量最好。但通过脚本调用无法自动触发翻译，需要手动按一下回车。
* **阿里翻译：** 阿里云翻译的子集，脚本调用便利，但是提供的语种少。日语、韩语均不提供。
* **腾讯翻译：** 词汇量和阿里云翻译一致，但语言组织不如阿里云通畅。
* **搜狗翻译：** 语言通畅程度和阿里云一致，但词汇量略少。
* **百度翻译：** 做得久，名气大，然而质量一般。只是其他AI翻译服务都是刚起步，均未宣传而已。
* **DeepL：** 语言流畅程度和阿里云相当，但日语等语种的词汇量小。而且它是把所有语言先翻译成德语，再把生成的德语翻译成目标语言，因此出错率更高，甚至出现无法翻译的情况。
* **彩云小译：**  日语词汇量较大，能准确翻译 烧卖、美人鱼等其他翻译服务经常翻译错误的娱乐领域词汇。





