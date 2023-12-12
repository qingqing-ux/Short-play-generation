# 微短剧动态漫画
### 记录生成过程
以视频从业者的视角，探索生成动态漫画的工作流，为产品的信息架构打下基础。

## 确认小说主题

## 构思分镜
分镜主要是用来设计画面的布局，展现角色的动作和情绪，以及控制故事整体的节奏。 这个环节可以借助 ChatGPT ，将故事大纲丢给它，ChatGPT 就会设计好每个画格的场景和摄影角度。
1. 故事场景
2. 角度行动
3. 摄影角度
```  
我想要请你替以下这个动画剧情设计六个分镜。每个分镜要具体说明故事场景、角色行动、 摄影角度。以下是剧情内容： 地点是19世纪英国的一个小乡村，有个女孩正在牧场中工作，此时她在远方看到爷爷正在返家的路上，于是女孩露出了开心的笑容。
```

## 确定绘图风格
...

## 制作角色概念草图
借助 ChatGPT 给出角色体型、容貌、服饰和发型等的建议
```
我要替这个故事制作角色概念草图，请你帮我设计一下女孩和爷爷这两个角色，包含他们的体型、容貌、服饰和发型等。
```
进一步转成 Midjourney 的 prompts，可以附上一个 Prompt 范例让 ChatGPT 作为参考
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

## AI 动画
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



## 工具合集

1. Photopea  https://www.photopea.com/ 
2. 画质提升网站  https://arc.tencent.com/en/ai-demos/imgRestore
3. 线上抠图网站  https://www.remove.bg/
4. Pika Labs  https://www.pika.art/
5. Runway  https://runwayml.com/
6. FinalFrame  https://finalframe.net/dev/






### 手动安装

1. 在 [Latest Release](https://github.com/yetone/openai-translator/releases/latest) 页面下载以 `.msi` 结尾的安装包
2. 下载完成后双击安装包进行安装
3. 如果提示不安全，可以点击 `更多信息` -> `仍要运行` 进行安装

### Visual Studio Code
* TypeScript
* Example Code
    * Chrome Storage


Run watch mode.

type `Ctrl + Shift + B`
