# Development

- [Getting started](development/getting-started.md)
- [Testing](development/testing.md)
- [Github OpenAPI](development/github-openapi.md)
- [Github GraphQL](development/github-graphql.md)

## Deprecation warning

Before removing attributes/methods, consider adding deprecation warnings instead.
The [typing_extensions](https://pypi.org/project/typing-extensions/) package provides a handy decorator to add deprecation warnings.

```python
from typing_extensions import deprecated

@property
@deprecated("Use core instead")
def rate(self):
   pass

@deprecated("Deprecated in favor of the new branch protection")
def get_protected_branch(self):
   pass
```
