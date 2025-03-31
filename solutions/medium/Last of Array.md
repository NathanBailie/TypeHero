# 📝 Last of Array

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/last-of-array)

### 💡 Solution

```typescript
type Last<T extends any[]> = T extends [...infer Rest, infer Last]
	? Last
	: never;
```
