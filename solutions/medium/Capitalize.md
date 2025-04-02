# 📝 Capitalize

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/capitalize)

### 💡 Solution

```typescript
type MyCapitalize<S extends string> = S extends `${infer First}${infer Rest}`
	? `${Uppercase<First>}${Rest}`
	: S;
```
