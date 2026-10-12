# topopt88

Andreassen 等人 2011 年论文配套的 88 行 MATLAB 拓扑优化代码，用于学习二维 SIMP 拓扑优化。

`top88.m` 从 [DTU TopOpt 官方页面](https://www.topopt.mek.dtu.dk/apps-and-software/efficient-topology-optimization-in-matlab)下载并原样保存，包含原作者署名和免责声明。

## 运行

将 `top88.m` 所在文件夹设为 MATLAB 当前文件夹，在命令窗口运行官方示例：

```matlab
top88(120,40,0.5,3.0,3.5,1)
```

程序计算半 MBB 梁，输出迭代次数、柔度目标值、材料体积分数和设计变化量，并显示材料密度分布。

## 参数

```matlab
top88(nelx,nely,volfrac,penal,rmin,ft)
```

| 参数 | 含义 | 示例值 |
| --- | --- | --- |
| `nelx` | 水平方向的单元数 | 120 |
| `nely` | 竖直方向的单元数 | 40 |
| `volfrac` | 材料体积分数 | 0.5 |
| `penal` | SIMP 惩罚指数 | 3.0 |
| `rmin` | 过滤半径，以单元间距为单位 | 3.5 |
| `ft` | 过滤类型：1 为灵敏度过滤，2 为密度过滤 | 1 |

## 出处

Erik Andreassen, Anders Clausen, Mattias Schevenels, Boyan S. Lazarov, Ole Sigmund (2011).
*Efficient topology optimization in MATLAB using 88 lines of code*.
*Structural and Multidisciplinary Optimization*, **43**(1), 1–16.

- [论文 DOI：10.1007/s00158-010-0594-7](https://doi.org/10.1007/s00158-010-0594-7)
- [DTU 官方下载页面](https://www.topopt.mek.dtu.dk/apps-and-software/efficient-topology-optimization-in-matlab)
- [DTU 原始 top88.m 文件](https://www.topopt.mek.dtu.dk/-/media/subsites/topopt/apps/dokumenter-og-filer-til-apps/top88.m)

代码用于教学，权利声明以 `top88.m` 末尾的原作者说明为准。
