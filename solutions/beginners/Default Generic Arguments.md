# 📝 Default Generic Arguments

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/default-generic-arguments)

### 💡 Solution

```typescript
type ApiRequest<T, M extends string = 'GET'> = { data: T; method: M };
type TSConfig<C = { strict: true }> = C;
```
