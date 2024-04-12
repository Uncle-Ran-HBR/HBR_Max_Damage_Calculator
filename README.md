# 红烧天堂（炽焰天穹）最大伤害计算器后端发布页

此仓库作为红烧天堂（炽焰天穹）最大伤害计算器后端发布页。

## 快速开始

### 工具下载

从[这里](https://github.com/Uncle-Ran-HBR/HBR_Max_Damage_Calculator/releases)下载工具，当前仅支持x86-64架构的 Windows 10/11 电脑运行。

![image.png](https://s2.loli.net/2024/04/12/awySpGMQLusrRXv.png)

下载后解压缩到任意路径。

### 在命令行打开工具

以 PowerShell 命令行为例，首先在资源管理器中进入工具解压目录，并复制路径。

![image.png](https://s2.loli.net/2024/04/12/ZI8aDyCQUdwLqm6.png)

![image.png](https://s2.loli.net/2024/04/12/5BnhOkuvgLlsEN7.png)

按下 Win + S 键弹出搜索框，搜索 PowerShell 。

![image.png](https://s2.loli.net/2024/04/12/ZOAmizao1In4Mxs.png)

点击打开。

![image.png](https://s2.loli.net/2024/04/12/s8piwVmueFS6AUY.png)

输入 cd 后面加一个空格。

![image.png](https://s2.loli.net/2024/04/12/JeNmskf6I9uYhEn.png)

再点击鼠标右键，应该会把之前复制的路径带过来。

![image.png](https://s2.loli.net/2024/04/12/vLOdPfRWuk7ynIl.png)

点击回车，会发现路径切换过来了。

![image.png](https://s2.loli.net/2024/04/12/XylZKpgGeJ5wmL4.png)

输入 h ，并按下 Tab 会自动补全。

![image.png](https://s2.loli.net/2024/04/12/F52zfUiCS8pyGon.png)

![image.png](https://s2.loli.net/2024/04/12/oBxgOD7YhJ2mzfc.png)

我们测试下能否查看版本号，输入空格，然后输入 -v ，回车，如果出现版本号，说明工具可以使用。

![image.png](https://s2.loli.net/2024/04/12/jeX5w8o4Wvm29T6.png)

如图所示，显示了版本号为0.8。

接下来我们选择一个常规场景计算一下伤害。

请将以下命令复制，然后到 PowerShell 中按右键粘贴。

```ps
.\hbr_max_damage_calculator.exe --element "火" --including "西装Tama,红梢" --excluding "浴衣500,暗惠" --need_survive 
```

![image.png](https://s2.loli.net/2024/04/12/28GgCrOvyWX47ZD.png)

这段命令的意思是，计算弱火Boss（默认弱点是250%倍率），组队中必带西装Tama和红梢，并且不带浴衣500和暗惠，同时要求队伍中必须至少有一个生存类角色（奶或T，奶量不能比月歌低，笑）的情况下，伤害最高的编队。

点击回车执行，然后等待工具运行成功即可。

![image.png](https://s2.loli.net/2024/04/12/UfwLW3Y6l85XJep.png)

可以看到工具不仅计算了火队，把跨属性打工的雷队和暗队也一起算上了，并根据队伍做了排序，Nice。

同时我们在工具目录发现了一个文件 temp.csv ，这个文件储存了计算结果，我们打开查看。

![image.png](https://s2.loli.net/2024/04/12/flb3KSNxHXYvaCe.png)

![image.png](https://s2.loli.net/2024/04/12/gvbNTKEcFGh7RDw.png)

很清晰，给兰叔点赞！
