# nonrepeat

Generate non-repeat filenames, ids and strings.

## Installation

```commandline
pip install nonrepeat
```

## Usage

```python
>>> import os
>>> os.listdir(os.getcwd())
['foo.bar', 'foo0.bar']
>>> from nonrepeat import nonrepeat_filename
>>> nonrepeat_filename('foo.bar')
'foo1.bar'
>>> from nonrepeat import nonrepeat
>>> nonrepeat('foo', pool=['foo', 'foo0', 'foo1'])
'foo2'
```
