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
