* print does not add a line return
* puts add a line return at the end of line


* ruby -e 'print 123'  #puts 123 from command line
* ruby file.rb # run ruby code in a file
* irb # the Interactive Ruby Shell
* irb --simple-prompt #simple prompt
* nil ==> Ruby version of null

"String".reverse

http://ruby-doc.org/core is the language documents for Ruby core
The above function definition can be found at http://ruby-doc.org/core-2.4.2/String.html

*ri String#reverse ??? Not working??

```ruby
puts 123 ```


## variables
  * variable's name
   * bad ones: var-some var_Some varSome aw_count * what's aw??  
   * good atricle_written snake_count

  * variable scope
   * Global $variable
   * Class @@variable
   * Instance @variable
   * Local variable
   * Block variable
## numbers
  * ``` 12345.6789.round ``` => 12346
  * ``` 12345.6789.to_i  ``` => 12345
  * ``` 12345.6789.ceil ``` => 12346
  * ``` 12345.6789.floor  ``` => 12345

## String
  * "Hello"
  * "1" * 5 ==> 11111
  * ```"\'"  ``` ====> escape \

## Array
  * data_set = []
  * data_set = ['a', 'b', 'c']
  * ``` data_set[1]  ``` =>> b
  * ```data_set << 'e' ``` # add new element to the end of array
  * ``` data_set.clear ``` clear the array to be empty
  * ``` data_set = nill ``` set the variable to be null, no longer an array

## Array methods
  * array.join
  * array.join(",")
  * String.split(",") ==> using , to split a string and convert it to an array
   *   ``` x = "1,2,3,4,5" ```
   * ``` y = x.split(",")  ```
   * ``` y.length ``` ==> 5
   * ``` y = x.split(" ") ``` using ' ' space to split x, one element
   *  ``` y.length ``` ==> 1

  * array.inspect
  * array.sort
  * array.uniq
  * array.sort! ==> write the result back to the original array
  * array.delete_at(2) ==> delete element at the index
  * array.delete(4) ==> delete element
  * array.push
  * array.pop ==> pop the last element
  * array.pop(4) ==> pop the last 4 elements
