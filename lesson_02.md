## Lesson 02 Homework Assignment

### Fork this [Repo](https://github.com/ROR101KG-0416/lesson-02-homework)
### Code Reading

<!-- Add a comment (a line starting with `#` ) before each line explaining what it does. Add a comment before the method name explaining, in plain english, what the method does. Try copying and pasting this into a ruby file and modifying it to help you figure it out. Try adding "puts" lines in at different places to see what happens.
 -->
<!-- ```ruby
#def=Method, assigning to full_name 3 different variables -->
def full_name(first_name, last_name, title)
  <!-- # Example comment line

  #name assigned as nil -->
  name = nil
  
  <!-- #setting the first scenario/condition when running code,if it comes true then puts the tittle first then space, first name, space then last name. -->
  if title && first_name && last_name
    name = title + " " + first_name + " " + last_name
 <!-- this send case is only when given title and last name -->
  elsif title && last_name
    name = title + " " + last_name
    <!-- the third condition with first and last name -->
  elsif first_name && last_name
    name = first_name + " " + last_name
    <!-- only the first name -->
  elsif first_name
    name = first_name
    <!-- otherwhise just comes as this line of sentence telling that the name wasnt writen properly -->
  else
    raise "Oh no, that doesn't look like a name"
  end
  <!-- prints the correct statement that matched the code above -->
  return name
  <!-- closing the def method -->
end
```

### Fix Broken Code

The following code contains some errors and some coding ettiquette issues. Fix and refactor the code so that it works and is more clear.

```ruby

def full_name(f, l)
  puts f + " " + l
end

puts full_name("bubba", "chuck")

```

### Coding

1. Write a method called `add` that does the following:
  - takes two parameters and adds them together returning the result. For example `add(1, 2)` should return `3`. 
  - Add a line that calls your add function with two values, stores the result in a variable, and then prints the result to the screen.

  def add(num1,num2)
   
    total = num1 + num2
    total
 

  end 

  puts add(1,2)





2. Write a method, `join_strings` that does the following: 
  - takes two string values as parameters and joins them together with a space in between, returning the result. 
  - For example `join_strings("hello", "dolly")` should return `"hello dolly"`


def join_strings(a, b)
  puts a + " " + b
end

puts join_strings("Handsome", "Man")


3. Write a method called 'old_enough_to_vote?' that does the following:
  - Takes a integer year as a parameter and returns a "yes" if a person born in that year is old enough to vote or returns "no" if the person is not old enough to vote

def old_enough_to_vote?(i)

  if i >= 18

   puts "yes"

  else 
 
   puts "no" 

  end

end   

  puts old_enough_to_vote?(27)


### Reading/Active Learning Assignment

- Complete RubyMonk's **Ruby Primer** interactive tutorial found [here](https://rubymonk.com/learning/books/1-ruby-primer)
- **Install Rails** - follow the instructions found [here](http://installrails.com/)
