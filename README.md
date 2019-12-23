# CustomCache.py
A python cache decorator with extra features like clearing cache and updating a key and more

In one of my projects I needed a cache tool to cache some values from an sql query so I wouldn't need to execute a query I've already have done it before. But in some specific cases I shouldv'e update the database with new values and in those cases, cache stayed unupdated and would return old values. I haven't found a feature in other cache tools to update a value in cache, so I decided to create my own.

It's a decorator. So you can just import the class in your project and use it like this:

```
from custom_cache import CustomCache

@CustomCache
def test_cache(x):
    return x*10

```
