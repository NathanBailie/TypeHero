# 📝 Index Signatures

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/index-signatures)

### 💡 Solution

```typescript
type Character = {
	id: number;
	name: string;
	status: string;
	species: string;
};

// №1
type GroceryList = Record<string, number>;

type InappropriateActionBySituation = Record<string, string[]>;

type CharactersById = Record<number, Character>;

// №2
// type GroceryList = {
// 	[key: string]: number;
// };

// type InappropriateActionBySituation = {
// 	[key: string]: string[];
// };

// type CharactersById = {
// 	[id: number]: Character;
// };
```
