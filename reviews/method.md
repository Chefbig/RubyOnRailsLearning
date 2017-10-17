# require

require a file with functions defined in it
``` require "file_name_with_method_defined.rb" ```

```ruby
def welcome
	puts "Hello World!"
end

```

``` ruby
def welcome(name)
	puts "Hello #{name}!"
end
welcome("Mary")
```


``` ruby
def welcome(name = "World")
	puts "Hello #{name}!"
end

welcome
# Hello World
welcome("Mary")
# Hello Mary
```

# syntactic sugar
``` ruby
puts 8 ** 2
puts 8.**(2)

array1 = [1,2,3]
puts array1.inspect
array2 = [1,2,3]
puts array2.inspect

array1 << 4
puts array1.inspect
array2.<<(4)
puts array2.inspect

```
