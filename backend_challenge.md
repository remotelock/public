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
PIPE_ENTRIES = [ # Birth date, First name, City - Feature for next sprint!!!
  '10.24.1990 | Joseph | New York City',
  '1.15.1995 | Jane | Denver'
]

class App
  def self.run(comma: [], dollar: [], pipe: [])
    # invoke your magical classes here
  end
end

App.run(comma: COMMA_ENTRIES, dollar: DOLLAR_ENTRIES, pipe: PIPE_ENTRIES)

# Expected output: <First name> <City> <Birth date> (ordered by city)
#   Elliot New York City 4/3/1947
#   Jane Denver 10/24/1990
#   Joseph New York City 1/15/1995
#   Mckayla Atlanta 5/29/1986
#   Rhiannon Los Angeles 10/4/1974
#   Rigoberto New York City 12/1/1962
```

# Deliverable

**One** file `app.rb` hosted in [GitHub Gist](http://gist.github.com) or similar
service, where we can view the solution with a single click.

**Don't worry about sending Gemfile[.lock]**
