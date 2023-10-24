# Markdown and Mermaid

A test of [**Markdown**](https://www.markdownguide.org/basic-syntax/) and [**Mermaid**](https://mermaid.js.org/syntax/flowchart.html) support in Github

```mermaid
graph TD
    a-->b
    b-->c
    c-->b
    c---d
    subgraph e
    end
    subgraph f
        g---h
    end
    b-->f
```

Same thing, but Left to Right (LR) instead of Top Down (TD):

```mermaid
graph LR
    a-->b
    b-->c
    c-->b
    c---d
    subgraph e
    end
    subgraph f
        g---h
    end
    b-->f
```

A fancier version

```mermaid
graph TD
    a([Hello])-->b((World))
    b-->c[More Words]
    c-->|back at you|b
    c---d[Like So]
    subgraph e[All alone]
    end
    subgraph f[Straight line here]
        g---|here really|h
    end
    b-->f
```


Note I use the [MarkDown Viewer](https://github.com/simov/markdown-viewer) Chrome Extension to preview these files before pushing them to Github. It's a little tricky to setup but there are some instructions at that link. You need to [install it](https://chrome.google.com/webstore/detail/markdown-viewer/ckkdlimhmcjmikdlpkmbgfkaikojcbjk?hl=en) in Chrome, then maybe watch the video, but turn on Mermaid support and enable local file system access. Then open your file by going to **file:///Users/** in the Chrome address bar and locating it from there.