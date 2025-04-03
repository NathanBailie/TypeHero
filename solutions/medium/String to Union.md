# 📝 String to Union

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/string-to-union)

### 💡 Solution

```typescript
type StringToUnion<T extends string> = T extends `${infer First}${infer Rest}`
	? First | StringToUnion<Rest>
	: never;
```
