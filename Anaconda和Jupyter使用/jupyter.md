# Jupyter

>Jupyter notebook（http://jupyter.org/） 是一种 Web 应用，能让用户将说明文本、数学方程、代码和可视化内容全部组合到一个易于共享的文档中。

## 安装

. 安装 Jupyter 的最简单方法是使用 Anaconda。该发行版附带了 Jupyter notebook。你能够在默认环境下使用 notebook。
要在 conda 环境中安装 Jupyter notebook，在conda终端使用命令（以下所有命令是指conda的终端Anaconda Prompt）：
> conda install jupyter notebook

## 启动

. 启动 notebook 服务器，在终端中输入： jupyter notebook。在浏览器中打开notebook页面地址：http://localhost:8888 

### 如何快速使用

* 安装环境自动关联包
> conda install nb_conda

该包可以将conda中创建的环境自动关联到你的notebook中。我们可以对应conda中的环境，就知道这些环境对应conda中的环境列表。用 conda env list 就可以列出你创建的所有环境。

* 在Anaconda终端安装代码自动补全包
> conda install pyreadline

### ipynb转为html格式
> jupyter nbconvert --to html notebook.ipynb
