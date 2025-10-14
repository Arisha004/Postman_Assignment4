# Postman API Testing Assignment  
**By:** Arisha Mumtaz (2312358)  
**Course:** QA Internship Project  
**Submission Date:** 17th October 2025  

---

##  Project Overview  
This project was created as part of my QA internship assignment to perform **API testing using Postman**.  
It includes practical work with multiple HTTP methods, variable handling, scripting, assertions, and API chaining.

---

##  Learning Objectives  
Through this project, I learned how to:  
- Create and manage **Postman collections**  
- Use and handle **environment variables**  
- Write **Pre-request** and **Tests** scripts  
- Generate and use **dynamic random data**  
- Parse **JSON responses** and log data  
- Apply **Chai assertions** for validation  
- Chain APIs using response variables for dynamic testing  

---

## Tasks Completed  

| No | Task Description | Status |
|----|------------------|--------|
| 1 | Used all API methods (GET, POST, PUT, PATCH, DELETE) | ✅ |
| 2 | Set Base URL as environment variable | ✅ |
| 3 | Generated random request body data | ✅ |
| 4 | Parsed JSON response and logged values | ✅ |
| 5 | Wrote Chai assertions (including one failing test) | ✅ |
| 6 | Used Pre-request and Tests sections for variable handling | ✅ |
| 7 | Chained APIs using response variables | ✅ |

---

##  Tools & Technologies Used  
- **Postman** for API testing  
- **JSONPlaceholder API** as the testing endpoint  
- **JavaScript (Chai Assertion Library)** for scripting  
- **GitHub** for submission and version control  

---

##  Base URL  
{{baseUrl}} = https://jsonplaceholder.typicode.com


---

##  Collection Details  

**Collection Name:** Bookstore_Assignment4_Arisha_Mumtaz.postman_collectionfinal
**Environment File:** Bookstore_Assignment4_Env.postman_environmentfinal

### Included Requests:
1. **GET Request** – Fetch data from `/posts`  
2. **POST Request** – Create a new post using random title & body  
3. **PUT Request** – Replace post data using chained `postId`  
4. **PATCH Request** – Partially update a post  
5. **DELETE Request** – Delete a post and clear environment variables  
6. **Negative Test** – Test invalid endpoint and assert failure intentionally  

---

##  Example Assertion Used
```javascript
pm.test("Response has id and title", function () {
    pm.expect(jsonData).to.have.property('id');
    pm.expect(jsonData).to.have.property('title');
    pm.expect(jsonData.title).to.eql(pm.environment.get('randomTitle'));
});

---

## Assignment Description

1. All methods (GET, POST, PUT, PATCH, DELETE) are successfully tested.

2. Random data generated dynamically for each new request.

3. Response values (like postId) are chained across requests.

4. Assertions confirm correct API behavior.

5. One intentionally failing test case is included for validation.

## Files in Repository
📁 Postman_Assignment4_Arisha_Mumtaz
│
├── Bookstore_Assignment4_Arisha_Mumtaz.postman_collection1
├── Bookstore_Assignment4_Env.postman_environmentfinal
└── README.md

## Submission Links

GitHub Repository:
https://github.com/arishamumtaz/Postman_Assignment4


## Conclusion

This assignment helped me understand the complete API testing flow — from creating requests, using variables, scripting validations, to chaining responses.
It also improved my practical understanding of Postman and QA automation concepts.

Completed by:
Arisha Mumtaz
QA Intern | 10 Pearls
