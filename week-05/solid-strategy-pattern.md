# Week 5 — Open/Closed Principle with Strategy

```python
from typing import Protocol

class Discount(Protocol):
    def apply(self, total: float) -> float: ...

class StudentDiscount:
    def apply(self, total: float) -> float:
        return total * 0.90

def checkout(total: float, discount: Discount) -> float:
    return discount.apply(total)
```

New discount rules extend the system without changing `checkout`.
