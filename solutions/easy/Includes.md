# 📝 Includes

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/includes)

### 💡 Solution

```typescript
type Includes<T extends readonly any[], U> = T extends [
	infer First,
	...infer Rest
]
	? Equal<First, U> extends true
		? true
		: Includes<Rest, U>
	: false;

type Equal<A, B> = (<T>() => T extends A ? 1 : 2) extends <T>() => T extends B
	? 1
	: 2
	? true
	: false;
```
