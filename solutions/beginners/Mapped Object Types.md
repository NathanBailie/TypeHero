# 📝 Mapped Object Types

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/mapped-object-types)

### 💡 Solution

```typescript
type MovieInfoByGenre<T> = {
	[K in keyof T]: {
		name: string;
		year: number;
		director: string;
	};
};
```
