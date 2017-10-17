# class

``` ruby
class Animal
  attr_accessor :name  # with both getter and setter
  attr_writer :color   # setter only
  attr_reader :legs, :arms # getter only

  # class scope variables
  @@species = ['cat', 'cow', 'dog', 'duck', 'horse', 'pig']
  @@current_animals = []

  # @@species should be access by self.
  def self.species # getter
    @@species
  end

  def self.species=(array=[]) # setter
    @@species = array
  end

  def self.current_animals # getter
    @@current_animals
  end

  def self.create_with_attributes(noise, color) #
    animal = self.new(noise) # create a new animal with specified noise by calling the default constructor
    animal.color = color # set the color of the animal
    return animal
  end
# invoking the above method
# animal2 = Animal.create_with_attributes("Quack!", "white")

  def initialize(noise, legs=4, arms=0) # default constructor 
    @noise = noise
    @legs = legs
    @arms = arms
    @@current_animals << self # put current_animal into class scope array
    puts "A new animal has been instantiated."
  end

  def noise=(noise) # define = method , setter
    @noise = noise
  end

  def noise # getter
    @noise
  end

  def color # getter for color, other than a default getter
    "The color is #{@color}."
  end
end

class Cow < Animal # sub-class Cow
  def color
    "The cow's color is #{@color}."
  end
  def color # second definition replaces the first
    "My color is #{@color}."
  end
end

class Pig < Animal
  def noise # override the parent_noise method
    parent_noise = super
    return "Hello and also #{parent_noise}"
  end
end

```
