# [[PCCP 기출문제] 1번 / 붕대 감기](https://school.programmers.co.kr/learn/courses/30/lessons/250137)

### Lv. 1

### 풀이 날짜

- 231213 수

---

## CODE 1

```javascript
function solution(bandage, health, attacks) {
  let [currentTime, currentHealth] = [0, health];
  for (let [time, damage] of attacks) {
    let diffTime = time - currentTime - 1;
    currentHealth += bandage[1] * diffTime;
    if (diffTime >= bandage[0])
      currentHealth += bandage[2] * Math.floor(diffTime / bandage[0]);
    if (currentHealth > health) currentHealth = health;
    currentHealth -= damage;
    if (currentHealth <= 0) return -1;
    currentTime = time;
  }
  return currentHealth;
}
```

## 해설 1
