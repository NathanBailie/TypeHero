# 📝 Replace

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/replace)

### 💡 Solution

```typescript
type Replace<
	S extends string,
	From extends string,
	To extends string
> = From extends ''
	? S
	: S extends `${infer Start}${From}${infer End}`
	? `${Start}${To}${End}`
	: S;
```
