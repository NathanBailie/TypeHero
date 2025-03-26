# 📝 Absolute

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/absolute)

### 💡 Solution

```typescript
type Absolute<T extends number | string | bigint> = `${T}` extends `-${infer U}`
	? U
	: `${T}`;
```
