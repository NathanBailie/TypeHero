# 📝 IsNever

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/isnever)

### 💡 Solution

```typescript
type IsNever<T> = [T] extends [never] ? true : false;
```
