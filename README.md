# 微短剧动态漫画
### 记录生成过程
以视频从业者的视角，探索生成动态漫画的工作流，为产品的信息架构打下基础。
——————————————————————————————————————————————————————————————————
* Step1 确定小说主题
* Step2 ChatGPT 写剧本
* Step3 AI 生成角色图
* Step4 构思分镜，批量生成分镜图
* Step5 AI 生成分镜动画
* Step6 剪映自动生成视频
* Step7 制作视频发布
——————————————————————————————————————————————————————————————————
## 确定小说主题
1. 根據小說APP（番茄小说、知乎）排行榜選文
2. 根据对标账号选文，在 YouTube 上搜索 AI 漫畫解說

## ChatGPT 生成剧本

### 本指令公式
```  
角色＋文章類型＋文字風格＋人設＋故事背景＋劇情大網，先列出一個章節目錄
```
* 1. 角色：你是一個頂級的網絡爽文作家
* 2. 文章類型：都市現代修仙文、古風修仙情感文、 青春校園喜劇、懸疑推理文等等
* 3. 文字風格：一般複製一段參考視頻的腳本或者小說內容。可以使用 `YouTube` -> `视频转文案` 
* 4. 人設：比如男女主是修仙者/學生/程序員等
* 5. 故事背景：比如在地球、在學校、在末世
* 6. 劇情大綱：一個關鍵詞
![Snipaste_2023-12-12_10-15-20](https://github.com/qingqing-ux/Short-play-generation/assets/107176473/8c5934e8-df42-40a7-b728-1cac84f8ad88)

#### 提示 ChatGPT 加入对话情节
```  
將第一章展開寫，大概2000字，有對話情節，並且加入相應的場景描述
```
#### 提示 ChatGPT 将章节展开

* 1. 每章都要發生什麼劇情内容          
* 2. 主角都要遇到什麼人
* 3. 產生了什麼樣的對話 

## 确定绘图风格
...

## 生成角色图
借助 ChatGPT 给出角色体型、容貌、服饰和发型等的建议
```
我要替这个故事制作角色概念草图，请你帮我设计一下女孩和爷爷这两个角色，包含他们的体型、容貌、服饰和发型等。
```
进一步转成 Midjourney 的 Prompts，可以附上一个 Prompt 范例让 ChatGPT 作为参考
```
好，接着我要请你把女孩和爷爷的角色描述改写成两个 Midjiourney Prompts (使用英文)，格式类似于下面这个句子：A little girl with light brown short wavy curly hair and blue eyes。
```

### 制作挑战
让角色维持外观的一致性，贯穿整部漫画。手部容易变形。

#### Tips
1. 角色设计图， character sheet， white background
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

#### Tips
1. 使用工具[AutoJourney](https://www.pika.art/)  -> ` Add to Chrome` .這個工具可以支持批量发送 Prompt,自动排队，自动放大，自动下载。


## 生成分镜动画
[Pika Labs](https://www.pika.art/) 它跟 Midjourney 一样是在 Discord 的平台上运作,可以把 Midjourney 的提示文字直接拿來使用，

```
etro Ghibli style, wide-angle view of a 19th-century English pasture at early morning. clear sky. sheep grazing. -ar 16:9 -fps 24 
```
### 制作挑战
动画时长较短，通常只有 3~4s

#### Tips
1. 注意电影独有的参数 -fps 24
2. 可以重复送出算图的請求，让 Pika Lab s一次生成多一点影片
3. 使用 [FinalFrame](https://finalframe.net/dev/) 截取取出影片的最後一張画面，把它当成下一段动画的初始影像，延伸想要的动画長度

## 剪映自动生成视频
剪映出品的`文字成片`功能，可以根据文案`自动配音`、`配画面`，生成视频
可以使用 AI 生成的图片替换视频中不符合要求的画面，这样做的好处是不需要一個個手動的去对齐画面和语音


## 工具合集
1. 免费生图工具  https://leonardo.ai/
2. Photopea  https://www.photopea.com/ 
3. 画质提升网站  https://arc.tencent.com/en/ai-demos/imgRestore
4. 线上抠图网站  https://www.remove.bg/
5. Pika Labs  https://www.pika.art/
6. Runway  https://runwayml.com/
7. FinalFrame  https://finalframe.net/dev/
8. AutoJourney  https://www.pika.art/
