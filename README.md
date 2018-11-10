![GA Logo](https://camo.githubusercontent.com/6ce15b81c1f06d716d753a61f5db22375fa684da/68747470733a2f2f67612d646173682e73332e616d617a6f6e6177732e636f6d2f70726f64756374696f6e2f6173736574732f6c6f676f2d39663838616536633963333837313639306533333238306663663535376633332e706e67)

# Ruby Language Weekend Homework

## PART 1! THE REPS

These problems better look familiar to you.  It's perfectly fine to look back at your JavaScript answers to this from Unit 1 and use the same algorithms to just rewrite a solution in Ruby.  

### 1. `lengths`

Write a method `lengths` that accepts a single parameter as an argument, namely an array of strings. The method should return an array of numbers. Each number in the array should be the length of the corresponding string.

```ruby
words = ["hello", "what", "is", "up", "dude"]
lengths(words)  # => [5, 4, 2, 2, 4]
```

### Commit!

---

### 2. `transmogrifier`

Write a Ruby method called `transmogrifier`
This method should accept three arguments, which you can assume will be numbers.
Your method should return the "transmogrified" result

The transmogrified result of three numbers is the product (numbers multiplied together) of the first two numbers, raised to the power (exponentially) of the third number.

For example, the transmogrified result of 5, 3, and 2 is `(5 times 3) to the power of 2` is 225.

Use your method to find the following answers.


```ruby
transmogrifier(5, 4, 3)
transmogrifier(13, 12, 5)
transmogrifier(42, 13, 7)
```

### Commit!

---

### 3. `toonify`

Write a method called `toonify` that takes two parameters, `accent` and `sentence`.
- If `accent` is the string `"daffy"`, return a modified version of `sentence` with all "s" replaced with "th".
- If the accent is `"elmer"`, replace all "r" with "w".
- Feel free to add your own accents as well!
- If the accent is not recognized, just return the sentence as-is.


```ruby
toonify("daffy", "so you smell like sausage")
#=> "tho you thmell like thauthage"
```

### Commit!

---

### 4. `word_reverse`

Write a method `word_reverse` that accepts a single argument, a string. The method should return a string with the order of the words reversed. Don't worry
about punctuation.

```ruby
word_reverse("Now I know what a TV dinner feels like")
# => "like feels dinner TV a what know I Now"
```

### Commit!

---

### 5. `letter_reverse`

Write a method `letter_reverse` that accepts a single argument, a string. The method should maintain the order of words in the string but reverse the letters in each word. Don't worry about punctuation. This will be very similar to round 4 except you won't need to split them with a space.

```ruby
letter_reverse("Now I know what a TV dinner feels like")
# => "woN I wonk tahw a VT rennid sleef ekil"
letter_reverse("Put Hans back on the line")
# => "tuP snaH kcab no eht enil"
```

### Commit!

---

### 6. `longest`

Write a method `longest` that accepts a single argument, an array of strings. The method should return the longest word in the array. In case of a tie, the method should return either.

```ruby
longest(["oh", "good", "grief"]) # => "grief"
longest(["Nothing" , "takes", "the", "taste", "out", "of", "peanut", "butter", "quite", "like", "unrequited", "love"])
# => "unrequited"
```

### Commit!

---

### 7. `check_prime?` & `get_primes` 

* Write a method called `check_prime?` that will test whether a number is Prime. The method will return true if Prime, false if not.

* Write another method called `get_primes` that will print all the Primes up to an arbitrary limit. For example, if you invoke your method with `get_primes 100`, it will print all the Prime numbers up to and including 100. This method can call on the previous `check_prime?` method.

> Hints/reminders/notes: A Prime number is a number that is not evenly divisible by another number except 1 and itself. To test whether a number is Prime, you only need to test as far as the **square root** of that number. This is advisable for optimization and testing large numbers.


When you've completed the problem (and no sooner!), check this out:
<details>
Check out [Ruby's `Prime` class](http://ruby-doc.org/stdlib-2.4.1/libdoc/prime/rdoc/Prime.html)
</details>

### Commit!

---

## PART 2: HANGMAN GAME

Make a hangman ruby console game.  You must have a Word class.  You should also have a `word_array` containing a couple dozen words to randomly choose from.  And then use `loop` for the main game logic with repeated guessing, and `break` when the game is over.  

#### Suggested methods for your Word class

* `initialize` -- perhaps make this take a parameter like `desired_word`
* `check_letter?` and/or `.contains`
* `.print_stats`: This could call the three below 
* `.render` (show with blanks for unguessed letters and letters for guessed letters)
* `.print_remaining_guesses`
* `.print_guessed_letters`

