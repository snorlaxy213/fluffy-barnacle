# fluffy-barnacle
兴趣使然的爬虫项目

使用技术：
- Python版本：Python 3.10.4


问题总结：
> Python 引入requests模块后VsCode出现问题提示 “could not be resolved”

1. pip list 查看是否安装了 requests 包

   ```shell
   pip list
   ```

    如表示已经安装 requests 包，如果没安装请跳到步骤二，如果已安装请跳到步骤三 

2. 安装 request 包

   ```shell
   pip install requests
   ```

3. 在当前项目的.vscode目录中，修改settings.json文件

   ```shell
   "python.analysis.extraPaths": [
   	"./py_src"
   ]
   ```

    将./py_src换成安装路径( 路径可以在cmd命令行中使用where python指令找到)
   例如C:\\Users\\XXX\\AppData\\Local\\Programs\\Python\\Python310\\Lib\\site-packages

> pip install 下载速度慢解决方法

```shell
# 配置镜像源
pip config set global.index-url https://pypi.doubanio.com/simple/
# 配置信任主机名
pip config set global.trusted-host pypi.doubanio.com
```

