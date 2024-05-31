# Advanced Learner Data Analysis in JavaScript

This repository contains a JavaScript function, `getLearnerData`, that processes and analyzes learner data from a course. The function uses advanced JavaScript features such as the `Map` object and the `Array.from` method, and includes extensive data validation and error handling.

## Functionality

The `getLearnerData` function takes in three parameters: `CourseInfo`, `AssignmentGroup`, and `LearnerSubmissions`. It validates the input data, processes it, and returns an array of objects. Each object represents a learner and contains their ID, their average score, and their score for each assignment.

## Data

The data used in this project includes `CourseInfo`, `AssignmentGroup`, and `LearnerSubmissions`. The `CourseInfo` and `AssignmentGroup` are objects that contain information about the course and the assignments respectively. The `LearnerSubmissions` is an array of objects, each representing a learner's submission for an assignment.

## Error Handling

The function handles potential errors gracefully using try/catch blocks and other error handling techniques. It skips assignments that are not yet due and applies a late penalty to the score if the submission is late.

## Output

The output of the function is an array of objects. Each object contains the following properties:

- `id`: The ID of the learner.
- `avg`: The learner's total, weighted average score.
- `<assignment_id>`: The learner's score for the assignment as a percentage of the total points possible.

## Usage

To use this function, call `getLearnerData(CourseInfo, AssignmentGroup, LearnerSubmissions)` with your data. The function will return the processed learner data.

## Example

```javascript
const result = getLearnerData(CourseInfo, AssignmentGroup, LearnerSubmissions);
console.log(result);
