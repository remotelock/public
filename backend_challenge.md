# Ruby full-stack Technical Evaluation

Code quality is very important to us. We're sending you this challenge so that
we can evaluate your coding skills with Ruby.

### What we expect from your code

- Object-oriented
- Clean code
- Consistent style
- Extensibility
- Maintainability
- Testability

# The challenge

- Write code to parse data represented in different formats and normalize to the following format:

  `<first name> <city name> <birth date M/D/YYYY>`

- Write at least 2 specs, but no more than 5 - we don't expect 100% coverage

### Instructions

- Use the test framework you're most familiar with
- Use anything you need from Ruby standard library
- Don't use any gem to accomplish the solution (except test framework)
- Don't worry about invalid input data

### Template code

```ruby
# File: app.rb

# WRITE YOUR CLASSES HERE

class PeopleController
  def self.normalize(request_params)
    # TODO
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

### Challenge extension

```ruby
# CHALLENGE EXTENSION
# Important:
#   - Communicate the ideas during the coding
#   - Write at least 1 spec for the extension solution
# Not important:
#   - Being fast is not the most important thing
#   - Don't worry about syntax typos (missing a comma, bracket)
#
# Task:
#   - Parse and normalize the new input format
#   - Sort entries by birth date

PeopleController.normalize({
  comma: [ # Fields: first name, city name, birth date
    'Mckayla, Atlanta, 5/29/1986',
    'Elliot, New York City, 4/3/1947',
  ],
  dollar: [ # Fields: city abbreviation, birth date, last name, first name
    'LA $ 10-4-1974 $ Nolan $ Rhiannon',
    'NYC $ 12-1-1962 $ Bruen $ Rigoberto',
  ],
  pipe: [ # Fields: birth date, first name, city name
    '10.24.1990 | Joseph | New York City',
    '1.15.1995 | Jane | Denver',
  ],
})

# Expected return (sorted by birth date):
# [
#   'Elliot New York City 4/3/1947',
#   'Rigoberto New York City 12/1/1962',
#   'Rhiannon Los Angeles 10/4/1974',
#   'Mckayla Atlanta 5/29/1986',
#   'Joseph New York City 10/24/1990',
#   'Jane Denver 1/15/1995',
# ]
```

# Deliverable

**One** file `app.rb` hosted in [GitHub Gist](http://gist.github.com) or similar
service, where we can view the solution with a single click.

**Don't worry about sending Gemfile[.lock]**
