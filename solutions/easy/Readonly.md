# 📝 Readonly

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/readonly)

### 💡 Solution

```typescript
type MyReadonly<T> = {
	readonly [K in keyof T]: T[K];
};
```
