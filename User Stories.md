# User Stories

## Feature: Save Recipes

### Scenario: Save recipe found on the internet
>Given the user enters the recipe url into the form.\
When the user saves the recipe\
Then the recipe should be saved in the database w/ html formatting and at least `cuisine` as a keyword filter.

### Scenario: Save recipe personally written
>Given the user enters the information for the recipe.\
When the user saves the recipe.\
Then the recipe should be saved in the database w/ at least `cuisine` as a keyword filter.

## Feature: View Recipes

### Scenario: Retrieve recipe found on the internet
>Given a recipe previously saved from the internet is requested.\
When the user views the recipe.\
Then the recipe should be displayed on the page w/ saved html formatting.

### Scenario: Retrieve recipe personally written
>Given a recipe personaly written is requested.\
When the user views the recipe.\
Then the recipe should be displayed on the page w/ preset html formatting.

## Feature: Edit Recipes
### Scenario: Edit personally written recipe
>Given an existing recipe is requested for editing.\
When the user edits the recipe.\
Then the recipe should be saved among the personally written recipes.

### Scenario: User cannot edit recipe from internet
>Given an existing recips is requested for editing.\
When the user requests to edit a internet saved recipe.\
Then the recipe should deny access to editing.

## Feature: Search Recipes
### Scenario: Retrieve recipes from a cuisine
>Given a user wants recipes from a specific cuisine.\
When the user searches with the cuisine filter for that cuisine.\
Then a list of recipes should populate the page with only recipes from that cuisine.

### Scenario: Retrieve recipes w/ multiple filters
>Given a user wants recipes w/ specific filters.\
When the user adds the filters to the search.\
Then the list of recipes should populate the page with recipes only with those filters.

