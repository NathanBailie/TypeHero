# 📝 Unshift

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/unshift)

### 💡 Solution

```typescript
type Unshift<T extends any[], U> = [U, ...T];
```
