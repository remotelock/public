# Ruby full-stack Technical Evaluation

Code quality is very important to us. We're sending you this challenge so that
we can evaluate your coding skills with Ruby.

### Instructions

- Use the test framework you're most familiar with
- Don't use any gem to accomplish the solution (except test framework)
- Use anything you need from Ruby standard library

### What we expect from your code

- Object-oriented
- Clean code
- Consistent style
- Extensibility
- Maintainability
- Testability

# The challenge

Write a code to parse data represented in different formats and normalize to the following format:

  `<first name> <city name> <birth date M/D/YYYY>`

### Template code

```ruby
# File: app.rb

# WRITE YOUR CLASSES HERE

class PeopleController
  def self.normalize(request_params)
    # FIXME
  end
end

PeopleController.normalize({
  comma: [ # Fields: first name, city name, birth date
    'Mckayla, Atlanta, 5/29/1986',
    'Elliot, New York City, 4/3/1947',
  ],
  dollar: [ # Fields: city abbreviation, birth date, last name, first name
    'LA $ 10-4-1974 $ Nolan $ Rhiannon',
    'NYC $ 12-1-1962 $ Bruen $ Rigoberto',
  ],
})

# Expected return (order of entries doesn't matter):
# [
#   'Mckayla Atlanta 5/29/1986',
#   'Elliot New York City 4/3/1947',
#   'Rhiannon Los Angeles 10/4/1974',
#   'Rigoberto New York City 12/1/1962',
# ]


# WRITE YOUR SPECS HERE
```

# Deliverable

**One** file `app.rb` hosted in [GitHub Gist](http://gist.github.com) or similar
service, where we can view the solution with a single click.

**Don't worry about sending Gemfile[.lock]**
