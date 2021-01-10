# Basic JS Unit Testing Suite 

Unit Testing is mostly about assert operations. JavaScript does not have a native assert operation, therefore one has been written here. It is the `testUnits()` method of the `unitTesting ` object.

There are two basic elements in play.

## testGroups
This is a JSON array that holds test group data, including the functions to be tested and the cases for each: input, expected output, messages.

## unitTesting
This consists of two main methods:

### prepareDOM()
This method parses the `testGroups` array and formats the DOM to prepare for unit testing output.

### testUnits()
This method parses the `testGroups` array and runs each test with the input stated. Depending on the outcome of the test, the output is styled with the appropriate CSS class. A count for each test group (of failed and successful tests) is also generated and inserted into the DOM.
