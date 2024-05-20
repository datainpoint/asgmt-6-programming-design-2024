# asgmt-6-programming-design-2024
Assignment 6: Programming Design 2024.

## 01. Define a class `ReduceArgs()` which instantiates objects with two methods `summation()` and `product()` that take flexible args and return aggregated result.

```python
class ReduceArgs:
    """
    >>> reduce_args = ReduceArgs(1, 2, 3, 4)
    >>> reduce_args.summation()
    10
    >>> reduce_args.product()
    24
    >>> reduce_args = ReduceArgs(1, 2, 3, 4, 5)
    >>> reduce_args.summation()
    15
    >>> reduce_args.product()
    120
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a class `SortArgs` which instantiates objects with two methods `sort_asc()` and `sort_desc()` that take flexible integers and return a sorted `list`.

```python
class SortArgs:
    """
    >>> sort_args = SortArgs()
    >>> sort_args.sort_asc(1, 2, 0)
    [0, 1, 2]
    >>> sort_args.sort_desc(1, 2, 0)
    [2, 1, 0]
    >>> sort_args.sort_asc(4, 3, 5)
    [3, 4, 5]
    >>> sort_args.sort_desc(4, 3, 5)
    [5, 4, 3]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a class `ReverseKeyValues` which instantiates objects with 2 attributes `keys` and `values`, 1 method `reverse()`.

```python
class ReverseKeyValues:
    """
    >>> reverse_key_values = ReverseKeyValues(twn='Taiwan')
    >>> reverse_key_values.keys
    ['twn']
    >>> reverse_key_values.values
    ['Taiwan']
    >>> reverse_key_values.reverse()
    {'Taiwan': 'twn'}
    >>> reverse_key_values = ReverseKeyValues(twn='Taiwan', jpn='Japan')
    >>> type(reverse_key_values)
    '__main__.ReverseKeyValues'
    >>> reverse_key_values.keys
    ['twn', 'jpn']
    >>> reverse_key_values.values
    ['Taiwan', 'Japan']
    >>> reverse_key_values.reverse()
    {'Taiwan': 'twn', 'Japan': 'jpn'}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a class `FizzBuzz` which instantiates objects with 2 methods `nth_element()` and `generate_sequence()`.

Source: <https://en.wikipedia.org/wiki/Fizz_buzz>

```python
class FizzBuzz:
    """
    >>> fizz_buzz = FizzBuzz()
    >>> fizz_buzz.nth_element(1)
    1
    >>> fizz_buzz.nth_element(3)
    'Fizz'
    >>> fizz_buzz.nth_element(5)
    'Buzz'
    >>> fizz_buzz.nth_element(15)
    'Fizz Buzz'
    >>> fizz_buzz.generate_sequence(5)
    [1, 2, 'Fizz', 4, 'Buzz']
    >>> fizz_buzz.generate_sequence(15)
    [1, 2, 'Fizz', 4, 'Buzz', 'Fizz', 7, 8, 'Fizz', 'Buzz', 11, 'Fizz', 13, 14, 'Fizz Buzz']
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a function `import_teams_json` which imports the `teams.json` as a `dict` in working directory.

```python
def import_teams_json() -> dict:
    """
    >>> teams_json = import_teams_json()
    >>> type(teams_json)
    dict
    >>> len(teams_json["data"])
    30
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 06. Define a function `find_teams_conference_division` which returns a team's conference and division in a `tuple` given team's abbreviation, based on `teams.json` in working directory.

```python
def find_teams_conference_division(team_abb: str) -> tuple:
    """
    >>> find_teams_conference_division("BOS")
    ('East', 'Atlantic')
    >>> find_teams_conference_division("MIA")
    ('East', 'Southeast')
    >>> find_teams_conference_division("LAL")
    ('West', 'Pacific')
    >>> find_teams_conference_division("DEN")
    ('West', 'Northwest')
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Define a function `find_teams_city` which returns a team's city given team's name, based on `teams.json` in working directory.

```python
def find_teams_city(team_name: str) -> str:
    """
    >>> find_teams_city("Celtics")
    'Boston'
    >>> find_teams_city("Heat")
    'Miami'
    >>> find_teams_city("Lakers")
    'Los Angeles'
    >>> find_teams_city("Nuggets")
    'Denver'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `import_movies_csv` which imports the `movies.csv` in working directory with `pandas` module as a `DataFrame`.

```python
def import_movies_csv() -> pd.core.frame.DataFrame:
    """
    >>> movies_csv = import_movies_csv()
    >>> movies_csv.shape
    (250, 6)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `find_min_max_runtime` which finds out the minimum and the maximum runtime given `movies.csv` in working directory.

```python
def find_min_max_runtime():
    """
    >>> min_max_runtime = find_min_max_runtime()
    >>> min_max_runtime["min_runtime"]
    (45, 'Sherlock Jr.')
    >>> min_max_runtime["max_runtime"]
    (238, 'Gone with the Wind')
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `value_counts_parent_guide()` which finds out the number of each parent guide category `movies.csv` in working directory.

```python
def value_counts_parent_guide():
    """
    >>> counts_parent_guide = value_counts_parent_guide()
    >>> counts_parent_guide["R"]
    102
    >>> counts_parent_guide["PG"]
    38
    >>> counts_parent_guide["PG-13"]
    36
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```