
[206. Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/)

**题目描述**


>输入一个链表，反转链表后，输出链表的所有元素。

#三指针滑动pPrev -> pNode -> pNext;
-------
通常我们想到的就是单个指针同时滑动
比如当前节点pNode所处的位置如下
>pPrev -> pNode -> pNext;
我们先保存原来的下一个指针位置，要不然翻转后其next会指向pPrev，从而丢失指向pNext的指针
接着反转指针，
然后下面指针同步后移，以便处理后面的指针
