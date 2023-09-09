# [Home](../README.md)

## JSON

### read

```python
import json

with open("path", "r") as file:
  data = json.load(file)
```

### write

```python
import json

with open("path", "w") as file:
  json.dump(data_dict, file)
```
