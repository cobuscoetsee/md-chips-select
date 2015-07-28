Learn from [Angular Material](https://material.angularjs.org/latest/#/), and add a multi-select menu to md-chips.

[Demo](http://codepen.io/boo0330/pen/EjOWgg)


Prerequisites: angularjs
Include the md-chips-select.js and md-chips-select.css

In your HTML file:

<md-chips-select ng-model="myItems" select-items="sItems" main-title="name"></md-chips-select>

ng-model (required):  The array to store the selected items
select-items (required): The array of the items in the select list
main-title (optional): The attributes seperated by space. It will combine all value of the attributes as the title of the list item.  If the main-title is not given, there must be one attibute named "title" in the select-items array
  Ex: main-title = "name id"
  
  It will combine the value of the attribute "name" and "id" (See the example below)

In your javascript:

Add an array for ngModel (selected)
Ex: $scope.myItems = []

Add an array for select-items
Ex: $scope.sItems = [{
      name: "Mini Cooper",
      id: 0
    }, {
      name: "Lexus IS250",
      id: 1
    }, {
      name: "Ford F150",
      id: 2
    }, {
      name: "Toyota Prius",
      id: 3
    }];
