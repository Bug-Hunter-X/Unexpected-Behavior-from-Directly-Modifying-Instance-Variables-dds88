# Unexpected Behavior from Directly Modifying Instance Variables

This repository demonstrates a common but subtle error in Ruby: directly modifying instance variables using `instance_variable_set`. While functional, this practice can lead to unexpected behavior and make code more difficult to maintain.  It bypasses any potential validation or access control you may have implemented through methods.

The `bug.rb` file illustrates the issue.  The solution is shown in `bugSolution.rb` and uses proper accessor methods for better code structure and maintainability.

## Solution

Use accessor methods (getters and setters) to access and modify instance variables. This provides a controlled way to manage data, allowing for validation, logging, or other actions to be performed before the internal state is altered.