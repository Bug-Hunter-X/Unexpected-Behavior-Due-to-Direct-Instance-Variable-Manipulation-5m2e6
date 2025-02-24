# Unexpected Behavior Due to Direct Instance Variable Manipulation in Ruby

This repository demonstrates a common issue in Ruby: directly manipulating instance variables outside the class definition. This practice can lead to unexpected behavior, break encapsulation, and make code more difficult to debug and maintain.

The `bug.rb` file shows how instance variables are accessed directly using `instance_variable_set` and `instance_variable_get`.  This bypasses the class's methods, potentially creating inconsistencies and side effects. 

The solution (`bugSolution.rb`) demonstrates the preferred approach: using accessor methods to interact with instance variables. This approach improves code organization, maintainability, and prevents accidental modifications.