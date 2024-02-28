# [H-Index](https://school.programmers.co.kr/learn/courses/30/lessons/42747)

### Lv. 2

### 풀이 날짜

- 240228 수

---

## CODE 1

```javascript
function solution(citations) {
  let ans = 0;
  citations.sort((a, b) => b - a);
  for (let i = 0; i < citations.length; i++) {
    if (citations[i] <= i) break;
    ans += 1;
  }

  return ans;
}
```

## 해설 1
