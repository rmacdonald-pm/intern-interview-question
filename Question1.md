
```python
@app.route('/update-name', methods=['POST'])
def updateName():
    data = request.json
    update_db(data.name)
    return jsonify({"success": True}), 200
```
