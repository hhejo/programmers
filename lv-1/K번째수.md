# [K번째수](https://school.programmers.co.kr/learn/courses/30/lessons/42748)

### Lv. 1

### 풀이 날짜

- 240201 목

---

## CODE 1

```javascript
function solution(array, commands) {
  let ans = [];
  for (let [i, j, k] of commands) {
    let newArr = array.slice(i - 1, j).sort((a, b) => a - b);
    ans.push(newArr[k - 1]);
  }
  return ans;
}
```

## 해설 1
