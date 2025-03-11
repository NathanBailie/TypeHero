# 📝 The `typeof` Operator

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/typeof)

### 💡 Solution

```typescript
type Width = typeof width;

type Margin = {
	[K in keyof typeof margin]: number;
};

type Data = {
	category: string;
	value: number;
}[];

type YScale = {
	type: string;
	domain: number[];
	range: number[];
};

type D3ChartConfig = {
	width: number;
	height: number;
	margin: Margin;
	data: Data;
	xScale: {
		type: string;
		domain: number[];
		range: number[];
	};
	yScale: {
		type: string;
		domain: number[];
		range: number[];
	};
	xAxis: {
		label: string;
		tickSize: number;
	};
	yAxis: {
		label: string;
		tickSize: number;
	};
	bar: {
		fill: string;
	};
};
```
