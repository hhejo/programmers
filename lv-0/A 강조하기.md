# [A 강조하기](https://school.programmers.co.kr/learn/courses/30/lessons/181874)

### Lv. 0

### 풀이 날짜

- 240515 수

---

## CODE 1

```javascript
function solution(myString) {
  let ans = "";
  for (let ch of myString) {
    if (ch === "a") ans += "A";
    else if (ch === ch.toUpperCase() && ch !== "A") ans += ch.toLowerCase();
    else ans += ch;
  }
  return ans;
}
```

## 해설 1
