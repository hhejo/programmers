# [x 사이의 개수](https://school.programmers.co.kr/learn/courses/30/lessons/181867)

### Lv. 0

### 풀이 날짜

- 240528 화

---

## CODE 1

```javascript
function solution(myString) {
  const ans = myString.split("x").map((el) => el.length);
  return ans;
}
```

## 해설 1
