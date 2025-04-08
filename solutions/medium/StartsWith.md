# 📝 StartsWith

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/startswith)

### 💡 Solution

```typescript
type StartsWith<T extends string, U extends string> = T extends `${U}${string}`
	? true
	: false;
```
