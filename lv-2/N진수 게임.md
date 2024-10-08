# [N진수 게임](https://school.programmers.co.kr/learn/courses/30/lessons/17687)

`Lv. 2`

- 241008 화

## 풀이 1

```javascript
function solution(n, t, m, p) {
  let [num, order, result] = [0, 0, ''];
  while (result.length < t) {
    for (let chNum of num.toString(n)) {
      if (order === p - 1) result += chNum;
      order = (order + 1) % m;
      if (result.length >= t) break;
    }
    num++;
  }
  return result.toUpperCase();
}
```
