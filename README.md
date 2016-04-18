# Fred's List Optmization

## Description
It is time to make Fred's List a little more optimized and proactive with automated testing caching and deployment

## Normal Mode

### Travis CI and Testing
* You must test have at least 1 test per html view and 1 test per api/verb combo (so both list and create)
* You must pass all tests
* Setup Travis-CI on your own fork.  It should test anything pushed to the master branch
* Your master branch README should include the travis icon indicating the branch is passing

### Caching
* Cache the main category view for 5 minutes
* Cache the cities in the template itself
* Cache the sessions with the write through [cached_db](https://docs.djangoproject.com/en/1.8/topics/http/sessions/#using-cached-sessions) 

### Optimizations
* Use select related on listing page querysets to reduce the number of queries

### Hard Mode
* Deploy your code from travis and stop deploying from local
* Use coverage and coveralls and have 75% code coverage

