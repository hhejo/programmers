# [홀수 vs 짝수](https://school.programmers.co.kr/learn/courses/30/lessons/181887)

### Lv. 0

### 풀이 날짜

- 240508 수

---

## CODE 1

```javascript
function solution(num_list) {
  let [sumEven, sumOdds] = [0, 0];
  for (let [idx, num] of num_list.entries()) {
    if (idx % 2) sumOdds += num;
    else sumEven += num;
  }
  let ans = sumEven > sumOdds ? sumEven : sumOdds;
  return ans;
}
```

## 해설 1
