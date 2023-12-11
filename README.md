# Short-play-generation-record
### 记录生成过程
以视频从业者的视角探索生成动态漫画工作流，为产品的信息架构打下基础

## 构思分镜
分鏡主要是用来设计画面的布局，展现角色的动作和情绪，以及控制故事整體的節奏。
这个环节可以借助 ChatGPT ，将故事大纲丢给它，ChatGPT 就會設計好每個畫格的場景和攝影角度。
```
我想要請你替以下這個動畫劇情設計六個分鏡。每個分鏡要具體說明故事場景、角色行動、 攝影角度。以下是劇情內容：
地點是19世紀英國的一個小鄉村，有個女孩正在牧場中工作，此時她在遠方看到爺爺正在返家的路上，於是女孩露出了開心的笑容。
```

## 确定绘图风格
...

## 制作角色概念草图
借助 ChatGPT 给出角色體型、容貌、服飾和髮型等的建议
```
我要替這個故事製作角色概念草圖，請你幫我設計一下女孩和爺爺這兩個角色，包含他們的體型、容貌、服飾和髮型等。
```
進一步轉成 Midjourney 的 prompts，可以附上一個 Prompt 範例讓 ChatGPT 作為參考
```
好，接著我要請你把女孩和爺爺的角色描述改寫成两個 Midjiourney Prompts (使用英文)，格式類似於下面這個句子：A little girl with light brown short wavy curly hair and blue eyes。
```

## 制作挑战
用 AI 製作漫畫最大的挑戰就是要讓角色維持外觀的一致性，賈穿整部漫畫

* 常见技巧
     * 角色设计图， character sheet， white background
```
Retro Ghibli style， a young girl with golden hair tied back into a simple braid，wearing a humble dress， character sheet， white background --niji 5
```
     * 画布扩充， 人物服饰维持一致风格
```
full body， turnaround
```
     *  [提升图片画质](https://arc.tencent.com/en/ai-demos/imgRestore) 
     *  [去除图片背景](https://www.remove.bg/zh)
     *  [提升图片画质](https://arc.tencent.com/en/ai-demos/imgRestore) 
     



### 手动安装

1. 在 [Latest Release](https://github.com/yetone/openai-translator/releases/latest) 页面下载以 `.msi` 结尾的安装包
2. 下载完成后双击安装包进行安装
3. 如果提示不安全，可以点击 `更多信息` -> `仍要运行` 进行安装
4. 开始使用吧！
5. 


## Setup

```
npm install
```

## Import as Visual Studio Code project

...

### Visual Studio Code
* TypeScript
* Example Code
    * Chrome Storage


Run watch mode.

type `Ctrl + Shift + B`
