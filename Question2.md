```javascript
async function submitName(firstName) {
  const response = await fetch("/update-name", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify('{"firstName": "John"}'),
  });
  const result = await response.json();
  return result;
}
```
