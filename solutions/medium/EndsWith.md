# 📝 EndsWith

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/endswith)

### 💡 Solution

```typescript
type EndsWith<T extends string, U extends string> = T extends `${string}${U}`
	? true
	: false;
```
