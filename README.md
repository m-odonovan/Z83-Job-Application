# Z83-Job-Application
Z83 Job Application solution is designed to be used by South African public sector organizations. It is built on the Microsoft Power Platform, and uses Microsoft Power Apps, Power Pages and Power Automate mostly. It allows a department to Manage job vacancies published to a portal and support online applications according to Z83 application form format.

## Background
Use "as-is" or customise as appropriate.

Provides the following features:
1. Create and manage job vacancies in a central admin application (Model Driven Power App)
2. Schedule, auto publish and remove the vacancy from the online web portal (Power Pages)
3. Allow applicants to apply online using same fields required in paper based Z83 form. Enforces integrity and accuracy of information through data validation, choice fields, required fields and more.
4. Submitted applications are saved associated to the job vacancy for easy review, along with a auto generated PDF version
5. Basic analytics provided for job vacancies and applications.

## Its a starter / sample
Please do note, this is a a starter / sample. It hasn't been well tested, and is missing some key features that I hope to add over time. It not officialy supported by myself or Microsoft. However, because the unmanaged and managed solution is provided, you should be able to support it yourself, either directly or through a certified Microsoft partner.

## How it works
There are 2 main applications which makeup this solution. 
1 - Admin Model Driven App (Z83 Manager)
2 - Power Portal / Power Pages site

All data resides in the Microsoft Dataverse. This includes job vacancies, job applications, master data, uploaded documents and more.

The admin model driven app is where you setup your job vacancies, job vacancies parameters like job description, salary level and more. You configure when it should be auto published to portal, and when it should be removed / applications close. 

Admin App
![Admin App](https://github.com/m-odonovan/Z83-Job-Application/blob/main/images/z83admin.gif "Admin App")

The portal allows for applicants to see vacancies, and apply. Applications are saved associated to the vacancy so that they can be screened / processed.

Web Portal
![Web App](https://github.com/m-odonovan/Z83-Job-Application/blob/main/images/z83web.gif "Power Pages Portal")

More information on how the solution works, including demo is in the attached Solution Demo PPT.

## Installation instructions
Documented in the instructions PPT.
