目前支持的 hash 算法：

```
function hashCode(str) {
        let hash = 0;
        for (let i = 0; i < str.length; i++) {
          hash = (hash << 5) - hash + str.charCodeAt(i); // hash * 31 + char
          hash |= 0; // 转换为32位整数
        }
        return hash;
      }
```
