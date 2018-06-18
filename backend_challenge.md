# Ruby full-stack Technical Evaluation

Code quality is very important for us. We're sending you this challenge so that
we can evaluate your coding skills with Ruby.

### Instructions

- Use the test framework you're most familiar with
- Don't use any gem to accomplish the solution (except test framework)
- Use anything you need from Ruby standard library

### What we expect from your code

- Object-oriented
- Clean code
- Extensibility
- Maintainability
- Testability

# The challenge

Write a code to parse data represented in different formats and print to standard
output in a single format:

  `<First name> <City> <Birth date>` (line order is not important, but date format is)

### Template code

```ruby
# File: app.rb

COMMA_ENTRIES = [ # First name, City, Birth date
  'Mckayla, Atlanta, 5/29/1986',
  'Elliot, New York City, 4/3/1947',
]
DOLLAR_ENTRIES = [ # City, Birth date, Last name, First name
  'LA $ 10-4-1974 $ Nolan $ Rhiannon',
  'NYC $ 12-1-1962 $ Bruen $ Rigoberto',
]

# WRITE YOUR CLASSES HERE

class App
  def self.run(comma: [], dollar: [])
    # INVOKE YOUR MAGICAL CLASSES HERE
  end
end

App.run(comma: COMMA_ENTRIES, dollar: DOLLAR_ENTRIES)
# Expected standard output:
#   Mckayla Atlanta 5/29/1986
#   Rhiannon Los Angeles 10/4/1974
#   Elliot New York City 4/3/1947
#   Rigoberto New York City 12/1/1962

# WRITE YOUR SPECS HERE
```

# Deliverable

**One** file `app.rb` hosted in [GitHub Gist](http://gist.github.com) or similar
service, where we can view the solution with a single click.

**Don't worry about sending Gemfile[.lock]**
