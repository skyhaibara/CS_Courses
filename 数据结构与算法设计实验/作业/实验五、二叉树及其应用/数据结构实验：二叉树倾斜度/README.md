# 数据结构实验：二叉树倾斜度

## 描述

求一棵二叉树的倾斜度，其中一个节点的倾斜度定义为“左子树元素之和”与“右子树元素之和”差的绝对值（空节点的元素值为0），二叉树的倾斜度定义为所有节点的倾斜度之和。

二叉树节点定义如下：

```c
struct TreeNode {
    int val;
    struct TreeNode *left;
    struct TreeNode *right;
};
```

题目部分代码已经完成，您只需要补充并提交以下函数：

`int findTilt(struct TreeNode* root);//root为根结点指针，返回倾斜度之和`

## 输入

输入为若干个整数（不超过512）表示一棵二叉树顺序表示时的结点元素值，其中0表示二叉树对应结点为空。输入以-1结束。 

## 输出

输出二叉树的倾斜度。

## 样例输入

```
1 2 3 -1
```

## 样例输出

```
1
```