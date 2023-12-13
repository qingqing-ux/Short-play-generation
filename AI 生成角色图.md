# 复刻热门漫画
找了一段B站热门漫画[我家师傅超凶哒](http://ryt0q68hc.hn-bkt.clouddn.com/%E8%A7%86%E9%A2%91/%E6%88%91%E5%AE%B6%E5%B8%88%E7%88%B6%E8%B6%85%E5%87%B6%E5%93%92.mp4) ，从这段视频中获得`角色＋文章类型＋文字风格＋人设＋故事背景＋剧情大纲`。整体画风需要靠近原片的二次元风格。

## 生成角色图
借助 ChatGPT 给出角色体型、容貌、服饰和发型等的建议。也可以选取喜欢的角色图，利用 AI 反推关键词。

### 女主角静态图
#### Text to lmage
1girl,solo,(masterpiece, best quality:1.2)bare shoulders,front,look down at,(close-up:1.1),yellow hair,hairpin,eyelashes,eyeshadow,(hair over one eye:1.1),(long hair:1.1),(head_down:1.2),look below with your eyes,holding a teacup,teacup,smile,simple background,military,((wash painting)),((ink s...)),purple long skirt

Negative prompt: easynegative,lowres,bad anatomy,deformed,text,error,cropped,watermark,worst quality,low quality,normal quality,jpegartifacts,signature,watermark,username

Steps: 25, Sampler: DPM++ 3M SDE Karras, CFG scale: 7, Seed: 1122334, Size: 1024x648, Model hash: c35e1054c0, Model: mistoonAnime_v20, Clip skip: 2, Eta: 0.67, Version: 1.7.0

#### Generated
[女主第一幕](http://ryt0q68hc.hn-bkt.clouddn.com/%E8%A7%86%E9%A2%91/%E6%88%91%E5%AE%B6%E5%B8%88%E5%82%85%E8%B6%85%E5%87%B6%E5%93%92%E5%A5%B3%E4%B8%BB/%E5%A5%B3%E4%B8%BB%E7%AC%AC%E4%B8%80%E5%B9%95.jpeg)

[女主第二幕](http://ryt0q68hc.hn-bkt.clouddn.com/%E8%A7%86%E9%A2%91/%E6%88%91%E5%AE%B6%E5%B8%88%E5%82%85%E8%B6%85%E5%87%B6%E5%93%92%E5%A5%B3%E4%B8%BB/%E5%A5%B3%E4%B8%BB%E7%AC%AC%E4%BA%8C%E5%B9%95%20%281%29.jpeg)

### 制作挑战
让角色维持外观的一致性，贯穿整部漫画。手部容易变形。

#### Tips
1. 画布扩充， 人物服饰维持一致风格 
```
full body， turnaround
```
 
## 生成分镜动画
[Pika Labs](https://www.pika.art/) 它跟 Midjourney 一样是在 Discord 的平台上运作,可以把 Midjourney 的提示文字直接拿來使用，

#### Image + prompt
Prompt: The girl spoke and bowed her head,Movie lens translation 

#### Generated

[女主第一幕动画](http://ryt0q68hc.hn-bkt.clouddn.com/%E8%A7%86%E9%A2%91/%E6%88%91%E5%AE%B6%E5%B8%88%E5%82%85%E8%B6%85%E5%87%B6%E5%93%92%E5%A5%B3%E4%B8%BB/%E5%A5%B3%E4%B8%BB%E7%AC%AC%E4%B8%80%E5%B9%95%E5%8A%A8%E7%94%BB.mp4) 

[女主第二幕动画](http://ryt0q68hc.hn-bkt.clouddn.com/%E8%A7%86%E9%A2%91/%E6%88%91%E5%AE%B6%E5%B8%88%E5%82%85%E8%B6%85%E5%87%B6%E5%93%92%E5%A5%B3%E4%B8%BB/%E5%A5%B3%E4%B8%BB%E7%AC%AC%E4%BA%8C%E5%B9%95%E5%8A%A8%E7%94%BB%20%281%29.mp4) 


### 制作挑战
动画时长较短，通常只有 3~4s

#### Tips
1. 注意电影独有的参数 -fps 24
2. 可以重复送出算图的請求，让 Pika Labs一次生成多一点影片
3. 使用 [FinalFrame](https://finalframe.net/dev/) 截取取出影片的最后一张画面，把它当成下一段动画的初始影像，延伸到想要的动画長度。
