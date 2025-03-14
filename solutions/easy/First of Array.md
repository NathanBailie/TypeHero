# 📝 First of Array

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/first-of-array)

### 💡 Solution

```typescript
type First<T extends any[]> = T extends [] ? never : T[0];
```
