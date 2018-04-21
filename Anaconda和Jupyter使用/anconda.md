# Anaconda

[官方文档](https://conda.io/docs/user-guide/tasks/index.html)

## 安装

安装过程略 [官网下载](https://www.anaconda.com/download/)

## 包

* conda list  查看你安装的内容
* conda upgrade --all 为了避免后面使用报错，你需要先更新下所有包。
* conda install package_name 安装包,比如conda install pandas，conda install pandas numpy，conda install numpy=1.10
* conda remove package_names 卸载包
* conda update package_name 更新包
* conda update --all 更新所有包

## 环境

* conda create -n env_name package_names 创建环境。
 env_name 是设置环境的名称（-n 是指该命令后面的env_name是你要创建环境的名称），package_names 是你要安装在创建环境中的包名称。比如 conda create -n py3 python=3, conda create -n py python=3.6

* 进入环境
 在 Windows 上，你可以使用 activate my_env进入。在 OSX/Linux 上使用 source activate my_env 进入环境。
* 离开环境
 在 Windows 上，终端中输入：deactivate 在 OSX/Linux 上 输入：source deactivate
* 共享环境
 你可以在你当前的环境中终端中使用 conda env export > environment.yaml 将你当前的环境保存到文件中包保存为YAML文件（包括Pyhton版本和所有包的名称）。命令的第一部分 conda env export 用于输出环境中的所有包的名称（包括 Python 版本）。
 conda env update -f=/path/to/environment.yml 本地使用。
* 列出环境 conda env list
* 删除环境 conda env remove -n env_name