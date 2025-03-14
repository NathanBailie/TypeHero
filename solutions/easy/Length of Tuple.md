# 📝 Length of Tuple

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/length-of-tuple)

### 💡 Solution

```typescript
type Length<T extends readonly any[]> = T['length'];
```
