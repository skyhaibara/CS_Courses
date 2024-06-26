# 图的遍历

## 描述

图的遍历操作是从图的某一顶点出发，依次访问图中其余顶点，且每个顶点仅被访问一次。请完成无向连通图的深度优先搜索和广度优先搜索。

## 输入

输入数据为多组，每组数据包含多行，第一行为2个整数n（1<=n<=30）,e，n为图的顶点数，e为边数，接下来是e行，每行2个整数，是一个顶点对，代表一条边所依附的两个顶点。例如，下图的输入数据为：

```
5 6
1 2
1 3
2 4
3 4
2 5
4 5
```

![](https://www.tzcoder.cn/acmhome/judge/images/13-05-22.jpg)

## 输出

每个图的深度优先搜索和广度优先搜索序列，每个序列占一行，输出的每个顶点后有一个空格。

## 样例输入

```
3 3
1 2
1 3
2 3
5 6
1 2
1 3
2 4
3 4
2 5
4 5
```

## 样例输出

```
1 2 3 
1 2 3 
1 2 4 3 5 
1 2 3 4 5 
```

## 提示

如题目描述中图所示，顶点值为整型，亦可看为顶点序号，取值从1开始。图中顶点数不超过30个，遍历时由顶点值最小的顶点开始。