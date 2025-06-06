```mermaid
flowchart LR

A[Load PDF<br/>(pymupdf)] --> B[Extract Text<br/>per Page]
B --> C[Split by Chapter<br/>(Regex BAB \\d+)]
C --> D[Clean Text<br/>(remove header, fix hyphen)]
D --> E[Export Cleaned<br/>Text to .txt File]
```
