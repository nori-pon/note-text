```mermaid
%%{
  init:{
    'theme':'base',
    'themeVariables': {
      'secondaryColor': '#1d1d3d',     %% 外側の四角の色
      'primaryColor': '#547792',       %% 中の丸の色
      'primaryBorderColor': '#1A3263', %% 丸の枠線
      'primaryTextColor': '#FAB95B'    %% 中の文字の色
    }
  }
}%%
flowchart LR
    subgraph outer [" "]
        direction LR
        node_pi(("pi")):::hugeText
    end

    %% スタイルの調整
    classDef hugeText fill:#547792,stroke:#1A3263,font-size:100px,stroke-width:10px,color:#FAB95B;
    
    %% サブグラフ
    style outer fill:#1d1d3d,stroke:#F6CE71,stroke-width:4px
```

---

```mermaid
graph LR
    classDef aStyle fill:#547792,stroke:#1A3263,font-size:200px,stroke-width:20px,color:#FAB95B;

    A(("pi")):::aStyle
```

---

```mermaid
%%{
  init:{
    'theme':'base',
    'themeVariables': {
      'secondaryColor': '#1d1d3d',     %% 外側の四角の色
      'primaryColor': '#547792',       %% 中の丸の色
      'primaryBorderColor': '#1A3263', %% 丸の枠線
      'primaryTextColor': '#FAB95B'    %% 中の文字の色
    }
  }
}%%
flowchart LR
    subgraph outer [" "]
        direction LR
        node_pi1(("4")):::hugeText
        node_pi2(("o")):::hugeText
        node_pi3(("4")):::hugeText
        node_pi4(("pi")):::hugeText
    end

    %% スタイルの調整
    classDef hugeText fill:#547792,stroke:#1A3263,font-size:100px,stroke-width:10px,color:#FAB95B;
    
    %% サブグラフ
    style outer fill:#1d1d3d,stroke:#F6CE71,stroke-width:6px
```

---

```mermaid
%%{
  init:{
    'theme':'base',
    'themeVariables': {
      'secondaryColor': '#1d1d3d',     %% 外側の四角の色
      'primaryColor': '#547792',       %% 中の丸の色
      'primaryBorderColor': '#1A3263', %% 丸の枠線
      'primaryTextColor': '#FAB95B'    %% 中の文字の色
    }
  }
}%%
flowchart LR
    subgraph outer [" "]
        direction LR
        node_pi1(("猫")):::hugeText
        node_pi2(("猫")):::hugeText
        node_pi3(("猫")):::hugeText
        node_pi4(("猫")):::hugeText

        node_pi1 ~~~ node_pi2 ~~~ node_pi3 ~~~ node_pi4
    end

    %% スタイルの調整
    classDef hugeText fill:#547792,stroke:#1A3263,font-size:40px,stroke-width:10px,color:#FAB95B,min-width:50px,min-height:90px,padding:90px;
    
    %% サブグラフ
    style outer fill:#1d1d3d,stroke:#F6CE71,stroke-width:6px
```

---

```mermaid
%%{
  init:{
    'theme':'base',
    'themeVariables': {
      'secondaryColor': '#1d1d3d',     %% 外側の四角の色
      'primaryColor': '#547792',       %% 中の丸の色
      'primaryBorderColor': '#1A3263', %% 丸の枠線
      'primaryTextColor': '#FAB95B'    %% 中の文字の色
    }
  }
}%%
flowchart LR
    subgraph outer [" "]
        direction LR
        node_pi1(("★")):::hugeText
        node_pi2(("☆")):::hugeText
        node_pi3(("★")):::hugeText
        node_pi4(("☆")):::hugeText

        node_pi1 ~~~ node_pi2 ~~~ node_pi3 ~~~ node_pi4
    end

    %% スタイルの調整
    classDef hugeText fill:#547792,stroke:#1A3263,font-size:40px,stroke-width:10px,color:#FAB95B,min-width:50px,min-height:90px,padding:90px;
    
    %% サブグラフ
    style outer fill:#1d1d3d,stroke:#F6CE71,stroke-width:6px
```
