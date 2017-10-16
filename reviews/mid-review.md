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
puts 123


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
