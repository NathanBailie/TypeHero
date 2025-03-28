# 📝 Tuple to Union

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/tuple-to-union)

### 💡 Solution

```typescript
type TupleToUnion<T extends any[]> = T[any];
```
