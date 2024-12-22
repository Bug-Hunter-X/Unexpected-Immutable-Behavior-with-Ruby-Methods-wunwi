# Unexpected Immutable Behavior in Ruby

This example demonstrates a common pitfall in Ruby where a method that looks like a getter might not be acting like a setter.

**The Problem:**
The `value` method in the `MyClass` only allows reading the `@value` instance variable.  Attempting to assign a new value (`my_object.value = 20`) has no effect; this is not setting a new value.