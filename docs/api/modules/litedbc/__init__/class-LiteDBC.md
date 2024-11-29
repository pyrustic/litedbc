###### LiteDBC API Reference
[Home](/docs/api/README.md) | [Project](/README.md) | [Module](/docs/api/modules/litedbc/__init__/README.md) | [Source](/src/litedbc/__init__.py)

# Class LiteDBC
> Module: [litedbc.\_\_init\_\_](/docs/api/modules/litedbc/__init__/README.md)
>
> Class: **LiteDBC**
>
> Inheritance: `object`

Database connector

## Properties table
Here are properties exposed in the class:

| Property | Methods | Description |
| --- | --- | --- |
| auto\_create | _getter_ | No docstring. |
| cached\_statements | _getter_ | No docstring. |
| detect\_types | _getter_ | No docstring. |
| filename | _getter_ | No docstring. |
| in\_memory | _getter_ | No docstring. |
| in\_transaction | _getter_ | No docstring. |
| init\_script | _getter_ | No docstring. |
| is\_closed | _getter_ | Boolean to tell whether this database is closed or not |
| is\_destroyed | _getter_ | Boolean to tell whether this database has been destroyed via this connection instance or not |
| is\_new | _getter_ | Returns True if the database has just been created, otherwise returns False |
| is\_readonly | _getter_ | No docstring. |
| on\_create\_conn | _getter_ | No docstring. |
| on\_create\_db | _getter_ | No docstring. |
| row\_factory | _getter_ | No docstring. |
| text\_factory | _getter_ | No docstring. |
| timeout | _getter_ | No docstring. |
| total\_changes | _getter_ | No docstring. |
| write\_lock | _getter_ | No docstring. |

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

