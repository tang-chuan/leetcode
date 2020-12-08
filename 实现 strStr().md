#### [实现 strStr()](https://leetcode-cn.com/problems/implement-strstr/)

实现 strStr() 函数。

给定一个 haystack 字符串和一个 needle 字符串，在 haystack 字符串中找出 needle 字符串出现的第一个位置 (从0开始)。如果不存在，则返回  -1。

```
class Solution {
    public int strStr(String haystack, String needle) {
int length = needle.length();
        int index = 0;
        while (index + length <= haystack.length()){
            if (needle.equals(haystack.substring(index,index+length))){
                return index;
            }
            index++;
        }
        return -1;
    }
}
```

```
//输入："hello"
"ll"
//输出：2
```

