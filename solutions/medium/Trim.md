# 📝 Trim

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/trim)

### 💡 Solution

```typescript
type Trim<T extends string> = T extends `${' ' | '\n' | '\t'}${infer Str}`
	? Trim<Str>
	: T extends `${infer Str}${' ' | '\n' | '\t'}`
	? Trim<Str>
	: T;
```
