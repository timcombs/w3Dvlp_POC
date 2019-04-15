# w3Dvlp-POC

This simple static site is a POC for w3Develops.
w3Develops uses a static site to sign up new study group and build group participants.
This information is collected via a Google Form and pushed to a Google sheet.

## User Story
Once a participant signs up for a group:
- information from the Google sheets should be available on the groups page
- participants will be sorted into categories based on their form selection
- groups page will display participants in the study/build groups
- participants will be displayed by discord username
- categories for sorting:
  - Username - Discord username including the number
  - Commitment - either full time - 6 hrs or part time - 3 hours daily
  - Technology - technology tracks for study currently 
    - html/css
    - vanilla javascript
    - React
  - Beginning - time to start study group midnight, 6 am, noon, 6 pm

## tips to consider
Parsing the JSON is pretty simple as well:
```
for(var key in data.feed.entry) {
  console.log(data.feed.entry[key]['gsx$title']['$t']);
};
```