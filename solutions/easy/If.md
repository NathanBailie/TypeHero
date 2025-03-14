# 📝 If

## 🔗 [Task description on TypeHero](https://typehero.dev/challenge/if)

### 💡 Solution

```typescript
type If<C extends true | false, T, F> = C extends true ? T : F;
```
