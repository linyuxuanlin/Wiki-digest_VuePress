# 删除 GitHub 仓库中某个文件夹

## 问题来源

在本地仓库上传到 GitHub 时，忘记忽略某个文件夹，直接 push 到远程仓库了。  
如何在保留本地文件夹的同时，删除 GitHub 仓库中的文件夹？

## 解决方法

```bash
$ git pull origin main        # 先将远程仓库里面的项目拉取下来
$ dir                           # 查看有哪些文件夹
$ git rm -r --cached target     # 删除名字为 target 的文件夹
$ git commit -m '删除了 target'  # 添加操作说明并提交
```

## 参考与致谢

- [删除 GitHub 中某个文件夹](https://blog.csdn.net/wudinaniya/article/details/77508229)

<br />

<br />

> 文章作者：**Power Lin**  
> 原文地址：<https://digest.wiki-power.com>  
> 版权声明：文章采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by/4.0/deed.zh) 协议，转载请注明出处。
