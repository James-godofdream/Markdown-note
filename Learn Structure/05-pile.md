# 优先队列与集合
## Priority Queue
<table>
<tr>
    <th></th><th>插入</th><th>查找</th><th>删除</th><th>评价</th>
</tr>
<tr>
    <td>数组</td><td>Θ(1)</td><td>Θ(N)</td><td>Θ(1)</td><td>查找慢</td>
</tr>
<tr>
    <td>单链表</td><td>Θ(1)</td><td>Θ(N)</td><td>Θ(1)</td><td>查找慢、空间费</td>
</tr>
<tr>
    <td>排序数组</td><td>Θ(logN)+Θ(N)</td><td>Θ(1)</td><td>Θ(1)</td><td>需排序、插入慢、需移动</td>
</tr>
<tr>
    <td>排序单链表</td><td>Θ(N)+Θ(1)</td><td>Θ(1)</td><td>Θ(1)</td><td>需排序、插入慢、空间费</td>
</tr>
<tr>
    <td>二叉搜索树</td><td>Θ(logN)</td><td>Θ(logN)</td><td>Θ(logN)</td><td>严重失衡</td>
</tr>
<tr>
    <td>AVL树</td><td>Θ(logN)</td><td>Θ(logN)</td><td>Θ(logN)</td><td>操作复杂、功能太多</td>
</tr>
</table>

# 堆  （完全二叉树）
### 创建：空堆
### 插入：插入在最后
### 然后 向上渗透percolate up
### 找儿子 下标*2+/-1
### 找父亲 下标/2 取整










