---
title: image_To_PDF
date: 2024-03-05 17:32:59
tags:
---
代码如下：
```bash
from PIL import Image
import os

def images_to_pdf(image_paths, output_pdf):
    img_list = []
    for img_path in image_paths:
        img = Image.open(img_path)
        img_list.append(img)

    # 保存为PDF文件
    img_list[0].save(output_pdf, "PDF", resolution=100.0, save_all=True, append_images=img_list[1:])

# 图片路径列表
image_paths = ["IMG_7395.jpg", "IMG_7396.jpg", "IMG_7397.jpg"]  # 替换为你的图片路径

# 输出PDF文件名
output_pdf = "output.pdf"

images_to_pdf(image_paths, output_pdf)
print(f"图片已成功转换为PDF文件：{output_pdf}")
```