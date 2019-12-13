# Hashing Algorithm

```javascript
1. looper = 1
2. addr = 0

hash key
3. loop(looper <= size)
    1. if (key[looper] not space)
        1. addr = addr + key[looper]
        2. rotate addr 12 bite right
    2. looper = looper + 1

test for negative address
4. if (addr <= 0)
    1. addr = absolute(addr)
5. addr = addr modulo maxAddr + 1
6. return

end hash
```