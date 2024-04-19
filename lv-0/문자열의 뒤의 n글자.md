# [문자열의 뒤의 n글자](https://school.programmers.co.kr/learn/courses/30/lessons/181910)

### Lv. 0

### 풀이 날짜

- 240420 토

---

## CODE 1

```javascript
function solution(my_string, n) {
  let len = my_string.length;
  let ans = my_string.slice(len - n);
  return ans;
}
```

## 해설 1
