# 📝 Trim Left

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/trim-left)

### 💡 Solution

```typescript
type TrimLeft<S extends string> = S extends `${' ' | '\n' | '\t'}${infer Rest}`
	? TrimLeft<Rest>
	: S;
```
