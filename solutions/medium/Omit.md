# 📝 Omit

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/omit)

### 💡 Solution

```typescript
type MyOmit<T, K extends keyof T> = {
	[P in keyof T as P extends K ? never : P]: T[P];
};
```
