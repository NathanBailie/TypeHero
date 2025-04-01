# 📝 Pop

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/pop)

### 💡 Solution

```typescript
type Pop<T extends any[]> = T extends [...infer Rest, any] ? Rest : [];
```
