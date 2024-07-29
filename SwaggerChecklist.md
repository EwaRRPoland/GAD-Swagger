|E                                                                                                                                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------|
|Page Header Checklist                                                                                                                            |
|Date of test run                                                                                                                                 |
|Tester                                                                                                                                           |
|OS                                                                                                                                               |
|Browser                                                                                                                                          |
|Positive tests                                                                                                                                   |
|users, POST create user: User registration                                                                                                       |
|authentication POST: User authenication                                                                                                          |
|authentication POST: Log out / refresh token                                                                                                     |
|authentication POST: Refresh tokens                                                                                                              |
|users,GET users: Get all users                                                                                                                   |
|users, GET users: Find user by ID (existing user)                                                                                                |
|articles, GET aricles: Get list of articles                                                                                                      |
|articles, GET aricles {id}: Find article by ID                                                                                                   |
|articles, POST articles:  Add an article with authorization,  418 characters - text in the body, with image                                      |
|articles, POST articles:  Add an article with authorization,  418 characters - text in the body, with image                                      |
|articles, PUT articles {id}:  Updates an article with authorization,  418 characters - text in the body, with image                              |
|articles, PATCH articles {id}:  Update an article with authorization,  418 characters - text in the body, with image                             |
|articles, DELETE articles {id}:  Deletes an article with authorization,  418 characters - text in the body, with image                           |
|articles, HEAD articles {id}:  Info about article with authorization,  article with id - exist                                                   |
|Negative tests                                                                                                                                   |
|users, POST create user: User registration using already existing e-mail                                                                         |
|users, POST create user: User registration with an e-mail without an @                                                                           |
|users, POST create user: User registration with an e-mail without a dot                                                                          |
|users, POST create user: User registration with no symbol in front of the @                                                                      |
|users, POST create user: User registration with a dash at the beginning of the email                                                             |
|users, POST create user: User registration with a dash at the end of the email                                                                   |
|users, POST create user: User registration with a special symbol in name part of the email                                                       |
|users, POST create user: User registration with an email over 64 characters long                                                                 |
|users, POST create user: User registration with an email under 10 characters                                                                     |
|users, POST create user: User registration with a registration with incorrect avatar link                                                        |
|authentication POST: User authentication with the wrong password/empty string                                                                    |
|authentication POST: User authenication with an inextisting e-mail                                                                               |
|authentication POST: User authentication with an invalid request body                                                                            |
|users, GET users: Find user by ID (int, non-existing user)                                                                                       |
|users, GET users: Find user by ID (string)                                                                                                       |
|users, GET users: Find user by ID (special symbols)                                                                                              |
|articles, GET aricles {id}: Find article by incorrect ID (-1)                                                                                    |
|articles, GET aricles {id}: Find article by incorrect ID (0)                                                                                     |
|articles, GET aricles {id}: Find article by incorrect ID (99)                                                                                    |
|articles, GET aricles {id}: Find article by incorrect ID (999)                                                                                   |
|articles, GET aricles {id}: Find article by incorrect ID ("a"%)                                                                                  |
|articles,GET aricles {id}: Find article by incorrect ID (b)                                                                                      |
|articles, POST articles:  Add an article with no authorization                                                                                   |
|articles, POST articles:  Add an article with authorization, 813 characters - text in the body                                                   |
|articles, POST articles:  Add an article with authorization,  418 characters - text in the body, without title                                   |
|articles, POST articles:  Add an article with authorization,   without body                                                                      |
|articles, PUT articles {id}:  Updates not your article with authorization,  418 characters - text in the body, with image                        |
|articles, PUT articles {id}:  Updates an article id of article does not exist, with authorization,  418 characters - text in the body, with image|
|articles, PUT articles {id}:  Updates an article You are not an owner, with authorization,  418 characters - text in the body, with image        |
|articles, PUT articles {id}:  Updates an article user_id is missing, with authorization,  418 characters - text in the body, with image          |
|articles, PUT articles {id}:  Updates an article, title is missing, with authorization,  418 characters - text in the body, with image           |
|articles, PUT articles {id}:  Updates an article, body is missing, with authorization, with image                                                |
|articles, PUT articles {id}:  Updates an article, expired access token                                                                           |
|articles, PUT articles {id}:  Updates an article, invalid access token                                                                           |
|articles, PUT articles {id}:  Updates an article, expired access token                                                                           |
|articles, HEAD articles {id}:  Info about article with authorization, article with id does not exist                                             |
|articles, HEAD articles {id}:  Info about article with authorization, article with id incorrect                                                  |
