# [ad 제거하기](https://school.programmers.co.kr/learn/courses/30/lessons/181870)

### Lv. 0

### 풀이 날짜

- 240524 금

---

## CODE 1

```javascript
function solution(strArr) {
  let ans = [];
  for (let str of strArr) {
    if (str.includes("ad")) continue;
    ans.push(str);
  }
  return ans;
}
```

## 해설 1
