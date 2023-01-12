# UFOs

## Overview

In this project we will use JavaScript, HTML, and CSS to build a webpage that displays a table organizing UFO sightings data. 

### Purpose

Having a dynamic website allows the data to be visually appealing and easy to access for everyone. Sifting through data manually in a table or array can be tedious but having a interactive website allows data access and understanding to be attainable to everyone. Using the tools mentioned above, a dynamic webpage will be built in which the data concerning UFO sightings can be stored, displayed visually, and be interative (able to filter based on search criteria). 

## Results

UFO Sightings:

![Webpage](https://user-images.githubusercontent.com/112137694/211950673-008de93e-c83f-4a54-8034-a650bc38796e.png)

Filters and the table:

![Table](https://user-images.githubusercontent.com/112137694/211950850-4dbd9531-fde9-4f9b-90df-798baf6de3c1.png)

Using the filter search, you can filter by any combinations of the search criteria. For example: you can search only by date or by every category. The search criteria corresponds with the columns of the table. All but the last two columns, 'Duration' and 'Comments,' are available to filter.

![Filters](https://user-images.githubusercontent.com/112137694/211950969-416be795-00f8-4125-a896-b3b6aceba03f.png)

Example of a filtered search:

![Example](https://user-images.githubusercontent.com/112137694/211951092-d545ba7d-8f38-42d4-a571-e374b15ae6cd.png)

## Analysis

There are a few challenges and drawbacks to the designed webpage:

- Case-sensitive search field: The table will not filter properly if the cases are not matched in the search box and in the table itself. There is also no instruction on how to enter the information into the search field. If the user mistakenly uses upper case when it should be lower case, they may not know why they aren't getting data returned or believe there to be no data at all for that search.
- No partial entries: the search criteria must be filled out in it's entirety or there will be no return of data in the table. This potentially causes the same issue stated above.
- There is no live data source connected to this data. The table will not update as more sightings are reported.
- The filters require a previous understanding of the data in the table. The user must know the specific date, city, or shape to search. Some shapes might not be intuitive.
- Whitespaces: this ties with the first two drawbacks listed. The data MUST be entered exactly how the table has the data stored. If there is an extra space that was not intended by user error, there will be no output

Recommendations:

1. Add a trim function to clear out white spaces
2. Create a function to standardize the entries as all upper case or lower case so despite how the user enters the data, it will be transformed to match the data in the table
3. Create a date range filter. Being able to see all the data from one month could be beneficial in tracking activity between different months
Add a live data source so the table can continuously update as new sightings are reported
