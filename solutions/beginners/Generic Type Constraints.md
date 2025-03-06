# 📝 Generic Type Constraints

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/generic-type-constraints/submissions/383720?success=true)

### 💡 Solution

```typescript
type AllowString<T extends string> = T extends string ? string : never;

type AllowNumber<T extends number> = T extends number ? number : never;

type CreateLogger<T extends (arg: number) => void> = T extends (
	arg: number
) => void
	? { log: T; exit: () => void }
	: never;
```
