## 功能
ocr识别结果，且不说准确性，换行总是处理不好，如果选择过滤换行，就会误伤一些，如果不去掉换行，又看了难受。  
处理流程：我使用的是utools, 截图ocr并复制，此时剪贴板最上面的就是识别后的内容。  
py监听处理，把结果push到剪贴板。  

### 方案1
快捷键:alt+b  
本地算：算出行的字数，在这个字数左右的行就去掉换行符号。
### 方案2
快捷键:alt+<  
用ai过一下ocr内容，能解决ocr识别的错误问题，解决换行问题，目前用的智谱api

## 使用
* 配置智谱api,配置在.env
* 环境安装: pip install -r .\requirements.txt
* python listener.py

## todo
- [x] 单元测试，保证ocr格式，各个demo正确
- [x] 单元测试，保证图片识别，各个demo正确

