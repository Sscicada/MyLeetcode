

[剑指 Offer 05. 替换空格](https://leetcode-cn.com/problems/ti-huan-kong-ge-lcof/)

```C++
class Solution {
public:
    string replaceSpace(string s) {
        string res;
        for(auto c:s){
            if(c!=' '){
                res.push_back(c);
            }
            else{
                res.push_back('%');
                res.push_back('2');
                res.push_back('0');
            }
        }
        return res;
    }
};
```
