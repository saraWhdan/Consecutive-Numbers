# Consecutive-Numbers
# Triangle-Judgement

Problem Link:https://leetcode.com/problems/consecutive-numbers/description/?envType=study-plan-v2&envId=top-sql-50


## Solution

```sql
SELECT DISTINCT t3.num AS ConsecutiveNums
FROM Logs t1
JOIN Logs t2 ON t2.id=t1.id-1 AND t2.num=t1.num
JOIN Logs t3 ON t3.id=t2.id-1 AND t3.num=t2.num
```
