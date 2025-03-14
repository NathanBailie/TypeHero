# 📝 Tuple to Object

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/tuple-to-object)

### 💡 Solution

```typescript
type TupleToObject<T extends readonly PropertyKey[]> = {
	[K in T[any]]: K;
};
```
