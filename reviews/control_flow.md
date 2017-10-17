# If

## simple if statement
```
if boolean
end
```
## if elsif
```
if boolean
  do something
  multipile lines
elsif
  do something else
else
  do something else
end
```

## inline condition
``` puts "This is Kevin!" if name == "Kevin" ```

# unless
```
  unless boolean
  ......
  end
```
```
  if !boolean
  ......
  end
```
# case
Using boolean expression, x == 1 , x == 2 ...
```
case
  when boolean
  ...
  when boolean
  ...
  else
  ...
  end
```
Using value expression, x, 1 , 2 ...
```
case test_value
  when value
  ...
  when value
  ...
  else
  ...
  end
```
# Ternary operator

``` boolean ? code1 : code2 ```
``` puts x == 1 ? "one" : "not one" ```

# or / or equals

``` x = y || z ``` assign to y if y exist, or assign it with z

if x don't have a value, assign it with z
```
unless x
  x = z
end
```

# loop

```
loop do
  ...
  break if boolean
  next # jump to next loop
  redo
  retry
end
```
```
while boolean
  ...
end
```

```
unless
  ...
end
```

```
x = 0
puts x += 2 while x < 100

y = 3245
puts y/=2 until y <= 1

```

# Iterators

```
5.times {puts "Hello"}

5.upto(10) {puts "Hello"}

(1..5).each {puts "Hello"}

```

# conclusion

* Integer/floats: times, upto, downto, step
* Range: each, step
* String: each, each_line, each_byte
* Array: each, each_index, each_with_index
* Hash: each, each_key, each_value, each_pair
