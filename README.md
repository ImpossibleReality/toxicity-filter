# toxicity-filter
*note: this is **not meant to be used as a bad-words detection mechanism**. This is meant to be used before testing with a more robust detection method*

<hr />

## usage:

Module will return an array that can be used to search for words

### regex example:
```js
toxicityFilter = require('toxicity-filter')

testToxicity = (txt) => {}

toxicityExpression = new RegExp(`(${toxicityFilter.join('|')})`)

text = 'tell me your password'

if (text.match(toxicityExpression)) {
    testToxicity(text)
}
```



