# [x만큼 간격이 있는 n개의 숫자](https://school.programmers.co.kr/learn/courses/30/lessons/12954)

### Lv. 1

### 풀이 날짜

- 240201 목

---

## CODE 1

```javascript
function solution(x, n) {
  let [ans, acc] = [[], 0];
  for (let i = 0; i < n; i++) {
    acc += x;
    ans.push(acc);
  }
  return ans;
}
```

## 해설 1
