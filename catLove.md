```mermaid
graph LR
    %% 全体の色の設定
    classDef catStyle fill:#D9B44A,stroke:#75B1A9,stroke-width:7px,color:#ffffff,font-size:40px;

    %% ノードの定義
    node1[/"🙀"/]:::catStyle
    node2["♥"]:::catStyle
    node3[/2.22\]:::catStyle
    node4((ねこ)):::catStyle
    node5{nya}:::catStyle

   %% 透明な線で横に並べる
    node1 ~~~ node2 ~~~ node3 ~~~ node4 ~~~ node5

```

```mermaid
graph LR
%%{init: {
    "theme": "base",
    "themeVariables": {
    "primaryColor": "#D9B44A",
    "primaryTextColor": "#ffffff",
    "lineColor": "#75B1A9",
    "tertiaryColor": "#D9B44A"
}}%%

    classDef catStyle fill:#D9B44A,font-size:40px,padding:10px,stroke:#75B1A9,stroke-width:7px,color:#ffffff,line-height:1.2,display:flex,ustify-content:center,align-items:center,text-align:center;

    node1[/"🙀"/]:::catStyle
    node2["♥"]:::catStyle
    node3[/2.22\]:::catStyle
    node4((ねこ)):::catStyle
    node5{nya}:::catStyle

    node1 ~~~ node2 ~~~ node3 ~~~ node4 ~~~ node5
```

```
fill-------------内側の塗りつぶし 背景色
stroke-----------枠線の色 図形を囲んでいる線   
stroke-width-----枠線の太さ 線の厚み（pxで指定）
color------------文字の色	
```

```mermaid
graph TD
    %% 丸のパーツだけ大きくする設定
    classDef largeCatCircle fill:#FE7A47,stroke:#F5CA99,stroke-width:12px,color:#D8412F,font-weight:bold,font-size:120px,min-width:800px,min-height:800px,padding:20px;
    A(("🐈")):::largeCatCircle

    classDef myStyle fill:#FE7A47,stroke:#F5CA99,stroke-width:8px,color:#D8412F,font-weight:bold,font-size:24px;
    B[/"2026/02/22"/]:::myStyle

    %% 透明な矢印でつなぐ
    A ~~~ B
```

```mermaid
graph TD
%%{init: {"theme": "base", "themeCSS": ".nodeLabel { display: flex; justify-content: center; align-items: center; }"}}%%
    %% 猫
    classDef largeCatCircle fill:#FE7A47,stroke:#F5CA99,stroke-width:12px,color:#D8412F,font-weight:bold,font-size:120px,min-width:500px,min-height:800px,padding:20px;
    A(("🐈")):::largeCatCircle

    classDef myStyle fill:#FE7A47,stroke:#F5CA99,stroke-width:8px,color:#D8412F,font-weight:bold,font-size:24px;
    B[/"2026/02/22"/]:::myStyle

    %% 透明な矢印でつなぐ
    A ~~~ B
```


```mermaid
graph LR
    %% 全体の初期化設定
    %%{init: {"theme": "base", "themeCSS": ".nodeLabel { display: flex; justify-content: center; align-items: center; }"}}%%

    %% 猫
    classDef catStyle fill:#FE7A47,stroke:#F5CA99,stroke-width:15px,font-size:150px,min-width:350px,min-height:350px;
    
    %% キラキラ
    classDef sparkStyle fill:#FFB300,stroke:#F5CA99,stroke-width:5px,font-size:40px,min-width:80px,min-height:80px;

    %% ノード定義
    L{"✨"}:::sparkStyle
    C(("🐈")):::catStyle
    R{"✨"}:::sparkStyle

    %% 横に並べる（透明な線でつなぐ）
    L ~~~ C ~~~ R

```

```
%% は通常、コメントアウト
%%{init: ...}%% は特別な意味を持つ 「ディレクティブ（設定指示）
```

---

### 書き方メモ

```
TD	上 → 下
BT	下 → 上
LR	左 → 右
RL	右 → 左
```

```
A["text"] 四角
A[/"text"\] 三角
A(("text")) 丸
A{"text"} ひし形
A[/"text"/] 平行四辺形
A["text"/] 逆向き平行四辺形（環境による）
```

` subgraph `：内部で使う名前（英数字推奨）
- ` subgraph katachi ` ：katachiが表示名になる
- ` end `：開いたら閉じる

```
rankSpacing　: 80 縦の間隔
nodeSpacing　: 80 横の間隔
```

### color

```
#000000（黒）
#ffffff（白）
#ff0000（赤）
#00ff00（緑）
#0000ff（青）
```
rgb / rgba
```
rgb(255, 0, 0)        :R,G,B
rgba(255, 0, 0, 0.5)  :R,G,B,A（透明度）

A = Alpha 値は0～1
0 → 完全透明
1 → 完全不透明
0.5 → 半透明

```






