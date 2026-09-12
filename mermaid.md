# Mermaid for diagrams and flow charts

[cheatsheet](https://jojozhuang.github.io/tutorial/mermaid-cheat-sheet/)

## Click
- Using anchor tag `<a>`  of html (which works in VS code markdown preview)
- Using `click` of mermaid (Did not work in VS code markdown preview) 

### Opening Relative Paths (Local Files)
If you want a node to open another file in your local directory or repository (like a sub-diagram or documentation page), use a relative file path.

```mermaid
flowchart LR
    Main[High Level Process] --> Detail[View Step 3 Details]

    click Detail href "#step-3-detailed-breakdown" "Jump to Step 3 Specs"

```
#### with 
```mermaid
flowchart LR
    Main[High Level Process] --> Detail[<a href="#step-3-detailed-breakdown" alt="Jump to Step 3 Specs">View Step 3 Details</a>]
```

```mermaid
flowchart TD
    Start[README] --> Sub[Mermaid]
    
    click Start href "./README.md" "See read me for all the tools for documentation"
```



```mermaid
flowchart TD
    Start[README] --> Sub[Mermaid]
    
    click Start href "./README.md" "See read me for all the tools for documentation"
```

```mermaid
flowchart TD
    Start[README] --> Sub[Mermaid]
    
    click Start href "./README.md" "See read me for all the tools for documentation"
```

```mermaid
flowchart TD
    Start[README] --> Sub[Mermaid]
    
    click Start href "./README.md" "See read me for all the tools for documentation"
```


### Step 3: Detailed Breakdown