# 📝 AllCombinations

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/allcombinations)

### 💡 Solution

```typescript
type StringToUnion<S extends string> = S extends `${infer First}${infer Rest}`
	? First | StringToUnion<Rest>
	: never;

type AllCombinations<S extends string, P extends string = StringToUnion<S>> = [
	P
] extends [never]
	? ''
	:
			| ''
			| {
					[K in P]: `${K}${AllCombinations<never, Exclude<P, K>>}`;
			  }[P];

type AllCombinations_ABC = AllCombinations<'ABC'>;
```
