###### LiteDBC API Reference
[Home](/docs/api/README.md) | [Project](/README.md) | Module | [Source](/src/litedbc/__init__.py)

# Module Overview
> Module: **litedbc.\_\_init\_\_**

Dbc class, useful functions and exception classes

## Fields
- [**All fields**](/docs/api/modules/litedbc/__init__/fields.md)
    - sqlite = `<module 'sqlite3' from '/usr/lib/python3.12/sqlite3/__init__.py'>`

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## Classes
- [**ColumnInfo**](/docs/api/modules/litedbc/__init__/class-ColumnInfo.md): ColumnInfo(cid, name, type, not_null, default, primary_key, foreign_key, index_info)
    - cid: Alias for field number 0
    - name: Alias for field number 1
    - type: Alias for field number 2
    - not\_null: Alias for field number 3
    - default: Alias for field number 4
    - primary\_key: Alias for field number 5
    - foreign\_key: Alias for field number 6
    - index\_info: Alias for field number 7
- [**Cursor**](/docs/api/modules/litedbc/__init__/class-Cursor.md): When the cursor context is not nested, i.e., not created within a transaction, it will `ROLLBACK` a pending transaction when you...
    - [arraysize](/docs/api/modules/litedbc/__init__/class-Cursor.md#properties-table); _getter, setter_
    - [dbc](/docs/api/modules/litedbc/__init__/class-Cursor.md#properties-table); _getter_
    - [description](/docs/api/modules/litedbc/__init__/class-Cursor.md#properties-table); _getter_
    - [lastrowid](/docs/api/modules/litedbc/__init__/class-Cursor.md#properties-table); _getter_
    - [row\_factory](/docs/api/modules/litedbc/__init__/class-Cursor.md#properties-table); _getter, setter_
    - [rowcount](/docs/api/modules/litedbc/__init__/class-Cursor.md#properties-table); _getter_
    - [close](/docs/api/modules/litedbc/__init__/class-Cursor.md#close): No docstring.
    - [execute](/docs/api/modules/litedbc/__init__/class-Cursor.md#execute): No docstring.
    - [executemany](/docs/api/modules/litedbc/__init__/class-Cursor.md#executemany): No docstring.
    - [executescript](/docs/api/modules/litedbc/__init__/class-Cursor.md#executescript): No docstring.
    - [fetch](/docs/api/modules/litedbc/__init__/class-Cursor.md#fetch): No docstring.
    - [fetchall](/docs/api/modules/litedbc/__init__/class-Cursor.md#fetchall): No docstring.
    - [fetchmany](/docs/api/modules/litedbc/__init__/class-Cursor.md#fetchmany): No docstring.
    - [fetchone](/docs/api/modules/litedbc/__init__/class-Cursor.md#fetchone): No docstring.
    - [get\_columns](/docs/api/modules/litedbc/__init__/class-Cursor.md#get_columns): No docstring.
    - [setinputsizes](/docs/api/modules/litedbc/__init__/class-Cursor.md#setinputsizes): Required by the DB-API. Does nothing in sqlite3.
    - [setoutputsize](/docs/api/modules/litedbc/__init__/class-Cursor.md#setoutputsize): Required by the DB-API. Does nothing in sqlite3.
- [**JournalMode**](/docs/api/modules/litedbc/__init__/class-JournalMode.md): Create a collection of name/value pairs.
    - DELETE = `'DELETE'`
    - TRUNCATE = `'TRUNCATE'`
    - PERSIST = `'PERSIST'`
    - MEMORY = `'MEMORY'`
    - WAL = `'WAL'`
    - OFF = `'OFF'`
- [**LiteDBC**](/docs/api/modules/litedbc/__init__/class-LiteDBC.md): Database connector
    - [auto\_create](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [cached\_statements](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [detect\_types](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [filename](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [in\_memory](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [in\_transaction](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [init\_script](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [is\_closed](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [is\_destroyed](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [is\_new](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [is\_readonly](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [on\_create\_conn](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [on\_create\_db](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [row\_factory](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [text\_factory](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [timeout](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [total\_changes](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [write\_lock](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#properties-table); _getter_
    - [backup](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#backup): Create a backup
    - [blobopen](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#blobopen): From Python 3.11
    - [close](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#close): Closes the connection
    - [copy](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#copy): Creates a new Dbc for the same database file
    - [create\_aggregate](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#create_aggregate): No docstring.
    - [create\_collation](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#create_collation): No docstring.
    - [create\_function](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#create_function): No docstring.
    - [create\_window\_function](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#create_window_function): No docstring.
    - [cursor](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#cursor): Returns a context manager
    - [deferred\_transaction](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#deferred_transaction): Returns a context manager
    - [deserialize](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#deserialize): No docstring.
    - [destroy](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#destroy): Destroy the underlying database file
    - [dump](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#dump): Export the database:
    - [enable\_load\_extension](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#enable_load_extension): No docstring.
    - [exclusive\_transaction](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#exclusive_transaction): Returns a context manager
    - [execute](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#execute): No docstring.
    - [executemany](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#executemany): No docstring.
    - [executescript](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#executescript): No docstring.
    - [get\_journal\_mode](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#get_journal_mode): No docstring.
    - [get\_locking\_mode](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#get_locking_mode): No docstring.
    - [get\_sync\_mode](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#get_sync_mode): No docstring.
    - [getconfig](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#getconfig): No docstring.
    - [getlimit](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#getlimit): No docstring.
    - [immediate\_transaction](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#immediate_transaction): Returns a context manager
    - [inspect](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#inspect): Returns information about the columns of a given table
    - [interrupt](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#interrupt): No docstring.
    - [iterdump](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#iterdump): No docstring.
    - [list\_tables](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#list_tables): Returns a tuple list of tables names.
    - [load\_extension](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#load_extension): No docstring.
    - [match](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#match): Match two database via their connectors. All tables defined in alpha_dbc should be in beta_dbc that might have additional tables...
    - [serialize](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#serialize): No docstring.
    - [set\_authorizer](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#set_authorizer): No docstring.
    - [set\_journal\_mode](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#set_journal_mode): No docstring.
    - [set\_locking\_mode](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#set_locking_mode): No docstring.
    - [set\_progress\_handler](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#set_progress_handler): No docstring.
    - [set\_sync\_mode](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#set_sync_mode): No docstring.
    - [set\_trace\_callback](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#set_trace_callback): No docstring.
    - [setconfig](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#setconfig): No docstring.
    - [setlimit](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#setlimit): No docstring.
    - [transaction](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#transaction): Returns a context manager
    - [vacuum](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#vacuum): No docstring.
    - [vacuum\_into](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#vacuum_into): No docstring.
    - [\_connect](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#_connect): No docstring.
    - [\_create\_conn\_config](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#_create_conn_config): No docstring.
    - [\_create\_connection](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#_create_connection): No docstring.
    - [\_get\_foreign\_keys](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#_get_foreign_keys): No docstring.
    - [\_get\_indexes](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#_get_indexes): No docstring.
    - [\_setup](/docs/api/modules/litedbc/__init__/class-LiteDBC.md#_setup): No docstring.
- [**LockingMode**](/docs/api/modules/litedbc/__init__/class-LockingMode.md): Create a collection of name/value pairs.
    - NORMAL = `'NORMAL'`
    - EXCLUSIVE = `'EXCLUSIVE'`
- [**SyncMode**](/docs/api/modules/litedbc/__init__/class-SyncMode.md): Create a collection of name/value pairs.
    - EXTRA = `'EXTRA'`
    - FULL = `'FULL'`
    - NORMAL = `'NORMAL'`
    - OFF = `'OFF'`
- [**Transaction**](/docs/api/modules/litedbc/__init__/class-Transaction.md): No docstring.
    - [cursor](/docs/api/modules/litedbc/__init__/class-Transaction.md#properties-table); _getter_
    - [dbc](/docs/api/modules/litedbc/__init__/class-Transaction.md#properties-table); _getter_
    - [mode](/docs/api/modules/litedbc/__init__/class-Transaction.md#properties-table); _getter_
- [**TransactionMode**](/docs/api/modules/litedbc/__init__/class-TransactionMode.md): Create a collection of name/value pairs.
    - DEFERRED = `'DEFERRED'`
    - IMMEDIATE = `'IMMEDIATE'`
    - EXCLUSIVE = `'EXCLUSIVE'`

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>
