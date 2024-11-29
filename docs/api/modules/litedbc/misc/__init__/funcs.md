###### LiteDBC API Reference
[Home](/docs/api/README.md) | [Project](/README.md) | [Module](/docs/api/modules/litedbc/misc/__init__/README.md) | [Source](/src/litedbc/misc/__init__.py)

# Functions within module
> Module: [litedbc.misc.\_\_init\_\_](/docs/api/modules/litedbc/misc/__init__/README.md)

Here are functions exposed in the module:
- [ensure\_db\_filename](#ensure_db_filename)
- [ensure\_parent\_dir](#ensure_parent_dir)
- [get\_readonly\_value](#get_readonly_value)
- [get\_start\_transaction\_stmt](#get_start_transaction_stmt)
- [is\_stmt](#is_stmt)
- [match](#match)

## ensure\_db\_filename
No docstring

```python
def ensure_db_filename(filename):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## ensure\_parent\_dir
No docstring

```python
def ensure_parent_dir(filename):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## get\_readonly\_value
No docstring

```python
def get_readonly_value(filename, is_readonly):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## get\_start\_transaction\_stmt
No docstring

```python
def get_start_transaction_stmt(isolation_level):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## is\_stmt
No docstring

```python
def is_stmt(name, sql):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>

## match
Match two database via their connectors.
All tables defined in alpha_dbc should be in beta_dbc that might have additional tables.

```python
def match(alpha_dbc, beta_dbc):
    ...
```

<p align="right"><a href="#litedbc-api-reference">Back to top</a></p>
