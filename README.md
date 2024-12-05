# Ruby Bug: Direct Modification of Instance Variables

This repository demonstrates a common Ruby bug: the unexpected behavior that can result from directly modifying instance variables using `instance_variable_set` or `instance_variable_get`.  Directly accessing instance variables circumvents accessor methods and can lead to maintenance difficulties and unexpected program behavior.

The `bug.rb` file illustrates the problem. The `bugSolution.rb` demonstrates a more robust and maintainable approach using accessor methods.

## How to Reproduce

1. Clone this repository.
2. Run `ruby bug.rb` to see the unexpected output.
3. Run `ruby bugSolution.rb` to see the solution.

## Solution

Always use accessor methods (`attr_accessor`, `attr_reader`, `attr_writer`) to interact with instance variables.  This ensures better encapsulation, maintainability, and prevents unintended side effects.