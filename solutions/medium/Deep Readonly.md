# 📝 Deep Readonly

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/deep-readonly)

### 💡 Solution

```typescript
type DeepReadonly<T> = T extends (...args: any[]) => any
	? T
	: T extends object
	? { readonly [K in keyof T]: DeepReadonly<T[K]> }
	: T;
```
