<br />
<br />
<p align="center">
  <img src="https://cdn.progressionapp.com/cdn-assets/new-progression-logo.svg" alt="Progression" width="180" />
<h3 align="center">Backend Technical Challenge</h3>
<br />
<br />
</p>

Thanks for taking a look at our Backend Technical Challenge! Please read this document before writing any code 🧑‍💻

## 👉 Brief

One of the most important pages in our application is the Framework page—it brings together everything you need to
understand what skills are required at every role in your organisation.

At the moment, this page is built using old-school Rails views and jQuery. We're going to rebuild this page in React so we're going to need some API end points for it.

Here's a lightweight version of the framework page we use in our real production app:

<p align="center">
  <img src="./assets/framework.png" width="600px" alt="Framework preview" />
</p>

We need you to kick this off for us! Take a look at the tasks below, and make sure to read the notes before starting.

#### Notes

- Please treat this as if you were really pairing, so feel free to email us with questions and use google.
- High quality work is important to us, treat this as if it was going to Production.
- Don't worry about finishing! We'd prefer to see how you work than get everything done. **Please don't spend an excessive amount of time on this task—anywhere between 2 and 3 hours is plenty**
— Feel free to make a note of anything you would do if you had more time.
- If some instructions are a little vague, take it as an invitation to use your imagination and best judgement.
- We're leaving technology choices up to you! Feel free to use libraries or frameworks that you think can help you get the work done quickly and to a high quality.


#### Implementation details

- No need to worry about authentication for this exercise.
- The source data is provided as JSON files, however in the future the data might come from XML files or a database. Make sure the data retrieval layer is decoupled from the data presentation layer, so if the data source were to change the data presentation layer wouldn't need to change.
- The API design should be RESTful and consistent, feel free to suggest a pattern or standard we should follow, you could add any thoughts or notes to a readme.


#### 1️⃣ &nbsp;Task 1: Skills and Positions
Create separate endpoints that return:

- A single skill, when provided a given skill_id
- A single position, when provided a given position_id

#### 2️⃣ &nbsp;Task 2
Create an endpoint that returns a row positions for a given discipline ID.

#### 3️⃣ &nbsp;Task 3
Create an endpoint which, for a given framework ID, returns the data required to render the framework view in a single request. This should consist of skills, positions, requirements, disciplines and categories.

#### 3️⃣ &nbsp;Task 4
We just made the frontpage of Product Hunt, Reddit and Hacker News on the same day and our traffic is up 1000x! Help us to improve the performance of the end points! 

For the purpose of this exercise you can assume the updated_at value for a parent is set when a child is updated, all the way up the chain. For example, when a requirement is updated, the updated_at of the parent skill, position is updated which in turns updates the category and discipline, which updates the framework.