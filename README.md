# Postman API Automation Integration with GitHub Actions #

This repository is a demonstration for POC for intigrating postman test with GitHub Actions. The tests are written in postman and they are executed in a VM with the help of Newman and Newman-reporter-htmlextra.
GitHub Actions will trigger the project execution on every push to the main branch. You can also execute the project manually, workflow_dispatch, or to run the project on a scheduled time with the help of a cron job.

The HTMl report is archived and kept in the artifact section for the team to download it. Along with that, they can view the report directly from github page: https://sundar10121992.github.io/Phoenix-Inwarranty-Flow/ .
The latest report is mailed to the team members using GMAIL SMTP.

## About ME ##
Hi My name is Sundar Kande . I have 3.5 Year Experince in Automation testing My skill set includes UI Automation with selenium WebDriver , And for API testing I used RestAssured and Postman 
Connect with me over : (https://www.linkedin.com/in/sundar-kande-872060243/)

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge case Testing
3. Token Testing
4. Data driven testing
5. Schema Validation
6. Secrete Management with Github secrete

## HTML Report ##
The Report will be created in Newman Folder

![Postman Report](https://raw.githubusercontent.com/SUNDAR10121992/Phoenix-Inwarranty-Flow/static-content/Newman_Report_Sample.png)   

## Project Structure ##


```
Phoenix Inwarranty flow
├─ In-WarrantyFlow Collection_Ext_CSV.postman_collection.json  # Collection File 
├─ QA.postman_environment.json # Environment File
└─ testData.csv # TestData File

```

## Tech stack ##
1. Postman
2. Newman
3. Node.js 22v
4. Newman-reporter-htmlextra
5. Github Actions
6. Gamil SMTP
7. Github pages
8. CSV for Data driven testing
9. AWS-EC2 instance for self hosted github runner

## GitHub Pages ##
You can directly view latest test report Postman test at the github Page link : https://sundar10121992.github.io/Phoenix-Inwarranty-Flow/ .

## How to Run the Project ##
You can run project on you local system for that :
1. Clone project on Local system : ```https://github.com/SUNDAR10121992/Phoenix-Inwarranty-Flow.git```
2. Install Node.js and NPM from : ```https://nodejs.org/en/download```
3. Install Newman : ``` npm install -g newman ```
4. Instal Newman-reporter-htmlextra : ``` npm install -g newman-reporter-htmlextra ```
5. Run the newman command :

 ```
              newman run 'In-WarrantyFlow Collection_Ext_CSV.postman_collection.json' \
             -e QA.postman_environment.json \
             -d testData.csv \
             -r cli,htmlextra \
             --reporter-htmlextra-export ./newman/index.html
```




     
   
   
