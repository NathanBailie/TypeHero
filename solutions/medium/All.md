# 📝 All

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/all)

### 💡 Solution

```typescript
type All<T extends any[], P> = T extends [infer First, ...infer Rest]
	? Equal<First, P> extends true
		? All<Rest, P>
		: false
	: true;

type Equal<A, B> = (<T>() => T extends A ? 1 : 2) extends <T>() => T extends B
	? 1
	: 2
	? true
	: false;
```
