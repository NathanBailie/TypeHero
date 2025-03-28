# 📝 AnyOf

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/anyof)

### 💡 Solution

```typescript
type Falsy = 0 | '' | false | [] | Record<string, never> | undefined | null;
type AnyOf<T extends readonly any[]> = T[number] extends Falsy ? false : true;
```
