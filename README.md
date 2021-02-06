### Hi there 👋

<h3>
    
```python
​
import json
from dataclasses import asdict, dataclass


@dataclass
class Stack:
    languages   : tuple[str, ...] = ("Python", "HTML", "CSS")
    misc        : tuple[str, ...] = ("WebDev & SysAdmin", "Linux", "Pyrogram")
    ongoing     : tuple[str, ...] = ("CyberSec Stuff", "C", "C++")

    def serialize(self):
        return json.dumps(asdict(self), indent=4)


stack = Stack()
print(stack.serialize())
​
```
</h3>


