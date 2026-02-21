```mermaid
graph TB
%%{
  init:{
    'theme':'base',
    'themeVariables': {
      'primaryColor': '#0000ff',
      'primaryTextColor': '#ffffff',
      'primaryBorderColor': '#0000ff',
      'lineColor': '#0000ff',
      'secondaryColor': '#0000ff',
      'tertiaryColor': '#ffffff'
    },
    'themeCSS':" .klass2 .nodeLabel,.klass3 .nodeLabel{ line-height: 1.6; font-weight: 900; display:flex; justify-content:center; align-items:center; text-align:center; overflow: visible;} .klass3 .nodeLabel{margin:0.4em}",
    'flowchart':{
     'rankSpacing' : 80,
     'nodeSpacing' : 80,
     'subGraphTitleMargin':{
      'top': 40,
      'bottom': 0
      }
   }
   }
}%%

    subgraph katachi
    direction TB
        M["四角"]:::klass2
        I[/"三角"\]:::klass2
        U(("丸")):::klass3
        F{"ひし形"}:::klass2
    end

    style satori stroke-width:10px
    classDef klass2,klass3 stroke-width:10px,font-size:96px
    classDef subGraphTitle color:transparent
    class satori,satorii subGraphTitle

```

---


- TD	上 → 下
- BT	下 → 上
- LR	左 → 右
- RL	右 → 左

- A["text"] 四角
- A[/""text\] 三角
- A(("text")) 丸
- A{"text"} ひし形
- A[/"text"/] 平行四辺形
- A["text"/] 逆向き平行四辺形（環境による）

- 'rankSpacing': 80 縦の間隔
- 'nodeSpacing': 80 横の間隔





