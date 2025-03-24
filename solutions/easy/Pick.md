# 📝 Pick

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/pick)

### 💡 Solution

```typescript
type MyPick<T, K extends keyof T> = {
	[P in K]: T[P];
};
```
