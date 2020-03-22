---
title: Why Ruby Methods Return 'nil'
description: The reason why Ruby methods return 'nil'
header: Why Ruby Methods Return 'nil'
---

In Ruby, the `return` keyword stops the execution flow of a method.  It's 
commonly used with guard clauses, which are a conditional statement at the 
top of a function.

```ruby
def currency(minor_currency)
  return "0.00" unless minor_currency.class == Integer
  major_currency = minor_currency / 100.to_f
  '%.2f' % major_currency
end

currency(1999) # 19.99
```

The return keyword specifies the object to be returned to the caller when the method has done its work. 

If no return keyword is specified, the object created by the last line in the method is automatically treated as the return value. A method must always return exactly one object.

Calling return without specifying an object to return results in a nil, which is returned by default. 

### references

[https://www.thechrisoshow.com/2009/02/16/using-guard-clauses-in-your-ruby-code/](https://www.thechrisoshow.com/2009/02/16/using-guard-clauses-in-your-ruby-code/)

