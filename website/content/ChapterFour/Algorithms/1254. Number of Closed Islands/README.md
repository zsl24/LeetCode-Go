# [1254. Number of Closed Islands](https://leetcode.com/problems/number-of-closed-islands/)


## 题目:

Given a 2D `grid` consists of `0s` (land) and `1s` (water). An *island* is a maximal 4-directionally connected group of `0s` and a *closed island* is an island **totally** (all left, top, right, bottom) surrounded by `1s.`

Return the number of *closed islands*.

**Example 1:**

![https://assets.leetcode.com/uploads/2019/10/31/sample_3_1610.png](https://assets.leetcode.com/uploads/2019/10/31/sample_3_1610.png)

    Input:Output:Explanation:

**Example 2:**

![https://assets.leetcode.com/uploads/2019/10/31/sample_4_1610.png](https://assets.leetcode.com/uploads/2019/10/31/sample_4_1610.png)

    Input:Output:

**Example 3:**

    Input:Output:

**Constraints:**

- `1 <= grid.length, grid[0].length <= 100`
- `0 <= grid[i][j] <=1`

## 题目大意

有一个二维矩阵 grid ，每个位置要么是陆地（记号为 0 ）要么是水域（记号为 1 ）。我们从一块陆地出发，每次可以往上下左右 4 个方向相邻区域走，能走到的所有陆地区域，我们将其称为一座「岛屿」。如果一座岛屿 完全 由水域包围，即陆地边缘上下左右所有相邻区域都是水域，那么我们将其称为 「封闭岛屿」。请返回封闭岛屿的数目。

提示：

- 1 <= grid.length, grid[0].length <= 100
- 0 <= grid[i][j] <=1


## 解题思路

- 给出一个地图，1 代表海水，0 代表陆地。要求找出四周都是海水的陆地的总个数。
- 这一题和第 200 题解题思路完全一致。只不过这一题要求必须四周都是海水，第 200 题的陆地可以是靠着地图边缘的。在此题中，靠着地图边缘的陆地不能最终计数到结果中。
