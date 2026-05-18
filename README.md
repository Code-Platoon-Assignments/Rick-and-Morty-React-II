# Rick and Morty React II

By the end of this assignment your project should meet the following requirements:
  
  - AboutPage.jsx should render general about me information about the show. (Maybe use an API to render this information?)
  - CharactersPage.jsx should render a Card BootStrap Component (displaying image and information of said character) for every character within the [Rick and Morty API](https://rickandmortyapi.com/)
    - Maybe use useState, useEffect, axios, async, map, conditional rendering?
  - Routes for each page mentioned above within Reacts Browser Router
  - NotFound.jsx should render an error message letting the user know this page does not exist
  - Error Route to render NotFound.jsx
  - NavBar.jsx should allow users to navigate your project
  - Testing with Cypress to ensure all requirements are being met
  - Styling from React BootStrap or Tailwind.css
  - Have fun!
  
> [!WARNING]
> The Rick and Morty API uses **pagination**.
>
> Pagination means the API does **not** return every matching item in one giant response. Instead, it breaks the data into smaller “pages” of results.
>
> For example, if there are hundreds of characters, the first API request may only return the first page. To get more results, you need to request the next page.
>
> Most list responses from the Rick and Morty API include an `info` object:
>
> ```json
> {
>   "info": {
>     "count": 826,
>     "pages": 42,
>     "next": "https://rickandmortyapi.com/api/character?page=2",
>     "prev": null
>   },
>   "results": []
> }
> ```
>
> The `info` object contains:
>
> - `count`: the total number of matching items across **all pages**
> - `pages`: the total number of pages available
> - `next`: the URL for the next page of results, or `null` if there is no next page
> - `prev`: the URL for the previous page of results, or `null` if there is no previous page
>
> The actual data you want is usually inside the `results` array.
>
> For this assignment, do not assume that one API request gives you every result. Check the `info` object and use `next`, `prev`, or the `page` query parameter when you need additional pages.