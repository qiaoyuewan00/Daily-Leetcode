# 思路

* 设置`dummyHead`+模拟

* 设置`dummyHead`+快慢指针

  倒数第`N`个节点，让快指针先走`N+1`步，然后移动快慢指针，直到`快指针.next.next`为`NULL`，此时慢指针还有`N`步到最后一个节点，也就是在倒数第`N`个节点了，设置`慢指针.next=慢指针.next.next`

# 题目

- [ ] https://leetcode.cn/problems/remove-nth-node-from-end-of-list/description/