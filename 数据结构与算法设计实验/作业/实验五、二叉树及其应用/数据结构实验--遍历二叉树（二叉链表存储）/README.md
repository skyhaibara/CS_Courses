# 数据结构实验--先序遍历二叉树（二叉链表存储）

## 描述

给定一棵二叉树，以二叉链表存储，要求输出先序遍历该二叉树得到的序列。

部分代码已经给出，请补充完整，提交时请勿包含已经给出的代码。

```cpp
int main()
{
	Bitnode *t;
	int n;
	cin>>n;
	while(n--)
	{
		t=CreatBitree_level();
		preorder(t);
		cout<<endl;
	}
	return 0;
}
```

## 输入

输入数据分为多组，第一行是测试数据的组数n，下面的n行分别代表一棵二叉树。每棵二叉树结点的值均为正整数，数据为0代表当前结点为空，数据为-1代表二叉树数据输入结束，-1不作处理。二叉树的构造按照层次顺序（即第1层1个整数，第2层2个，第3层4个，第4层有8个......，如果某个结点不存在以0代替）。

## 输出

输出每棵二叉树的先序遍历序列，每个结点值之前有一个空格。

## 样例输入

```
2
1 -1
1 2 0 3 -1
```

## 样例输出

```
 1
 1 2 3
```

# 数据结构实验--后序遍历二叉树（二叉链表存储）

## 描述

给定一棵二叉树，以二叉链表存储，要求输出后序遍历该二叉树得到的序列。

部分代码已经给出，请补充完整，提交时请勿包含已经给出的代码。

```cpp
int main()
{
	Bitnode *t;
	int n;
	cin>>n;
	while(n--)
	{
		t=CreatBitree_level();
		postorder(t);
		cout<<endl;
	}
	return 0;
}
```

## 输入

输入数据分为多组，第一行是测试数据的组数n，下面的n行分别代表一棵二叉树。每棵二叉树结点的值均为正整数，数据为0代表当前结点为空，数据为-1代表二叉树数据输入结束，-1不作处理。二叉树的构造按照层次顺序（即第1层1个整数，第2层2个，第3层4个，第4层有8个......，如果某个结点不存在以0代替）

## 输出

输出每棵二叉树的后序遍历序列，每个结点值之前有一个空格。

## 样例输入

```
2
1 -1
1 2 0 3 4 -1
```

## 样例输出

```
 1
 3 4 2 1
```