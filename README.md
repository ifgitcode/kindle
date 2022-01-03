## 项目说明

这是一个使用 Python 语言编写的小工具，用于将 Kindle 标注笔记文件 `My Clippings.txt` 转换成 html 文件。fork 自 [muzi502/kindle](https://github.com/muzi502/kindle)预览网站 [github.io/kindle/](https://ifgitcode.github.io/kindle/)

## 使用说明

- 1、从 kindle 中拷贝出标注文件 `My Clippings.txt`，重命名为 source.txt。
- 2、下载本项目源码，使用你的 source.txt 进行替换。
- 3、在 Python3 环境下执行 `python3 kindle.py` 指令，等待生成网页文件。

```shell
git clone https://github.com/muzi502/kindle
cd kindle
cat /your/path/My Clippings.txt > source.txt
python3 kindle.py
```

## 相关脚本

在 Windows 环境下可以使用 .bat 脚本来自动复制 `My Clippings.txt` 文件到相应的位置。根据自己的环境修改相应的变量即可。

```powershell
set src="G:\documents\My Clippings.txt" 
set dist=F:\MykindleText\kindle-master\source.txt
set pngsrc=G:\*.png
set pngdist=F:\MykindleText\kindle-master
copy /Y  %src% %dist%
copy /Y %pngsrc% %pngdist%
```
