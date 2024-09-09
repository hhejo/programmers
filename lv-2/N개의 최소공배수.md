# [N개의 최소공배수](https://school.programmers.co.kr/learn/courses/30/lessons/12953)

`Lv. 2`

- 240225 일

## 풀이 1

```javascript
function solution(arr) {
  function getGcd(a, b) {
    if (b === 0) return a;
    return getGcd(b, a % b);
  }
  let ans = arr.reduce((a, b) => (a * b) / getGcd(a, b));
  return ans;
}
```
