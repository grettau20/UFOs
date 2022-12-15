# Introduction

The purpose of this project was to first add additional filters to the UFO Sightings webpage created in the JavaScript module practice,these were city, state, country and shape. Second, was to add a listenning event to listen to various input change to the filters.

The original function was set to identify a date format equal to a specific date input in the box. Then a button was set up to filter the data and only fill the table with data corresponding to the specific date filter. In order to make the changes requested, we modified the javascript file(app_1.js) and the index.html file respectively.

# Analysis

We start with the javascript file, we first changed the handleclick() function into an updatefilters() function, then set up 3 variables:

1. A "changedElement" to capture the each of the input element we are filtering for.
2. An "ElementValue" to capture values corresponding to the changedelement.
3. A "filter id" to link with each of the element to be filtred.

We changed the if statement so that if a filter value is entered; then that filterId and value are added to the filters list. Otherwise, that filter is cleared from the filters object.

Next we set up a filterTable() function to be filled the table with newly filtered data, a foreach loop looped through the data so as to retain only values corresponding to the each of the keys which were the changedElements we are filtering for, a new table with filtered data is built, then finally we modified the listening event function to listen input change which is under the list-group-item in the index.html file.

The second set of changes are performed in the index.html file, and simply consist of adding additional list tags that match the four filters to be added. The class remain the same but the label, input id and input placeholder were changed. We also removed the filter button that was previously present.

# Summary

After modifying both files, we relaunched the webpage and tested the filters. All seemed to be working as they should.
