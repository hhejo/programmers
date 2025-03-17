# 문자열 내 p와 y의 개수

Programmers

- [문자열 내 p와 y의 개수](https://school.programmers.co.kr/learn/courses/30/lessons/12916)
- Difficulty: `Lv. 1`

Solution Dates

- 240201 목
- 250318 화

## Solution 1

Code

```javascript
function solution(s) {
  let arr = [...s.toUpperCase()];
  let p = arr.reduce((acc, ch) => (ch === 'P' ? acc + 1 : acc), 0);
  let y = arr.reduce((acc, ch) => (ch === 'Y' ? acc + 1 : acc), 0);
  let ans = p === y ? true : false;
  return ans;
}
```

Explanation

## Solution 2

Code

```javascript
function solution(s) {
  let [ans, p, y] = [true, 0, 0];
  for (let ch of s) {
    ch = ch.toUpperCase();
    if (ch === 'P') p++;
    else if (ch === 'Y') y++;
  }
  if (p !== y) ans = false;
  return ans;
}
```

Explanation
