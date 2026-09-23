| TC-01 (Create User) | POST | http://localhost:8081/api/users | {"name": "Karan Partap Singh", "email": "karanpratap1277@gmail.com"} | Response returns ID with created data. | 201 Created | **PASS** |
| TC-02 (Get All Users) | GET | http://localhost:8081/api/users | None | Returns JSON list containing user ID 1. | 200 OK | **PASS** |
| TC-03 (Get User By ID) | GET | http://localhost:8081/api/users/1 | None | Returns data for user with ID 1. | 200 OK | **PASS** |
| TC-04 (Update User) | PUT | http://localhost:8081/api/users/1 | {"name": "Karan Singh", "email": "karan.singh@example.com"} | Updated name and email reflected. | 200 OK | **PASS** |
| TC-05 (Delete User) | DELETE | http://localhost:8081/api/users/1 | None | Empty body. | 204 No Content | **PASS** |
| TC-06 (Get Deleted User) | GET | http://localhost:8081/api/users/1 | None | User no longer exists. | 404 Not Found | **PASS** |
| TC-07 (Negative Test) | GET | http://localhost:8081/api/users/99 | None | Non-existent ID. | 404 Not Found | **PASS** |