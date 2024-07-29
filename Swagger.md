#

##

# Page Header Checklist

- **Date of test run:** 02.06.2024
- **Tester:** Ewa Rostecka-Rzońca
- **OS:** Windows 10
- **Browser:** Microsoft Edge 125.0.2535.79 64-bit

## Positive tests

| Test Description | Expected Result (code - expected) | Result (code - current) | Results | Comments |

| users, POST create user: User registration | 201 | 201 | PASS | User created |

| authentication POST: User authentication | 200 | 200 | PASS | Generated token |

| authentication POST: Log out / refresh token | 200 | 200 | PASS | Successful operation |

| authentication POST: Refresh tokens | 200 | 200 | PASS | Successful operation |

| users, GET users: Get all users | 200 | 200 | PASS | Successful operation (no parameters) |

| users, GET users: Find user by ID (existing user) | 200 | 200 | PASS | Successful operation |

| articles, GET articles: Get list of articles | 200 | 200 | PASS | Successful operation (no parameters) |

| articles, GET articles {id}: Find article by ID | 200 | 200 | PASS | Successful operation |

| articles, POST articles: Add an article with
| authorization, 418 characters - text in the body,
| with image | 201 | 201 | PASS | Article created (no information in the documentation about| the | maximum number of characters in the article body) z|
| articles, PUT articles {id}: Updates an article with authorization, 418 characters - text in the body, with image | 200 | 200 | PASS | Article updated |
| articles, PATCH articles {id}: Update an article with authorization, 418 characters - text in the body, with image | - | - | PASS | - |
| articles, DELETE articles {id}: Deletes an article with authorization, 418 characters - text in the body, with image | - | - | PASS | - |
| articles, HEAD articles {id}: Info about article with authorization, article with id - exist | 200 | 200 | PASS | Article exists |
