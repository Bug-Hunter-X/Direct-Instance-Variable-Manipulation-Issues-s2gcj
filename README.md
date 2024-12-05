# Ruby Instance Variable Gotcha
This example demonstrates a potential issue when directly manipulating instance variables in Ruby using `instance_variable_set` and `instance_variable_get`. While these methods can be useful in certain scenarios, they can break encapsulation and lead to unexpected behavior if not used with caution.  The `bug.rb` file shows the problem; `bugSolution.rb` offers a more robust approach.

**How to reproduce:**
1. Run `bug.rb`.
2. Observe that the output changes unexpectedly.  This happens because we're bypassing the class's methods to alter the instance variable directly.

**Key takeaway:** Favour using methods to interact with object's internal state to maintain code clarity, predictability and better maintainability.