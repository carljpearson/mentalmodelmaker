# mentalmodelmaker
Generates a Mental Model Diagram (based on Indi Young's Mental Models technique)

Requires a CSV that has the following headers:
- "Mental Space" - The mental space (refer to Mental Models)
- "Task tower" - The task tower (refer to Mental Models)
- "Atomic task" - The atomic task (refer to Mental Models)
- "TID" - A unique ID for each task
- "CleanType" - Role with no asterisks or special charators. In this data, it is "QE, PM, RCM etc". Used for color coding. *Note: If you use different types, you'll need to change the CSS to reference the types that you use*

The CSV should be organized by Mental Space first, Task Tower second. (An easy way to do this is to sort your spreadsheet from A-Z on the task tower first, and then A-Z on the Mental spaces)

(If mental space or task tower is undefined, it will be put into a general bucket of empty items.)

## Sample data
Below is a google sheet you can copy that is already configured with correct headers. You can add more columns/headers, but if you delete/edit the existing ones you run the risk of this not working!

Google Sheet:
https://docs.google.com/spreadsheets/d/1E7wbZL9lz05eHDmCkxT9f9ucIg5O-inJxFKK8wkqO-o/edit?usp=sharing

CSV output of that sample data:
https://docs.google.com/spreadsheets/d/e/2PACX-1vQFPTjOD4FoGfQpwBtp5eka2LA-5eVCx6Eo4WKc4NMAqzlBlv1JLCUqOhrKNU9LzHU32cxbtXKFaUOc/pub?output=csv

## About Mental Models
Indi Young wrote a book about this UX research technique. 
In her book she references a Phython script she wrote to generate these models for Omnigraffle. This script generates it into HTML.

Interview with Young: https://indiyoung.com/why-are-mental-models-important/

Buy the book: https://rosenfeldmedia.com/books/mental-models/

Buy the book (amazon): https://www.amazon.com/Mental-Models-Aligning-Strategy-Behavior/dp/1933820063

## Other notes
Requires PHP. Built with v7.2.10 & I haven't tested with any other version.

You'll need somewhere to host this. I use OpenShift Online (https://www.openshift.com/products/online/) but you could use any other platform. 
