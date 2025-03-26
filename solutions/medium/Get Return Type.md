# 📝 Get Return Type

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/get-return-type)

### 💡 Solution

```typescript
type MyReturnType<T> = T extends (...args: any) => infer U ? U : never;
```
