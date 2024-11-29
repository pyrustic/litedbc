###### LiteDBC API Reference
[Home](/docs/api/README.md) | [Project](/README.md) | [Module](/docs/api/modules/litedbc/cursor/__init__/README.md) | [Source](/src/litedbc/cursor/__init__.py)

# Class Cursor
> Module: [litedbc.cursor.\_\_init\_\_](/docs/api/modules/litedbc/cursor/__init__/README.md)
>
> Class: **Cursor**
>
> Inheritance: `object`

When the cursor context is not nested, i.e., not created within a transaction,
it will `ROLLBACK` a pending transaction when you close it (the cursor)

## Properties table
Here are properties exposed in the class:

| Property | Methods | Description |
| --- | --- | --- |
| arraysize | _getter, setter_ | No docstring. |
| dbc | _getter_ | No docstring. |
| description | _getter_ | No docstring. |
| lastrowid | _getter_ | No docstring. |
| row\_factory | _getter, setter_ | No docstring. |
| rowcount | _getter_ | No docstring. |

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

# Methods within class
Here are methods exposed in the class:
- [\_\_init\_\_](#__init__)
- [close](#close)
- [execute](#execute)
- [executemany](#executemany)
- [executescript](#executescript)
- [fetch](#fetch)
- [fetchall](#fetchall)
- [fetchmany](#fetchmany)
- [fetchone](#fetchone)
- [get\_columns](#get_columns)
- [setinputsizes](#setinputsizes)
- [setoutputsize](#setoutputsize)

## \_\_init\_\_
Initialize self.  See help(type(self)) for accurate signature.

```python
def __init__(self, dbc, conn):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## close
No docstring

```python
def close(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## execute
No docstring

```python
def execute(self, sql, params=None, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## executemany
No docstring

```python
def executemany(self, sql, params=None, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## executescript
No docstring

```python
def executescript(self, sql_script, /, transaction_mode=<TransactionMode.DEFERRED: 'DEFERRED'>):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## fetch
No docstring

```python
def fetch(self, limit=None, buffer_size=None):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## fetchall
No docstring

```python
def fetchall(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## fetchmany
No docstring

```python
def fetchmany(self, size=None):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## fetchone
No docstring

```python
def fetchone(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## get\_columns
No docstring

```python
def get_columns(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## setinputsizes
Required by the DB-API. Does nothing in sqlite3.

```python
def setinputsizes(self, sizes, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## setoutputsize
Required by the DB-API. Does nothing in sqlite3.

```python
def setoutputsize(size, column=None, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>
