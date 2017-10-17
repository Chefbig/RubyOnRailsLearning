
# find

* ```(1..10).find {|i| i == 5} ``` => 5
* ```(1..10).find {|i| i % 3} ``` => 3
* ```(1..10).detect {|i| i % 3} ``` => 3
* ```(1..10).find_all {|i| i % 3} ``` => [3, 6, 9] # array with all true
* ```(1..10).detect {|i| i % 30} ``` => [] # empty array
* ``` (1..10).any? {|i| i % 3 == 0 } ``` =>true
* ``` (1..10).all? {|i| i % 3 == 0 } ``` =>false
* ``` [*1..10].delete_if {|i| i % 3 == 0 } ``` => [1, 2, 4, 5, 7, 8, 10]


# merge


``` h1 = { "a" => 111, "b" => 222 } ``` => {"a"=>111, "b"=>222}

``` h2 = { "b" => 333, "c" => 444 } ``` => {"b"=>333, "c"=>444}
```
h1.merge(h2) do |key, old, new|
  if old < new
    old
  else
    new
  end
end
```


# collect / map

map will always generate an array
Array#each executes the given block for each element of the array, then returns the array itself.
Array#map also executes the given block for each element of the array, but returns a new array whose values are the return values of each iteration of the block.

# sort
<=>
``` 1 <=> 2 ``` => -1
``` 2 <=> 1 ``` => 1
``` 2 <=> 2 ``` => 0

```
array = [3,1,5,2,4]
# => [3, 1, 5, 2, 4]
array
# => [3, 1, 5, 2, 4]
array.sort {|v1,v2| v1 <=> v2 }
# => [1, 2, 3, 4, 5]
array.sort
# => [1, 2, 3, 4, 5]
array.sort {|v1,v2| v2 <=> v1 }
# => [5, 4, 3, 2, 1]
array.sort.reverse
# => [5, 4, 3, 2, 1]
fruits = ['banana', 'apple', 'orange', 'pear']
# => ["banana", "apple", "orange", "pear"]
fruits.sort
# => ["apple", "banana", "orange", "pear"]
fruits.sort {|fruit1,fruit2| fruit1.length <=> fruit2.length}
# => ["pear", "apple", "orange", "banana"]
fruits.sort_by {|fruit| fruit.length}
# => ["pear", "apple", "orange", "banana"]
fruits.sort_by {|fruit| fruit.reverse }
# => ["banana", "orange", "apple", "pear"]
fruits
# => ["banana", "apple", "orange", "pear"]
fruits.sort! {|fruit1,fruit2| fruit1.length <=> fruit2.length}
# => ["pear", "apple", "orange", "banana"]
fruits
```

# inject

```
array = [*1..10]
# => [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
sum = array.inject {|memo, n| memo + n }
# => 55
sum = array.inject(100) {|memo, n| memo + n }
# => 155

# only get the longest one
fruits = ['apple', 'pear', 'banana', 'plum']
# => ["apple", "pear", "banana", "plum"]
longest_word = fruits.inject do |memo, fruit|
  if memo.length > fruit.length
    memo
  else
    fruit
  end
end
# => "banana"
```
