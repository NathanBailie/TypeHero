# 📝 Length of String

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/length-of-string)

### 💡 Solution

```typescript
type LengthOfString<
	S extends string,
	T extends any[] = []
> = S extends `${infer First}${infer Rest}`
	? LengthOfString<Rest, [First, ...T]>
	: T['length'];
```
