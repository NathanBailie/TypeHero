# 📝 IsUnion

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/isunion)

### 💡 Solution

```typescript
type IsUnion<T, U = T> = T extends T ? ([U] extends [T] ? false : true) : never;
```
