---
title: Google AI local deployment
date: 2024-03-03 22:36:57
tags:
---
##下载安装ollama客户端
[下载地址](https://ollama.com/download)

普通7B版 安装指令：（适合8G显存）
```bash
$ ollama run gemma:7b
```

如果你是第一次部署，它会自动下载！

7B的全量版本：（需要16G左右的显存）
```bash
$ ollama run gemma:7b-instruct-fp16
```
2B轻量版：（适合CPU会低配电脑安装）
```bash
$ ollama run gemma:2b
```

