<div class="mdown-container">

<div>

# Challenge: Historical Events Finder

## Basic Requirements

Build a single-page app that enables users to search and browse historical event information based on data found in the JSON file included with this repo. Use:

*   ReactJS for all views and bundle with Webpack
*   [json-server ](https://github.com/typicode/json-server)as your simple web+api server
*   [react-paginate ](https://www.npmjs.com/package/react-paginate)to manage data fetch from the server

You'll be working with a "messy" dataset. In this dataset, the dates are sometimes represented as year-only and sometimes as YYYY/MM/DD. Additionally, some dates fall into the BC range, and those dates have a negative sign in front. Lastly, citations are improperly formatted and are unusable in their current form. Yuck!

For basic requirements, you are going to ignore this messiness at the server layer by using `json-server` to create a simple web+api server from your JSON data source. Configure `json-server` to serve up static assets from your `public` folder. Target webpack to build into the `public` folder, then create an `index.html` file which loads that bundle, and you now have a simple full-stack react app.

Build a React UI that allows the user to search for historical events based on a keyword. Use the full-text search features of `json-server` to return a result to the UI for browsing. Paginate the list of events using `react-paginate`, loading no more than ten at a time. Ensure you are implementing [server-side pagination ](https://github.com/typicode/json-server#paginate)NOT client-side pagination.

**Reminder:** emphasis should be placed on creating well-defined interfaces, writing code with a clear separation of concerns, and using the principles of modularity, encapsulation, abstraction.

<div id="challenge-f5e0cb23-b3c4-4556-8541-545ebf327c04">

<form class="challenge-block" data-challenge-type="project" data-is-gradeable="true" id="challenge_70464"><input name="challenge_id" type="hidden" value="70464">

<div class="challenge-header">

<div class="icon-container">1</div>

<div class="textcontainer">

<div class="title">Historical Events Finder</div>

</div>

</div>

<div class="problem ">

Submit the URL to your completed project below.

</div>

<div class="answer"><input autocomplete="off" name="answer" placeholder="http://github.com/<github-username>/<repo-name>" type="text" value=""></div>

<div class="actions">

<div class="buttons"><button class="lp-style-button resetbutton">Reset Input</button>

<div style="display: inline-block;"><button class="lp-style-button undefined " id="challenge-button-70464" type="submit">SUBMIT</button></div>

</div>

</div>

</form>

</div>

## Advanced Content

*   That data is messy! Add an `edit` button on the UI to allow the historical event information to be edited. Allow those edits to be saved back to the server using a `save` button.
*   Add the feature of "Favoriting" a historical event: when the user favorites an event, they are prompted for a "Favorite Set". The user may select an already existing "Favorite Set" or may wish to create a new "Favorite Set." What's a Favorite Set? Instead of having only one set of favorites, some sites (like Airbnb) allow users to create _many sets of favorites,_ where each set has a unique name. For example, a user might favorite some events into "War Story" favorites and others into "Science Story" favorites.
*   Use `react-router` to navigate throughout the app. Allow the user to navigate to a page where they can see all of their Favorite Sets and another page to see all the events of a selected Favorite Set. Don't forget to let the user navigate back to the search page.

## Nightmare Mode

*   Replace `json-server` with your own server, created using Express+MongoDB

</div>

</div>