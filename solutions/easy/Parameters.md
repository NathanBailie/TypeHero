# 📝 Parameters

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/parameters)

### 💡 Solution

```typescript
type MyParameters<T extends (...args: any) => any> = T extends (
	...args: infer P
) => any
	? P
	: never;
```
