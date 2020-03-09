---
title: Ruby Structs
description: Example usage of structs in Ruby
header: Ruby Structs Example
---
Structs are a built-in Ruby class that can act like a custom class.  They are great for testing, debugging and playing.

```ruby
LunchOrder = Struct.new(:name, :drink, :food)
event_order = []
event_order << LunchOrder.new('hakeem', 'water', 'Mixed Veggie')
event_order << LunchOrder.new('selena', 'mango lasse', 'Bangkok Dumplings')
event_order << LunchOrder.new('jingyan', 'tea', 'Yellow Curry')
drinks = event_order.map(&:drink)
```

Structs are compared by value equality rather than referential equality.  If two struct objects have the same value they are equal. Classes with the same values are not equal.

### references

[https://www.leighhalliday.com/ruby-struct](https://www.leighhalliday.com/ruby-struct)

[https://blog.bigbinary.com/2018/01/16/ruby-2-5-allows-creating-structs-with-keyword-arguments.html](https://blog.bigbinary.com/2018/01/16/ruby-2-5-allows-creating-structs-with-keyword-arguments.html)

#### Keyword parameters in structs were introduced in Ruby 2.5