# [문자열 내 p와 y의 개수](https://school.programmers.co.kr/learn/courses/30/lessons/12916)

### Lv. 1

### 풀이 날짜

- 240201 목

---

## CODE 1

```javascript
function solution(s) {
  let arr = [...s.toUpperCase()];
  let p = arr.reduce((acc, ch) => (ch === "P" ? acc + 1 : acc), 0);
  let y = arr.reduce((acc, ch) => (ch === "Y" ? acc + 1 : acc), 0);
  let ans = p === y ? true : false;
  return ans;
}
```

## 해설 1
