###### LiteDBC API Reference
[Home](/docs/api/README.md) | [Project](/README.md) | [Module](/docs/api/modules/litedbc/__init__/README.md) | [Source](/src/litedbc/__init__.py)

# Class ColumnInfo
> Module: [litedbc.\_\_init\_\_](/docs/api/modules/litedbc/__init__/README.md)
>
> Class: **ColumnInfo**
>
> Inheritance: `tuple`

ColumnInfo(cid, name, type, not_null, default, primary_key, foreign_key, index_info)

## Fields table
Here are fields exposed in the class:

| Field | Description |
| --- | --- |
| cid | Alias for field number 0 |
| name | Alias for field number 1 |
| type | Alias for field number 2 |
| not\_null | Alias for field number 3 |
| default | Alias for field number 4 |
| primary\_key | Alias for field number 5 |
| foreign\_key | Alias for field number 6 |
| index\_info | Alias for field number 7 |

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

# Methods within class
Here are methods exposed in the class:
- [\_asdict](#_asdict)
- [\_make](#_make)
- [\_replace](#_replace)

## \_asdict
Return a new dict which maps field names to their values.

```python
def _asdict(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_make
Make a new ColumnInfo object from a sequence or iterable

```python
@classmethod
def _make(iterable):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_replace
Return a new ColumnInfo object replacing specified fields with new values

```python
def _replace(self, /, **kwds):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>
