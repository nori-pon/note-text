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
