# 📝 Concat

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/concat)

### 💡 Solution

```typescript
type Concat<T extends readonly any[], U extends readonly any[]> = [...T, ...U]
```
