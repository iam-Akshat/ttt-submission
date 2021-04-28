# ttt-submission

This is the submission for Software Engineer Intern role.

# Frontend in react hosted on netlify
[Frontend Repo](https://github.com/iam-Akshat/ttt-front)
[Frontend Live link](https://awesome-heyrovsky-54802a.netlify.app/)
- ## Libraries used
  - axios for data fetching
  - react-query for data management
  - @testing-library for testing
  - bootstrap for styling
- ## Structure and Explanation
  - App is divided into 2 main components for brevity
  - `<Table />` shows data received from backend
  - `<Input />` Accepts user input and send the request to backend
  - useFetchResults is a custom hook for getting specifically our data, makes testing easier
  - table.test.js tests for correct data rendering
  - input.test.js tests all states of component , Loading, Error and successful
 
 # Backend in Node using Express hosted on heroku
 [Backend repo](https://github.com/iam-Akshat/ttt-back)
 - ## Libraries used
  - axios for data fetching from ttt website
  - cors for cors
  - jest and supertest for testing

- ## Structure and Explanation
  - Express app is in app.js and server is in index.js
  - Since it was a single route app, route is in app , else another file needs to be made for routes
  - /api/rollnums validates user data ,if data is correct,it processes else send 400 error
  - getResults hits the ttt api and returns the data accordingly, uses Promise.all
  - The test is written for 3 cases
    - Bad data
    - ttt backend error
    - Successful result
 
