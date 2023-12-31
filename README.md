# 微短剧-动态漫画
本文主要记录动态漫画的生成过程，以视频从业者的视角，探索生成动态漫画的工作流，为产品的信息架构打下基础。

* Step1 确定小说主题
* Step2 ChatGPT 写剧本
* Step3 AI 生成角色图
* Step4 构思分镜，批量生成分镜图
* Step5 AI 生成分镜动画
* Step6 剪映自动生成视频
* Step7 制作视频发布

## 确定小说主题
1. 根据小说APP（番茄小说、知乎）排行榜选文
2. 根据对标账号选文，在 YouTube 上搜索 AI 漫画解说/动态漫画

## ChatGPT 写剧本

### 指令公式
```  
角色＋文章类型＋文字风格＋人设＋故事背景＋剧情大纲，先列出一個章节目录
```
* 1. 角色：贝拉、贝拉的爷爷、外地音乐商人
* 2. 文章类型：成长故事、家庭情感
* 3. 文字风格：感人、温馨。一般复制一段参考视频的脚本或者小说内容。可以使用 `YouTube` -> `视频转文案` 
* 4. 人设：贝拉，一个勤劳善良的女孩，对小提琴充满热爱。爷爷，一个慈祥的老人，深爱着贝拉。外地音乐商人，一个懂音乐、慷慨乐善好施的人。
* 5. 故事背景：在19世纪英国的小乡村中
* 6. 剧情大纲：一个关键词
```  
现在，假设你是一位顶级网络小说作家，请写一篇以“家庭情感”和“成长故事”为主题的文章，文字风格你可以参考“在19世纪英国的小乡村中，贝拉是一位勤劳的女孩，在牧场里工作。有一天，她看到爷爷驾着马车从市集回来，带着一个包裹和一把古老的小提琴。贝拉因为一直以来都梦寐以求的小提琴而高兴得眼眶泛泪。不久之后，乡村传来了坏消息。一场可怕的瘟疫正在蔓延，许多人被感染，生命岌岌可危。贝拉的爷爷也不幸染病，他的身体变得虚弱，生命的火花摇摇欲坠。治疗所需的药品价格昂贵，贝拉和家人陷入了困境。他们尽力筹集资金，但仍然无法支付得起。贝拉心如刀绞，她感到无助和绝望。”贝拉的人设是勤劳善良的小女孩，对小提琴充满热爱。爷爷的人设是一个慈祥的老人，深爱着贝拉。爷爷也以他的行动表达了对贝拉的深厚的爱，他保留了另一把小提琴，等待适当时机将其交给贝拉。先列出一个章节目录。
``` 
![Frame 1_副本](https://github.com/qingqing-ux/Short-play-generation/assets/107176473/3cae4c7f-c96a-4ea9-b18f-14c4c391347a)


#### 提示 ChatGPT 加入对话情节
```  
将第一章展开写，大概2000字，有对话情节，并且加入相应的场景描述
```
#### 提示 ChatGPT 将章节展开

* 1. 每章都要发生什麽剧情内容          
* 2. 主角都要遇到什麽人
* 3. 产生了什麽样的对话 

## 生成角色图
借助 ChatGPT 给出角色体型、容貌、服饰和发型等的建议。也可以选取喜欢的角色图，利用 AI 反推关键词。
```
我要替这个故事制作角色概念草图，请你帮我设计一下女孩和爷爷这两个角色，包含他们的体型、容貌、服饰和发型等。
```
进一步转成 Midjourney 的 Prompts，可以附上一个 Prompt 范例让 ChatGPT 作为参考
```
好，接着我要请你把女孩和爷爷的角色描述改写成两个 Midjiourney Prompts (使用英文)，格式类似于下面这个句子：A little girl with light brown short wavy curly hair and blue eyes。
```

### 制作挑战
让角色维持外观的一致性，贯穿整部漫画。手部容易变形。

#### 解决方案
1. 角色设计图需要含关键词 `character sheet` ` white background`  
```
Retro Ghibli style， a young girl with golden hair tied back into a simple braid，wearing a humble dress， character sheet， white background --niji 5
```
2. 画布扩充， 人物服饰维持一致风格 
```
full body， turnaround
```
 
## 构思分镜
分镜主要是用来设计画面的布局，展现角色的动作和情绪，以及控制故事整体的节奏。 借助 ChatGPT， 将 `第一章节` -> `分成N个分镜场景` ，它就会设计好每个画格的场景和摄影角度。并进一步转成 Midjourney 的 Prompts。
1. 故事场景
2. 角度行动
3. 摄影角度
```  
我想要请你替以下这个动画剧情设计六个分镜。每个分镜要具体说明故事场景、角色行动、 摄影角度。以下是剧情内容： 地点是19世纪英国的一个小乡村，有个女孩正在牧场中工作，此时她在远方看到爷爷正在返家的路上，于是女孩露出了开心的笑容。
```
### 制作挑战
场景图较多，需要批量生成分镜图

#### 解决方案
1. 使用工具[AutoJourney](https://www.pika.art/)  -> ` Add to Chrome` .這個工具可以支持批量发送 Prompt，自动排队，自动放大，自动下载。


## 生成分镜动画
[Pika Labs](https://www.pika.art/) 它跟 Midjourney 一样是在 Discord 的平台上运作,可以把 Midjourney 的提示文字直接拿來使用，

```
etro Ghibli style, wide-angle view of a 19th-century English pasture at early morning. clear sky. sheep grazing. -ar 16:9 -fps 24 
```
### 制作挑战
动画时长较短，通常只有 3~4s

#### 解决方案
1. 注意电影独有的参数 -fps 24
2. 可以重复送出算图的請求，让 Pika Labs一次生成多一点影片
3. 使用 [FinalFrame](https://finalframe.net/dev/) 截取取出影片的最后一张画面，把它当成下一段动画的初始影像，延伸到想要的动画長度。

## 剪映自动生成视频
剪映出品的`文字成片`功能，可以根据文案`自动配音`、`配画面`，生成视频
可以使用 AI 生成的图片替换视频中不符合要求的画面，这样做的好处是不需要一個個手动的去对齐画面和语音


## 工具合集
1. 免费生图工具  https://leonardo.ai/
2. Photopea  https://www.photopea.com/ 
3. 画质提升网站  https://arc.tencent.com/en/ai-demos/imgRestore
4. 线上抠图网站  https://www.remove.bg/
5. Pika Labs  https://www.pika.art/
6. Runway  https://runwayml.com/
7. FinalFrame  https://finalframe.net/dev/
8. AutoJourney  https://www.pika.art/
