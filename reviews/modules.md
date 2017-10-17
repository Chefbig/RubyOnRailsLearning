# modules

``` ruby
module ContactInfo
  attr_accessor :first_name, :last_name, :city, :state, :zip_code

  def full_name
    return @first_name + " " + @last_name
  end

  def city_state_zip
    csz = @city
    csz += ", #{@state}" if @state
    csz += "  #{@zip_code}" if @zip_code
    return csz
  end
end

class Person
  include ContactInfo
end

class Teacher
  include ContactInfo
  attr_accessor :lesson_plans
end

class Student < Person
  attr_accessor :books, :grades
end
```

# load
loads a source files every time it is called
``` ruby
load 'file_name.rb'
```

# require
loads a source files only once
```
require 'source.rb'
```

# include

The require method does what include does in most other programming languages: run another file. It also tracks what you've required in the past and won't require the same file twice. To run another file without this added functionality, you can use the load method.

The include method takes all the methods from another module and includes them into the current module. This is a language-level thing as opposed to a file-level thing as with require. The include method is the primary way to "extend" classes with other modules (usually referred to as mix-ins). For example, if your class defines the method "each", you can include the mixin module Enumerable and it can act as a collection. This can be confusing as the include verb is used very differently in other languages.
[Source1](https://web.archive.org/web/20150405161656/http://ruby.about.com/b/2008/10/23/a-quick-peek-at-ruby-include-vs-require.htm)
[Source0](https://stackoverflow.com/questions/318144/what-is-the-difference-between-include-and-require-in-ruby)

So if you just want to use a module, rather than extend it or do a mix-in, then you'll want to use require.
