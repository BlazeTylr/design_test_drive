# {{PROBLEM}} Function Design Recipe

Copy this into a `recipe.md` in your project and fill it out.

## 1. Describe the Problem

As a user
So that I can keep track of my tasks
I want to check if a text includes the string `#TODO`.

## 2. Design the Function Signature

Include the name of the function, its parameters, return value, and side effects.
def task_todo(string):
return True if it is containing the #TODO
return False if #TODO not present

```python
# EXAMPLE

def task_todo(mixed_words):
    """if #TODO is in the string it will return True

    Parameters: (list all parameters and their types)
        mixed_words: a string containing words (e.g. "hello WORLD")

    Returns: a Boolean value: True or False

```

```python
# If text does contain string '#TODO', it will return True

task_todo('This contains a #TODO') => True

# If text does not contain string '#TODO', it will return False

task_todo('This does not contain a #TODO') => False

_Encode each example as a test. You can add to the above list as you go._
```

## 3. Create Examples as Tests

_Make a list of examples of what the function will take and return._

def test_task_todo_true_check():
actual = #TODO
expected = #TODO
the test will compare actual and expected and if they are the same the test will pass

def test_task_todo_true_missing():
actual = todo is not in the string
expected = todo
the test will pass if actual and expected not the same

## 4. Implement the Behaviour

_After each test you write, follow the test-driving process of red, green, refactor to implement the behaviour._

Here's an example for you to start with:

```python
# EXAMPLE
def test_task_todo_contains_todo():
    result = task_todo('This contains a #TODO')
    assert result is True

def test_task_todo_no_todo():
    result = task_todo('This does not contain a #TODO')
    assert result is False


```
