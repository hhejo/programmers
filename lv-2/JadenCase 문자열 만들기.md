# [JadenCase 문자열 만들기](https://school.programmers.co.kr/learn/courses/30/lessons/12951)

`Lv. 2`

- 240211 일

## 풀이 1

```javascript
function solution(s) {
  let ans = '';
  const arr = [...s.toLowerCase()];
  for (let i = 0; i < arr.length; i++) {
    if (arr[i - 1] === ' ' || i === 0) ans += arr[i].toUpperCase();
    else ans += arr[i].toLowerCase();
  }
  return ans;
}
```
