# VMR Technical Challenge
Welcome to the Versent Modern Run technical challenge! 
We want to get a feel for how you approach the type of problems you might face day-to-day in VMR. 
Please complete the task outlined below to the best of your ability and submit by the deadline given in the invitation. 
When planning your approach please keep in mind that you should only spend 4 to 8 hours in total.

## Problem Statement
Consider the principle of *Contact Tracing*: Individuals check in on various dates at various locations to facilitate rapid notification in the event of an outbreak. Naturally contact tracing information is collated in two ways:
1. A location provides a list of persons and what date they attended
2. A person provides a list of locations and what date they attended

The attached file [`data.json`](./data.json) contains contact tracing data of the first kind. Your mission is to: 

```
DESIGN and DEPLOY a web API that allows users to:
- Find every PERSON that has visited a particular LOCATION on a particular date
- Find every LOCATION that a particular PERSON has visited on a particular date
- [BONUS] given a specific PERSON and date, identify their CLOSE CONTACTS on that date

Write DOCUMENTATION explaining how to use your API, and the reasoning behind your architectual decisions in a `README`

Package your SOURCE CODE into a single `git` repo for submission
```

You may make the following assumptions:
- Names of people and locations are globally unique
- Attendance on the same date constitutes close contact
- Data is sorted alphanumerically

## Submission
Your submission should consist of:
1. The public URL endpoint of your API
2. Your source code; either as a link to a private GitHub repository; or as a .zip via email to your interviewer's email address.

We kindly ask that you keep the details of this technical challenge private.

## Marking Criteria
Your submission will be judged on:
- How well it addresses the problem statement
- Quality of code and comments
- Documentation and rationale behind the design

There is no single correct answer to this challenge.
*Even a partial solution is better than nothing.*
You are encouraged to use whatever tools, platforms, languages, and frameworks you are comfortable with.
If in doubt, keep it simple, and use 'boring' [[1]](http://boringtechnology.club/) technology. 

DevOps means a lot of different things to different people and we try to take all of this into consideration. A submission from a sysadmin would likely look different to one from a software engineer. Likewise we would expect more from a mid-level engineer than a junior. At Versent we value diversity of perspectives and look forward to receiving your submission and feedback.

## Hints
We primarily use AWS with a bit of Azure. Stick to these platforms unless you're confident you can explain your rationale for picking something else.

Beware when working with dates and timezones! All dates are given as ISO Strings at midnight UTC.

`Normal people... believe that if it ain't broke, don't fix it. Engineers believe that if it ain't broke, it doesn't have enough features yet. - Scott Adams`

[1] http://boringtechnology.club/
