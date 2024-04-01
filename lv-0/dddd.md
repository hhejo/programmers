# [코드 처리하기](https://school.programmers.co.kr/learn/courses/30/lessons/181932)

### Lv. 0

### 풀이 날짜

- 240401 월

---

## CODE 1

```javascript
function solution(code) {
  let [mode, ret] = [0, ""];
  for (let i = 0; i < code.length; i++) {
    if (mode === 0) {
      if (code[i] !== "1" && i % 2 === 0) ret += code[i];
      else if (code[i] === "1") mode = 1;
    } else {
      if (code[i] !== "1" && i % 2 === 1) ret += code[i];
      else if (code[i] === "1") mode = 0;
    }
  }
  return ret === "" ? "EMPTY" : ret;
}
```

## 해설 1
