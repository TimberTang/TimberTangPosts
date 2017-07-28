---
title: 'Swift LeetCode 系列之 7: Reverse  Integer'
date: 2017-07-21 10:31:48
tags:
---



#### 本篇文章我是LeetCode 系列之第一篇, 仅此笔记代表自己的个人思路

#### 原地址

[LeetCode 7: Reverse Interger](https://leetcode.com/problems/reverse-integer/#/)

#### 描述

将数字进行反转

#### 注意点

 Int 的取值范围

#### 解决:

Swift

    class Solution {
        func reverse(_ x: Int) -> Int {
            var result = 0
            var remain = x  
            if x == 0 {
               return 0 
            }  
            repeat { 
                result = remain / 10  + remain % 10 * 10
                remain = remain / 10
                if (result < Int.min || result > Int.max) {
                	return 0
                }
            }while(remain > 0)
            
            return result 
        }
    }

