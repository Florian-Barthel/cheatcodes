# [Home](../README.md)

## JSON

### Read

```python
import json

with open("path", "r") as file:
  data = json.load(f)
```

### write

```python
import json

with open("path", "w") as file:
  json.dump(data_dict, file)
```
