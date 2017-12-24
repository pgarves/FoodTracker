# FoodTracker

CMSC389L Final Project

## Overview

Food Tracker is a web application that will allow users to track their food that has been eaten throughout the day.

It will record the food’s nutritional attributes such as protein, carbohydrates, fiber, calcium, and iron.

It will then suggest other foods for the remainder of the day that allow for the user to get the remaining amount of nutrients for a well balanced diet.

## Services Used

- Hosted on s3 [here](http://cching-food-tracker.s3-website.us-east-2.amazonaws.com/)
- DynamoDB
- Cloudtrail
- API for USDA Food Composition Databases

## YouTube Video Demo

[Video Demo Link](https://youtu.be/qSbygZA7BdM)

## Architecture

![Click here to view the architecture diagram](https://lh3.googleusercontent.com/PsM0ezC8j65xaRskQcU1UA99qHTiIZXGKk_Uie6r199cMEFscogwbkIq5YgZwdd6febwOB45r2aRzlJJYsjRHlzRYllddWPT7bl-RepSp1FGUoJnEVtWMCbExz3TcWQ6PVrxkgyoKBg)

## API Overview

[Click here to learn more](https://ndb.nal.usda.gov/ndb/doc/apilist/API-FOOD-REPORTV2.md)
United States Department of Agriculture Food Composition Databases

Used "ndbno" as the food index number then parsed through from report -> food -> nutrients to get this food's nutritional arrtibutes: protein, carbohydrates, fiber, calcium, and iron.

## How to Run It

- Visit the link [here](http://cching-food-tracker.s3-website.us-east-2.amazonaws.com/)

- Or if you wish to edit the code yourself, clone the repo and change the accessKeyId and secretAccessKey in the javascript. Also create your own Cloudtrail on the AWS console.
