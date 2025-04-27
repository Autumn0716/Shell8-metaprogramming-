# Shell8-metaprogramming-
Build your own GitHub action to run proselint or write-good on all the .md files in the repository. Enable it in your repository, and check that it works by filing a pull request with a typo in it. 构建自己的 GitHub 操作运行 proselint 或 write-good 所有 仓库中的 .md 文件。在您的仓库中启用它，并通过提交包含拼写错误的拉取请求来检查它是否正常工作。

yml文件可在.github/workflows目录里查询.这里不做赘述.
本仓库参考使用[proselint](https://github.com/amperser/proselint)该程序进行检测.

但是目前看来有不少拼写错误其实并不能够有效检测出来,这里不是本仓库的问题,而是proselint本身无法检测.(会误判导致)
举例:
能被检测出来的:
``John is very unique``
无法比较.
不能被检测出来的:

```
preosnna is a god jesk.
Please cancle this task.
click here to tska the operation
JOhn is vry unique.
```
也可使用 write-good 程序,链接在[write-good](https://github.com/btford/write-good).
由于环境虚拟机均使用 Ubuntu 系统以及 python 环境,拉取代码过程也一样,只需要把下载行的 ``proselint``换为 ``write-good``即可.
