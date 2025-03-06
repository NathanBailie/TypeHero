# 📝 Generic Type Arguments

## 🔗 [Task description on CodeWars](https://typehero.dev/challenge/generic-type-arguments)

### 💡 Solution

```typescript
type GroceryStore<Name, City> = {
	name: Name;
	city: City;
};

type GroceryItem = {
	name: string;
	price: number;
	inStock: boolean;
};

type CapreseSalad = GroceryItem & {
	name: 'Caprese Salad';
	price: 14.99;
	inStock: true;
};
```
