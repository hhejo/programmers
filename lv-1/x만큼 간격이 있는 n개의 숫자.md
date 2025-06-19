# x만큼 간격이 있는 n개의 숫자

Programmers

- **[x만큼 간격이 있는 n개의 숫자](https://school.programmers.co.kr/learn/courses/30/lessons/12954)**
- Difficulty: `Lv. 1`

Solution Dates

- 240201 목
- 250620 금

## Solution 1

Code

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

Explanation

## Solution 2

Code

```javascript
function solution(x, n) {
  let ans = Array(n).fill(x);
  for (let i = 1; i < n; i++) {
    ans[i] = ans[i - 1] + x;
  }
  return ans;
}
```

Explanation
