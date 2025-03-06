# 📝 Generic Function Arguments

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/generic-function-arguments)

### 💡 Solution

```typescript
// #1
const identity = <T>(arg: T): T => arg;

const mapArray = <T, M>(arr: T[], fn: (elem: T) => M): M[] => arr.map(fn);

// #2
function identity<T>(arg: T) {
	return arg;
}

const mapArray = <T, M>(arr: T[], fn: (elem: T) => M): M[] => {
	return arr.map(fn);
};
```
