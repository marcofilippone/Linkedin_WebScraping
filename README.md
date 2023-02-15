# Linkedin_WebScraping

To put the knowledge, we have gained during session 4 in practice, this assignment is dedicated to scrapping one of the most used networking platforms in the business world, LinkedIn. In particular, you are going to retrieve information about all available Data scientist jobs currently available in the Barcelona area. You can find the full list of results in the following link.

## Objective:

Generate a DataFrame that contains the following information for all the listed job posts:

1. Job Title
2. Company Name
3. Location
4. State
5. Posting Date
6. Offer URL
7. Number of Applicants (in int form)
8. Promoted (in boolean form)
9. Workspace
10. Seniority
11. Employment Type
12. Industry
13. Python Required (in boolean form)
14. Application through Linkedin (in boolean form)
15. Number of Employees (in int form)

## According to the following criteria:

1. In cases when values for any of the attributes above are not specified, the corresponding entries should be filled with pandas NaN values.  
2. The Job Titlte, Company Name and Location attributes should correspond to the basic offer information as displaye din both the short listing and the extended offer webpage.
3. The State attribute should be “Early Applications” if there is an alert that shows Early Applicant, "On-going" if there is an alert that shows Actively Hiring/Recruiting, or “Others” for alerts that are different than the two previously mentioned ones.
4. The Posting Date attribute should correspond to the time elapsed since the publication of the job offer (as displayed in the job post).
5. The Offer URL should correspond to the URL address for the more detailed job description page.
6. The Number of Applicants attribute should be stored in integer form. In some cases, you'll notice that the text "Be among the first 25 applicants" appears where the number of applications should be. For this case, the retrieved value should be 25.
7. The Promoted attribute should be encoded with a True if the job offer is Promoted and with a False otherwise.
8. The Workspace attribute should include information about whether the job offer is Hybrid, On-site , Remote or Other
9. The Seniority attribute should encode the level of the job, i.e. whether it's Entry, Mid-Senior, Senior, etc.
10. The Employment Type attribute should encode the work schedule, i.e. whether it's Full-time, Part-time, etc.
11. The Industry attribute should encode the sector of industry the company belongs to
12. The Python Required atribute should be equal to True if the word Python is mentioned in the Job Description (your check should not be case sensitive), or False if the word python is not mentioned in the Job Description.
13. In some cases, it is possible to apply for the job directly through LinkedIn using the Easy apply feature. In others, the offer will redirect you to the company's website where you can complete the applications process. The Application through Linkedin attribute should include a True whenever Easy apply is enabled and a False otherwise
14. The Number of Employees attribute should be stored in integer form and displayed the number of employees of the company offering the job. Should be filled by a pandas NaN when the company name is not specified, or the number of employees is not specified.
15. In all cases, strings should be properly formatted by removing any unnecessary spaces.
