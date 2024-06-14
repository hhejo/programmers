# [qr code](https://school.programmers.co.kr/learn/courses/30/lessons/181903)

### Lv. 0

### 풀이 날짜

- 240614 금

---

## CODE 1

```javascript
function solution(q, r, code) {
  let ans = "";
  [...code].map((e, i) => (i % q === r ? (ans += e) : ans));
  return ans;
}
```

## 해설 1
