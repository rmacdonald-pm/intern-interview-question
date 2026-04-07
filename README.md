# Python Flask
```python
@app.route('/update-name', methods=['POST'])
def updateName():
    data = request.json
    update_db(data.name)
    return jsonify({"success": True}), 200
```


# Javascript
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
