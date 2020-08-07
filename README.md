# ProxyCrawl Test

Welcome to ProxyCrawl test, if you haven't applied for a job offer yet, please do so before starting the test by emailing us at `jobs at proxycrawl dot com`

## Instructions

1. Clone/fork this repository.
2. Read [Project to Build](#project-to-build) section to see what you have to build in the test.
3. Make commits to the repository like you would normally do on your daily job.
4. Once you are done, if you've forked this project, you can send us the link to the Github project. If you haven't, you can send us the zip file of the project (make sure it includes the `.git` folder).

## Project to build

Create an application using NodeJS or Ruby (depending on the job offer you've applied) that scrapes Amazon SERP pages and saves product details in a database using [ProxyCrawl Crawling API](https://proxycrawl.com/docs/crawling-api).

*Please create a free account if you haven't done so yet, the first 1000 requests are free of charge, if you need more free requests please ask the person in charge of your role application.*

The application must process a list of Amazon SERP URLs and crawl them using the ProxyCrawl API. The data has to be stored in a SQL database (MySQL, SQLite, etc.) and you should save as much information as you want to make the database rich for each Amazon product if it exists in the DB, do not store it again. The information must be crawled using the [ProxyCrawl Crawling API](https://proxycrawl.com/dashboard/docs).

### Important notes to follow

1. The crawling of the Amazon SERP pages has to be done in **background jobs** (ex. to push the URLs to a queue and crawl them as background jobs).
1. The crawling project should run every week on Monday at 10:00 AM through a predefined scheduler (ex. Same URLs have to be crawled every week and the product info has to be updated accordingly)
1. The parsing of the raw HTML pages has to be done internally in the project and not to rely on ProxyCrawl API built in scrapers.
1. Implement **CRUD operations** through a **REST API** which is accessed externally with basic authentication, that should do -- it creates, reads, updates, and deletes (CRUD) data from a database in response to a given HTTP request, and provides a suitable JSON response.

## Important notes

- This project is to showcase your skills, so try to do it as best as you can.
- You don't have restrictions on libraries or frameworks to use for the test, that is up to you. But don't forget that we want to see your skills, not the ones of the guys from the libraries, so do it wisely ;)
- We should be able to run the test and try it. If there are setup instructions please include them in this README file.
- There are no restrictions, limits, or instructions on the frontend part. We want to see your creativity!
- The test is not time metered but we don't want you to use more than 5 hours on it.
- If you have any questions, don't hesitate to contact the person in charge of your application.
