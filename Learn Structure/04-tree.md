# 树结构
### 二叉树及遍历
### 满二叉树 (Full Binary Tree)
#### 每一个节点要么没有节点，要么每个节点都有两个子节点
### 完全二叉树(Complete BT)
#### 从左至右不能有空子节点
### 完美二叉树(Perfect BT)
### 所有层级必须拥有所有子节点，无法再增加
### 树与二叉树的顺序实现
#### 补充子节点至完全二叉树，并编号
### 树与二叉树的链式实现
#### 指向父节点，则不便于寻找子节点
#### 左子右兄
#### 二叉树则分左右指针即可，或可添父节点
### 二叉树的遍历
### 递归
#### 前序遍历：先访问根节点，再按前序遍历的方式访问左子树，再右子树【根左右】
#### 中序遍历：先用中根序的方式访问左子树，再用中根序的方式访问根树，再用中根序的方式访问右子树【左根右】
#### 后序遍历：先用后根序的方式访问左子树，再用后根序的方式访问右子树，再访问根树【左右根】
## 迭代
### 任何递归程序都可以通过栈将递归转化为非递归函数
## 层序
# 二叉搜索树（BST) ：Binary search tree
### 左子树元素比树根小
### 右子树元素比树根大
### 左右子树都是BST
## 查找操作
### FindMax
### FindMin
### FindX
## 插入与删除
### 删除叶子节点：直接删除
### 删除单叶子节点：上下线连接
### 删除双叶子节点：
#### 1、用左树最大或右树最小元素代替待删节点
#### 2、删左子树最大或右子树最小
# 平衡二叉搜索树（AVL）
## Adelson Velsky Landis Trees:
## 自平衡的二叉搜索树
### 空树是平衡的
### 非空树平衡<=>左右子树平衡 且 左右子树高度差绝对值< = 1
### => 每个节点的平衡因子（balance factor)是-1、0、或1.
### 左左单旋：左子树的左子树的插入导致不平衡
#### 则原根节点的左儿子变成新的根节点，原根节点变成新根节点的右子树，新根节点原来的右节点变成原根节点的左节点
### 左右双旋：左子树的右子树下的插入导致根节点不平衡
#### 根节点的左子树的右子节点变为新的根节点，原根节点变成新根节点的右子树，新根节点原位置的左子树变成根节点的左子树的右子树，新根节点原位置的右子树变成原根节点新位置的左子树