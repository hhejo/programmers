# [n보다 커질 때까지 더하기](https://school.programmers.co.kr/learn/courses/30/lessons/181884)

### Lv. 0

### 풀이 날짜

- 240510 금

---

## CODE 1

```javascript
function solution(numbers, n) {
  let acc = 0;
  for (let num of numbers) {
    if (acc > n) break;
    acc += num;
  }
  return acc;
}
```

## 해설 1
