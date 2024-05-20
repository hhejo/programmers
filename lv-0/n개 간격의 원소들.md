# [n개 간격의 원소들](https://school.programmers.co.kr/learn/courses/30/lessons/181888)

### Lv. 0

### 풀이 날짜

- 240520 월

---

## CODE 1

```javascript
function solution(num_list, n) {
  const ans = [];
  for (let i = 0; i < num_list.length; i += n) {
    ans.push(num_list[i]);
  }
  return ans;
}
```

## 해설 1
