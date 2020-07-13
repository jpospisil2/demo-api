# Interview

Testing is important - but for brevity sake, we're not expecting any automated during the interview. 

Similarly, abstract as much as you'd like or as is necessary, but we won't expect full abstraction for the interview.

## Tasks

1. Build an API endpoint that returns an author. (hardcoded author)

    `GET /api/authors/1`
    
    Example Response:

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
    
## You pick what's next
    
1.  Create a customized error experience

    When saving an author with a name `<script>bad actor</script>`, have the api respond with a custom error response: 
    
    ```json
    {
      "error": "Please don't hack me."
    }
    ```

1.  Create/Modify an endpoint to search for authors by name. 
    
    Given `Charles Dickens` and `William Shakespeare` are in the database as authors  
    
    I want to be able to search with the string `ha` and find both authors: `Charles Dickens` and `William Shakespeare` (because both authors have the string `ha` in their name)
    
1.  Create Tests for our application

    A good application is supported by good tests - please add some test coverage!