# Methods within class
Here are methods exposed in the class:
- [\_\_init\_\_](#__init__)
- [backup](#backup)
- [blobopen](#blobopen)
- [close](#close)
- [copy](#copy)
- [create\_aggregate](#create_aggregate)
- [create\_collation](#create_collation)
- [create\_function](#create_function)
- [create\_window\_function](#create_window_function)
- [cursor](#cursor)
- [deferred\_transaction](#deferred_transaction)
- [deserialize](#deserialize)
- [destroy](#destroy)
- [dump](#dump)
- [enable\_load\_extension](#enable_load_extension)
- [exclusive\_transaction](#exclusive_transaction)
- [execute](#execute)
- [executemany](#executemany)
- [executescript](#executescript)
- [get\_journal\_mode](#get_journal_mode)
- [get\_locking\_mode](#get_locking_mode)
- [get\_sync\_mode](#get_sync_mode)
- [getconfig](#getconfig)
- [getlimit](#getlimit)
- [immediate\_transaction](#immediate_transaction)
- [inspect](#inspect)
- [interrupt](#interrupt)
- [iterdump](#iterdump)
- [list\_tables](#list_tables)
- [load\_extension](#load_extension)
- [match](#match)
- [serialize](#serialize)
- [set\_authorizer](#set_authorizer)
- [set\_journal\_mode](#set_journal_mode)
- [set\_locking\_mode](#set_locking_mode)
- [set\_progress\_handler](#set_progress_handler)
- [set\_sync\_mode](#set_sync_mode)
- [set\_trace\_callback](#set_trace_callback)
- [setconfig](#setconfig)
- [setlimit](#setlimit)
- [transaction](#transaction)
- [vacuum](#vacuum)
- [vacuum\_into](#vacuum_into)
- [\_connect](#_connect)
- [\_create\_conn\_config](#_create_conn_config)
- [\_create\_connection](#_create_connection)
- [\_get\_foreign\_keys](#_get_foreign_keys)
- [\_get\_indexes](#_get_indexes)
- [\_setup](#_setup)

## \_\_init\_\_
Init

```python
def __init__(self, filename=None, init_script=None, auto_create=True, is_readonly=False, timeout=5.0, detect_types=0, cached_statements=128, on_create_db=None, on_create_conn=None, row_factory=None, text_factory=None):
    ...
```

| Parameter | Description |
| --- | --- |
| filename | path to SQLite file, either string or a pathlib.Path instance. Leave this parameter to None if you want to create an in-memory database |
| init\_script | SQL script (string) |
| conn\_config | keywords-arguments to pass to sqlite.connect() |
| on\_create\_db | callback called just after the creation of the database, before the execution of init_script and the other on_create_db callback. This callback must accept the dbc instance as argument |
| on\_create\_conn | callback called just after the connection to the database and the execution of on_create_db. This callback must accept the dbc instance as argument |

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## backup
Create a backup

```python
def backup(self, dst, *, pages=-1, progress=None, name='main', sleep=0.25):
    ...
```

| Parameter | Description |
| --- | --- |
| dst | destination filename |

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## blobopen
From Python 3.11

```python
def blobopen(self, table, column, row, /, *, readonly=False, name='main'):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## close
Closes the connection

```python
def close(self):
    ...
```

### Value to return
Returns a boolean

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## copy
Creates a new Dbc for the same database file

```python
def copy(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## create\_aggregate
No docstring

```python
def create_aggregate(self, name, n_args, aggregate_cls, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## create\_collation
No docstring

```python
def create_collation(self, name, func, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## create\_function
No docstring

```python
def create_function(self, name, n_args, func, /, *, deterministic=False):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## create\_window\_function
No docstring

```python
def create_window_function(self, name, n_args, aggregate_cls, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## cursor
Returns a context manager

```python
def cursor(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## deferred\_transaction
Returns a context manager

```python
def deferred_transaction(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## deserialize
No docstring

```python
def deserialize(self, data, /, *, name='main'):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## destroy
Destroy the underlying database file

```python
def destroy(self):
    ...
```

### Value to return
Returns a boolean

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## dump
Export the database:

```python
def dump(self, dst=None):
    ...
```

| Parameter | Description |
| --- | --- |
| dst\_filename | destination filename |

### Value to return
it returns a string of sql code if dst isn't set

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## enable\_load\_extension
No docstring

```python
def enable_load_extension(self, enabled, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## exclusive\_transaction
Returns a context manager

```python
def exclusive_transaction(self):
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

## get\_journal\_mode
No docstring

```python
def get_journal_mode(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## get\_locking\_mode
No docstring

```python
def get_locking_mode(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## get\_sync\_mode
No docstring

```python
def get_sync_mode(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## getconfig
No docstring

```python
def getconfig(self, op, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## getlimit
No docstring

```python
def getlimit(self, category, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## immediate\_transaction
Returns a context manager

```python
def immediate_transaction(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## inspect
Returns information about the columns of a given table

```python
def inspect(self, table):
    ...
```

| Parameter | Description |
| --- | --- |
| table | name of the table to inspect |

### Value to return
Returns a tuple containing ColumnInfo instances.
A ColumnInfo instance is a namedtuple:
    namedtuple(col_id, name, type, not_null, default, primary_key, foreign_key, index_info)

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## interrupt
No docstring

```python
def interrupt(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## iterdump
No docstring

```python
def iterdump(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## list\_tables
Returns a tuple list of tables names.

```python
def list_tables(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## load\_extension
No docstring

```python
def load_extension(self, path, /, *, entrypoint=None):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## match
Match two database via their connectors.
All tables defined in alpha_dbc should be in beta_dbc that might have additional tables.

```python
def match(self, target_dbc):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## serialize
No docstring

```python
def serialize(self, *, name='main'):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## set\_authorizer
No docstring

```python
def set_authorizer(self, callback):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## set\_journal\_mode
No docstring

```python
def set_journal_mode(self, journal_mode):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## set\_locking\_mode
No docstring

```python
def set_locking_mode(self, locking_mode):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## set\_progress\_handler
No docstring

```python
def set_progress_handler(self, callback, n):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## set\_sync\_mode
No docstring

```python
def set_sync_mode(self, sync_mode):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## set\_trace\_callback
No docstring

```python
def set_trace_callback(self, callback):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## setconfig
No docstring

```python
def setconfig(self, op, enable=True, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## setlimit
No docstring

```python
def setlimit(self, category, limit, /):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## transaction
Returns a context manager

```python
def transaction(self, transaction_mode=<TransactionMode.DEFERRED: 'DEFERRED'>):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## vacuum
No docstring

```python
def vacuum(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## vacuum\_into
No docstring

```python
def vacuum_into(self, dst):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_connect
No docstring

```python
def _connect(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_create\_conn\_config
No docstring

```python
def _create_conn_config(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_create\_connection
No docstring

```python
def _create_connection(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_get\_foreign\_keys
No docstring

```python
def _get_foreign_keys(self, table):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_get\_indexes
No docstring

```python
def _get_indexes(self, table):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## \_setup
No docstring

```python
def _setup(self):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>
