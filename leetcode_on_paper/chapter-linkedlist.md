# LinkedList 链表

## 解题思路

递归，快慢指针，如果有需要添加dummyHead，画图搞清链接。
主要题型：反转、中间节点和合并链表的组合；反转全部，反转部分，K个一组反转

## 典型题目
[ ] [206. 反转链表](https://leetcode-cn.com/problems/reverse-linked-list/)

[ ] [92. 反转链表 II](https://leetcode-cn.com/problems/reverse-linked-list-ii/)

[ ] [25. K 个一组翻转链表](https://leetcode-cn.com/problems/reverse-nodes-in-k-group/)

[ ] [21. 合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists/)

[ ] [23. 合并K个升序链表](https://leetcode-cn.com/problems/merge-k-sorted-lists/)

[ ] [141. 环形链表](https://leetcode-cn.com/problems/linked-list-cycle/)

[ ] [142. 环形链表 II](https://leetcode-cn.com/problems/linked-list-cycle-ii/)

[ ] [160. 相交链表](https://leetcode-cn.com/problems/intersection-of-two-linked-lists/)

[ ] [19. 删除链表的倒数第 N 个结点](https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list/)

[ ] [83. 删除排序链表中的重复元素](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list/)

[ ] [82. 删除排序链表中的重复元素 II](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list-ii/)

[ ] [61. 旋转链表](https://leetcode-cn.com/problems/rotate-list/)

[ ] [24. 两两交换链表中的节点](https://leetcode-cn.com/problems/swap-nodes-in-pairs/)

[ ] [86. 分隔链表](https://leetcode-cn.com/problems/partition-list/)

[ ] [328. 奇偶链表](https://leetcode-cn.com/problems/odd-even-linked-list/)

[ ] [148. 排序链表](https://leetcode-cn.com/problems/sort-list/)

[ ] [234. 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list/)

[ ] [138. 复制带随机指针的链表](https://leetcode-cn.com/problems/copy-list-with-random-pointer/)

[ ] [430. 扁平化多级双向链表](https://leetcode-cn.com/problems/flatten-a-multilevel-doubly-linked-list/)

<div style="page-break-after: always"></div>

## 206. [反转链表](https://leetcode-cn.com/problems/reverse-linked-list/)

### 题目

给你单链表的头节点 head ，请你反转链表，并返回反转后的链表。

**示例1**
输入：head = [1,2,3,4,5]
输出：[5,4,3,2,1]

**示例2**
输入：head = [1,2]
输出：[2,1]

**示例3**
输入：head = []
输出：[]

**提示**
链表中节点的数目范围是 [0, 5000]
-5000 <= Node.val <= 5000
 
**进阶**
链表可以选用迭代或递归方式完成反转。你能否用两种方法解决这道题？

### ✐
<div style="page-break-after: always"></div>

## [92. 反转链表 II](https://leetcode-cn.com/problems/reverse-linked-list-ii/)

### 题目

给你单链表的头指针 head 和两个整数 left 和 right ，其中 left <= right 。请你反转从位置 left 到位置 right 的链表节点，返回反转后的链表 。

**示例1**
输入：head = [1,2,3,4,5], left = 2, right = 4
输出：[1,4,3,2,5

**示例2**
输入：head = [5], left = 1, right = 1
输出：[5]

**提示**
* 链表中节点数目为 n
* 1 <= n <= 500
* -500 <= Node.val <= 500
* 1 <= left <= right <= n
 
**进阶**
你可以使用一趟扫描完成反转吗？

### ✐
<div style="page-break-after: always"></div>

## [25. K 个一组翻转链表](https://leetcode-cn.com/problems/reverse-nodes-in-k-group/)

### 题目

给你一个链表，每 k 个节点一组进行翻转，请你返回翻转后的链表。

k 是一个正整数，它的值小于或等于链表的长度。

如果节点总数不是 k 的整数倍，那么请将最后剩余的节点保持原有顺序。

**示例1**
输入：head = [1,2,3,4,5], k = 2
输出：[2,1,4,3,5]

**示例2**
输入：head = [1,2,3,4,5], k = 3
输出：[3,2,1,4,5]

**示例3**
输入：head = [1,2,3,4,5], k = 1
输出：[1,2,3,4,5]

**示例4**
输入：head = [1], k = 1
输出：[1]

**提示**
* 链表中节点的数目在范围 [0, 500] 内
* -100 <= Node.val <= 100
* 1 <= k <= 链表节点数

**进阶**
你可以设计一个只用 O(1) 额外内存空间的算法解决此问题吗？

### ✐
<div style="page-break-after: always"></div>

## [21. 合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists/)

### 题目

将两个升序链表合并为一个新的 **升序** 链表并返回。新链表是通过拼接给定的两个链表的所有节点组成的。

**示例1**
输入：l1 = [1,2,4], l2 = [1,3,4]
输出：[1,1,2,3,4,4]

**示例2**
输入：l1 = [], l2 = []
输出：[]

**示例3**
输入：l1 = [], l2 = [0]
输出：[0]

**提示**
* 两个链表的节点数目范围是 [0, 50]
* -100 <= Node.val <= 100
* l1 和 l2 均按 非递减顺序 排列

### ✐
<div style="page-break-after: always"></div>

## [23. 合并K个升序链表](https://leetcode-cn.com/problems/merge-k-sorted-lists/)

### 题目

给你一个链表数组，每个链表都已经按升序排列。

请你将所有链表合并到一个升序链表中，返回合并后的链表。

**示例1**
输入：lists = [[1,4,5],[1,3,4],[2,6]]
输出：[1,1,2,3,4,4,5,6]
解释：链表数组如下：
[
  1->4->5,
  1->3->4,
  2->6
]
将它们合并到一个有序链表中得到。
1->1->2->3->4->4->5->6

**示例2**
输入：lists = []
输出：[]

**示例3**
输入：lists = [[]]
输出：[]

**提示**
* k == lists.length
* 0 <= k <= 10^4
* 0 <= lists[i].length <= 500
* -10^4 <= lists[i][j] <= 10^4
* lists[i] 按 升序 排列
* lists[i].length 的总和不超过 10^4

### ✐
<div style="page-break-after: always"></div>

## [23. 合并K个升序链表](https://leetcode-cn.com/problems/merge-k-sorted-lists/)

### 题目

给你一个链表数组，每个链表都已经按升序排列。

请你将所有链表合并到一个升序链表中，返回合并后的链表。

**示例1**
输入：lists = [[1,4,5],[1,3,4],[2,6]]
输出：[1,1,2,3,4,4,5,6]
解释：链表数组如下：
[
  1->4->5,

  1->3->4,

  2->6
]
将它们合并到一个有序链表中得到。
1->1->2->3->4->4->5->6

**示例2**
输入：lists = []
输出：[]

**示例3**
输入：lists = [[]]
输出：[]

**提示**
* k == lists.length
* 0 <= k <= 10^4
* 0 <= lists[i].length <= 500
* -10^4 <= lists[i][j] <= 10^4
* lists[i] 按 升序 排列
* lists[i].length 的总和不超过 10^4

### ✐
<div style="page-break-after: always"></div>

## [141. 环形链表](https://leetcode-cn.com/problems/linked-list-cycle/)

### 题目

给定一个链表，判断链表中是否有环。

如果链表中有某个节点，可以通过连续跟踪 next 指针再次到达，则链表中存在环。 为了表示给定链表中的环，评测系统内部使用整数 pos 来表示链表尾连接到链表中的位置（索引从 0 开始）。如果 pos 是 -1，则在该链表中没有环。注意：pos 不作为参数进行传递，仅仅是为了标识链表的实际情况。

如果链表中存在环，则返回 true 。 否则，返回 false 。

**示例1**
输入：head = [3,2,0,-4], pos = 1
输出：true
解释：链表中有一个环。从链表的头节点开始，链表中的各个节点依次为 3、2、0、-4，其中 2 的下一个节点是 0，0 的下一个节点是 -4，-4 的下一个节点是 2 ，形成了一个环。

**示例2**
输入：head = [1,2], pos = 0
输出：true
解释：链表中有一个环。从链表的头节点开始，链表中的各个节点依次为 1、2 。其中 2 的下一个节点是 1 ，形成了一个环。

**示例3**
输入：head = [1], pos = -1
输出：false
解释：链表中没有环。

**提示**
* 链表中节点的数目范围是 [0, 10^4]
* -10^5 <= Node.val <= 10^5
* pos 为 -1 或者链表中的一个有效索引。

### ✐
<div style="page-break-after: always"></div>

## [142. 环形链表 II](https://leetcode-cn.com/problems/linked-list-cycle-ii/)

### 题目

给定一个链表，返回链表开始入环的第一个节点。 如果链表无环，则返回 null。为了表示给定链表中的环，我们使用整数 pos 来表示链表尾连接到链表中的位置（索引从 0 开始）。如果 pos 是 -1，则在该链表中没有环。注意，pos 不作为参数进行传递，仅仅是为了标识链表的实际情况。

不允许修改 链表。


**示例1**
输入：head = [3,2,0,-4], pos = 1
输出返回索引：1
解释：链表中有一个环，其尾部连接到第二个节点。

**示例2**
输入：head = [1,2], pos = 0
输出返回索引：0
解释：链表中有一个环，其尾部连接到第一个节点。

**示例3**
输入：head = [1], pos = -1
输出返回索引：-1
解释：链表中没有环。

**提示**
* 链表中节点的数目范围是 [0, 10^4]
* -10^5 <= Node.val <= 10^5
* pos 为 -1 或者链表中的一个有效索引。

### ✐
<div style="page-break-after: always"></div>


## [160. 相交链表](https://leetcode-cn.com/problems/intersection-of-two-linked-lists/)

### 题目

给你两个单链表的头节点 headA 和 headB ，请你找出并返回两个单链表相交的起始节点。如果两个链表没有交点，返回 null 。

图示两个链表在节点 c1 开始相交：

![img](https://assets.leetcode-cn.com/aliyun-lc-upload/uploads/2018/12/13/160_statement.png)

题目数据 保证 整个链式结构中不存在环。

注意，函数返回结果后，链表必须 保持其原始结构 。

**示例1**
输入：intersectVal = 8, listA = [4,1,8,4,5], listB = [5,0,1,8,4,5], skipA = 2, skipB = 3
输出：Intersected at '8'
解释：相交节点的值为 8 （注意，如果两个链表相交则不能为 0）。
从各自的表头开始算起，链表 A 为 [4,1,8,4,5]，链表 B 为 [5,0,1,8,4,5]。在 A 中，相交节点前有 2 个节点；在 B 中，相交节点前有 3 个节点。

**示例2**
输入：intersectVal = 2, listA = [0,9,1,2,4], listB = [3,2,4], skipA = 3, skipB = 1
输出：Intersected at '2'
解释：相交节点的值为 2 （注意，如果两个链表相交则不能为 0）。
从各自的表头开始算起，链表 A 为 [0,9,1,2,4]，链表 B 为 [3,2,4]。在 A 中，相交节点前有 3 个节点；在 B 中，相交节点前有 1 个节点。

**示例3**
输入：intersectVal = 0, listA = [2,6,4], listB = [1,5], skipA = 3, skipB = 2
输出：null
解释：从各自的表头开始算起，链表 A 为 [2,6,4]，链表 B 为 [1,5]。由于这两个链表不相交，所以 intersectVal 必须为 0，而 skipA 和 skipB 可以是任意值。
这两个链表不相交，因此返回 null 。

**提示**

* listA 中节点数目为 m
* listB 中节点数目为 n
* 1 <= m, n <= 3 * 10^4
* 1 <= Node.val <= 10^5
* 0 <= skipA <= m

### ✐
<div style="page-break-after: always"></div>

## [19. 删除链表的倒数第 N 个结点](https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list/)

给你一个链表，删除链表的倒数第 `n` 个结点，并且返回链表的头结点。

**示例1**
输入：head = [1,2,3,4,5], n = 2
输出：[1,2,3,5]

**示例2**
输入：head = [1], n = 1
输出：[]

**示例3**
输入：head = [1,2], n = 1
输出：[1]

**提示**

* 链表中结点的数目为 `sz`
* 1 <= sz <= 30
* 0 <= Node.val <= 100
* 1 <= n <= sz

### ✐
<div style="page-break-after: always"></div>

## [83. 删除排序链表中的重复元素](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list/)

给定一个已排序的链表的头 `head` ， 删除所有重复的元素，使每个元素只出现一次 。返回 已排序的链表 。

**示例1**
输入：head = [1,1,2]
输出：[1,2]

**示例2**
输入：head = [1,1,2,3,3]
输出：[1,2,3]

**提示**

* 链表中节点数目为 `n`
* 0 <= n <= 300
* -100 <= Node.val <= 100
* 题目数据保证链表已经按升序排列

### ✐
<div style="page-break-after: always"></div>

## [82. 删除排序链表中的重复元素 II](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-list-ii/)

给定一个已排序的链表的头 `head` ， 删除所有重复元素，使每个元素只出现一次 。返回 已排序的链表 。

**示例1**
输入：head = [1,1,2]
输出：[2]

**示例2**
输入：head = [1,1,2,3,3]
输出：[2,3]

**提示**

* 链表中节点数目为 `n`
* 0 <= n <= 300
* -100 <= Node.val <= 100
* 题目数据保证链表已经按升序排列

### ✐
<div style="page-break-after: always"></div>

## [61. 旋转链表](https://leetcode-cn.com/problems/rotate-list/)

给你一个链表的头节点 `head` ，旋转链表，将链表每个节点向右移动 `k` 个位置。

**示例1**
输入：head = [1,2,3,4,5], k = 2
输出：[4,5,1,2,3]

**示例2**
输入：head = [0,1,2], k = 4
输出：[2,0,1]

**提示**

* 链表中节点数目为 `n`
* 1 <= n <= 500
* -100 <= Node.val <= 100
* 0 <= k <= 2 * 10^9

### ✐
<div style="page-break-after: always"></div>

## [24. 两两交换链表中的节点](https://leetcode-cn.com/problems/swap-nodes-in-pairs/)

给你一个链表，两两交换其中相邻的节点，并返回交换后链表的头节点。你必须在不修改节点内部的值的情况下完成本题（即，只能进行节点交换）。

**示例1**
输入：head = [1,2,3,4]
输出：[2,1,4,3]

**示例2**
输入：head = []
输出：[]

**示例3**
输入：head = [1]
输出：[1]

**提示**

* 链表中节点数目为 `n`
* 0 <= n <= 1000
* 1 <= Node.val <= 1000

### ✐
<div style="page-break-after: always"></div>

## [86. 分隔链表](https://leetcode-cn.com/problems/partition-list/)

给你一个链表的头节点 `head` 和一个特定值 `x` ，请你对链表进行分隔，使得所有 小于 `x` 的节点都出现在 大于或等于 `x` 的节点之前。

你应当 保留 两个分区中每个节点的初始相对位置。

**示例1**
输入：head = [1,4,3,2,5,2], x = 3
输出：[1,2,2,4,3,5]

**示例2**
输入：head = [2,1], x = 2
输出：[1,2]

**提示**

* 链表中节点数目为 `n`
* 1 <= n <= 500
* -100 <= Node.val <= 100
* -100 <= x <= 100

### ✐
<div style="page-break-after: always"></div>

## [328. 奇偶链表](https://leetcode-cn.com/problems/odd-even-linked-list/) 
给定一个单链表，把所有的奇数节点和偶数节点分别排在一起。请注意，这里的奇数节点和偶数节点指的是节点编号的奇偶性，而不是节点的值的奇偶性。

请尝试使用原地算法完成。你的算法的空间复杂度应为 O(1)，时间复杂度应为 O(nodes)，nodes 为节点总数。

**示例1**
输入: 1->2->3->4->5->NULL
输出: 1->3->5->2->4->NULL

**示例2**
输入: 2->1->3->5->6->4->7->NULL 
输出: 2->3->6->7->1->5->4->NULL

**提示**

* 链表中节点的数目在范围 [0, 10^4] 内
* -10^6 <= Node.val <= 10^6

### ✐
<div style="page-break-after: always"></div>

## [148. 排序链表](https://leetcode-cn.com/problems/sort-list/)

给你链表的头结点 `head` ，请将其按 **升序** 排列并返回 排序后的链表 。

**进阶：**

* 你可以在 `O(n log n)` 时间复杂度和 `O(1)` 空间复杂度下，对链表进行排序吗？

**示例1**
输入：head = [4,2,1,3]
输出：[1,2,3,4]

**示例2**
输入：head = [-1,5,3,4,0]
输出：[-1,0,3,4,5]

**示例3**
输入：head = []
输出：[]

**提示**

* 链表中节点的数目在范围 `[0, 5 * 10^4]` 内
* `-10^5 <= Node.val <= 10^5`

### ✐
<div style="page-break-after: always"></div>

## [234. 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list/)

请判断一个链表是否为回文链表。

**示例1**
输入: 1->2
输出: false

**示例2**
输入: 1->2->2->1
输出: true

**提示**

* 链表 L 的长度范围为 `[1, 10^5]`
* 0 <= node.val <= 9

### ✐
<div style="page-break-after: always"></div>

## [138. 复制带随机指针的链表](https://leetcode-cn.com/problems/copy-list-with-random-pointer/)

给你一个长度为 `n` 的链表，每个节点包含一个额外增加的随机指针 `random` ，该指针可以指向链表中的任何节点或空节点。构造这个链表的 **深拷贝**。 深拷贝应该正好由 `n` 个 **全新** 节点组成，其中每个新节点的值都设为其对应的原节点的值。新节点的 `next` 指针和 `random` 指针也都应指向复制链表中的新节点，并使原链表和复制链表中的这些指针能够表示相同的链表状态。复制链表中的指针都不应指向原链表中的节点 。例如，如果原链表中有 `X` 和 `Y` 两个节点，其中 `X.random --> Y` 。那么在复制链表中对应的两个节点 `x` 和 `y` ，同样有 `x.random --> y` 。返回复制链表的头节点。

用一个由 `n` 个节点组成的链表来表示输入/输出中的链表。每个节点用一个 `[val, random_index]` 表示：

* `val`：一个表示 `Node.val` 的整数。 
* `random_index`：随机指针指向的节点索引（范围从 `0` 到 `n-1`）；如果不指向任何节点，则为  `null` 。

你的代码 **只** 接受原链表的头节点 `head` 作为传入参数。

**示例1**
输入：head = [[7,null],[13,0],[11,4],[10,2],[1,0]]
输出：[[7,null],[13,0],[11,4],[10,2],[1,0]]

**示例2**
输入：head = [[1,1],[2,1]]
输出：[[1,1],[2,1]]

**提示**

* 链表中的节点数目在范围 `[0, 1000]` 内
* `-10000 <= Node.val <= 10000`
* `Node.random` 为 `null` 或指向链表中的节点。

### ✐
<div style="page-break-after: always"></div>

## [430. 扁平化多级双向链表](https://leetcode-cn.com/problems/flatten-a-multilevel-doubly-linked-list/)

多级双向链表中，除了指向下一个节点和前一个节点指针之外，它还有一个子链表指针，可能指向单独的双向链表。这些子列表也可能会有一个或多个自己的子项，依此类推，生成多级数据结构，如下面的示例所示。

给你位于列表第一级的头节点，请你扁平化列表，使所有结点出现在单级双链表中。

**示例1**
输入：head = [1,2,3,4,5,6,null,null,null,7,8,9,10,null,null,11,12]
输出：[1,2,3,7,8,11,12,9,10,4,5,6]
解释：
输入的多级列表如下图所示：
扁平化后的链表如下图：

**示例2**
输入：head = [1,2,null,3]
输出：[1,3,2]
解释：
输入的多级列表如下图所示：
扁平化后的链表如下图：

**提示**

* 节点数目不超过 1000
* 1 <= Node.val <= 10^5

### ✐
<div style="page-break-after: always"></div>
