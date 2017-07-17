## Interfaces

```typescript
interface Writer {
	write(message: string): void;    
}
```

```typescript
function writeUserName(writer: Writer) {
	writer.write(user.name);
}
```
