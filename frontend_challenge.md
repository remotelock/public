# Frontend Technical Evaluation

Code quality is very important to us. We're sending you this challenge so that
we can evaluate your coding skills with JavaScript.

### Instructions

- Use the test framework you're most familiar with
- Don't use any library to accomplish the solution (except test framework)
- Use anything you need from ES6+ standard library

### What we expect from your code

- Clean code
- Extensibility
- Maintainability
- Testability

# The challenge

Write a code to parse data represented in different formats and print to standard
output in a single format:

  `<First name> <City> <Birth date>` (line order is not important, but date format is)

### Template code

```javascript
// File: app.js

const COMMA_ENTRIES = [ // First name, City, Birth date
  'Mckayla, Atlanta, 5/29/1986',
  'Elliot, New York City, 4/3/1947',
]
const DOLLAR_ENTRIES = [ // City, Birth date, Last name, First name
  'LA $ 10-4-1974 $ Nolan $ Rhiannon',
  'NYC $ 12-1-1962 $ Bruen $ Rigoberto',
]

// WRITE YOUR FUNCTIONS / CLASSES HERE

class App {
  static run({ comma = [], dollar = [] }) {
    // INVOKE YOUR MAGICAL CODE HERE
  }
}

App.run({ comma: COMMA_ENTRIES, dollar: DOLLAR_ENTRIES })

// Expected standard output:
//   Mckayla Atlanta 5/29/1986
//   Rhiannon Los Angeles 10/4/1974
//   Elliot New York City 4/3/1947
//   Rigoberto New York City 12/1/1962

// WRITE YOUR SPECS HERE
```

# Deliverable

**One** file `app.js` hosted in [GitHub Gist](http://gist.github.com) or similar
service, where we can view the solution with a single click.

**Don't worry about sending package.json**
