# 📝 Type Unions

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/type-unions)

### 💡 Solution

```typescript
type Meters = {
	unit: 'meters';
	value: number;
};

type Miles = {
	unit: 'miles';
	value: number;
};

type Feets = {
	unit: 'feet';
	value: number;
};

type Distance = Meters | Miles | Feets;

type Position =
	| 'top'
	| 'topLeft'
	| 'topRight'
	| 'left'
	| 'center'
	| 'right'
	| 'bottomLeft'
	| 'bottom'
	| 'bottomRight';
```
