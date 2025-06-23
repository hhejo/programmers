# K번째수

Programmers

- **[K번째수](https://school.programmers.co.kr/learn/courses/30/lessons/42748)**
- Difficulty: `Lv. 1`

Solution Dates

- 240201 목
- 250623 월

## Solution 1

Code

```javascript
function solution(array, commands) {
  let ans = [];
  for (let [i, j, k] of commands) {
    let newArr = array.slice(i - 1, j).sort((a, b) => a - b);
    ans.push(newArr[k - 1]);
  }
  return ans;
}
```

Explanation

## Solution 2

Code

```javascript
function solution(array, commands) {
  const answer = [];
  for (let [i, j, k] of commands) {
    const arr = array.slice(i - 1, j).sort((a, b) => a - b);
    answer.push(arr[k - 1]);
  }
  return answer;
}
```

Explanation
