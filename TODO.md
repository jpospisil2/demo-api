# Interview

Testing is important - but for brevity sake, we're not expecting any automated during the interview.

Similarly, abstract as much as you'd like or as is necessary, but we won't expect full abstraction for the interview.



1. Build an API endpoint that returns an author. (hardcoded author)

    `GET /api/authors/1`
    
    Expected Response:

    ```json
    {
      "id": 1, 
      "firstName": "Mark",
      "lastName": "Twain"
    }
    ```

1. Build a new endpoint that saves an author to the H2 Database. (H2 is on the pom)

    The endpoint should accept firstName and lastName. The saved author should be returned with its id. 

1. Wire up your endpoint from step 1 to return live data

1. Create a new endpoint to return all authors in the db

    `GET /api/authors`
    
1.  TODO: Create a customized error experience

1.  TODO: Create/Modify an endpoint to search for authors by name. 
