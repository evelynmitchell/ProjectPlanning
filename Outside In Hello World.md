# Outside In

Outside in development is similar to waterfall, i  that you start from the highest level description of your project and a test for that description, and progressively refine both tests and code in parallel till you are done.

# Tooling
React
Vue

Testing libraries
Jest
Mocha

End to end testing 
Cypress 
Playwright
testcafe [title](https://testcafe.io/)
https://github.com/DevExpress/testcafe


[title](https://playwright.dev/python/)


[https://new.pythonforengineers.com/blog/web-automation-dont-use-selenium-use-playwright/
]
The killer feature of Playwright is: You can automatically generate tests by opening a web browser and manually running through the steps you want.



# Testing concepts

## Assertions and exceptions 

assert - something that should be the case
```
assert.equal(sum, 7);
```
Checks that the return value of sum is 7

Jest uses expect instead of assert, whic allows you to chain functions together.
```
expect(sum).toEqual(7);
```
Checks that use an expect are called expectations.

Cypress lets us check if an element on the page .contains() a specific string. 
   Questions 
      Is there any scoping for the contains?
      Is it negatable?
      at what point in the page render process is this checked?

## Cypress Docker


[Cypress Docker Github](https://docs.cypress.io/examples/examples/docker)

There are Docker images:

cypress/base:<Node version> has the operating system dependencies required to run Cypress.
cypress/browsers:<tag> extends the base images with pre-installed browsers.
cypress/included:<Cypress version> extends the base images with pre-installed Cypress versions.

https://github.com/bahmutov/cypress-open-from-docker-compose
https://mtlynch.io/painless-web-app-testing/
https://mtlynch.io/notes/cypress-vs-playwright/#what-i-miss-about-cypress

fluent-style API 
https://en.wikipedia.org/wiki/Fluent_interface
When a Cypress test fails, it screenshots your app at the point of failure and saves the image to disk. It’s easy to configure your CI platform to keep these images as test artifacts for easy debugging.

Playwright produces a more complicated set of test artifacts. Instead of simple images and videos, Playwright generates a static web app for viewing all the test artifacts.



## Best Practices

"Stop requiring only one assertion per unit test: Multiple assertions are fine" "One test case, not one test assertion."
[https://stackoverflow.blog/2022/11/03/multiple-assertions-per-test-are-fine/]


# documentation 

[Good Docs Project](https://gitlab.com/tgdp/templates)

