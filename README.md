# recipes_server
simple JSON routes server API


## 1- GET route that returns all recipe names.
route: /recipes

### Error response


## 2- GET route that takes a recipe name as a string param
route: /recipes/details

### Error response
If recipe does NOT exist: 
Response body (JSON): {}
Status: 200


## 3- POST route that can add additional recipes in the existing format
route: /recipes

### Error response
If the recipe already exists:

```json
**Response body (JSON):**
{
	"error": "Recipe already exists"
}
**Status: 400**
```


## 4- PUT route that can update existing recipes.
route: /recipes

### Error response
If the recipe doesn't exist:

```json
**Response body (JSON):**
{
	"error": "Recipe does not exist"
}
**Status: 404**
```
