# Homework Week 2

Base your week 2 homework on the result of week 1.

When you are done update your PR from week 1.

## Outline

Extend your todo list app with dynamic rendering of items based on the following JSON list:

```json
[
  {
    "id": 1,
    "description": "Get out of bed",
    "deadline": "2017-09-11",
    "done": true
  },
  {
    "id": 2,
    "description": "Brush teeth",
    "deadline": "2017-09-10",
    "done": false
  },
  {
    "id": 3,
    "description": "Eat breakfast",
    "deadline": "2017-09-09",
    "done": false
  }
]
```

The JSON list should be in the **state** of the `App` component. Create a checkbox in each todo item. When you click the checkbox, the done state of the item should change. When an item is marked as done, it should be rendered with a `line-through` decoration. A mockup of the end result is the following:

```
Todo List

* [x] Get-out-of-bed,-Wed-Sep-13-2017
* [ ] Brush teeth, Thu Sep 14 2017
* [ ] Eat breakfast, Fri Sep 15 2017
```

When there are no items, the todo app should render the text "No items...":

```
Todo List

No items...
```

## Extra

- Add a delete button behind every item
- Add a checkbox 'hide done todo's' above the list, that when you click/check it, it should filter out all items with `done === false`
- Add a input search field above the list, which you could filter the todo list on the description field

## Extra II

Go back to the github repo example we're used in our class.
- Remove the click event (deleteRepo) on a repoItem
- On click on a repoItem show more information of that item and show a delete button where you add the deleteRepo event again
- The Repo Component will need a state to hold the state of showing more or less information.