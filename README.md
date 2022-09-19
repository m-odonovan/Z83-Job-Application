# Z83-Job-Application
Z83 Job Application solution is designed to be used by South African public sector organizations. It is built on the Microsoft Power Platform, and uses Microsoft Power Apps and Power Pages mostly. It allows a department to Manage job vacancies published to a portal and support online applications according to Z83 format application form format.

## Background
Use "as-is" or customise as appropriate.

Provides the following features:
1. Create and manage job vacancies in a central admin application (Model Driven Power App)
2. Schedule, auto publish and remove the vacancy from the online web portal (Power Pages)
3. Allow applicants to apply online using same fields required in paper based Z83 form. Enforces integrity and accuracy of information through data validation, choice fields, required fields and more.
4. Submitted applications are saved associated to the job vacancy for easy review
5. Basic analytics provided for job vacancies and applications.

## Its a starter / sample
Please do note, this is a sample application that is not intended to be used in production environments as is. It is intended to help a Power Apps developer to learn how they could assemble such an application. It is certainly not a perfect solution, it hasn't been well tested, and is missing some key features that I hope to add over time.

## How it works
There are 2 main applications which makeup this solution. 
1 - Admin Model Driven App
2 - User Canvas App

All data resides in the Microsoft Dataverse (CDS), both job vacancies, job applications, master data, uploaded documents and more.

The admin model driven app is where you setup your WizAuds. A WizAud is something you want to capture e.g. Site Inspection, Vehicle Inspection, Request for Leave etc. Within a WizAud you define what fields (questions) you would like a person using the Canvas app to complete. A WizAud has a name, option start and end date, and some future feature flags e.g. generate PDF, request final signature etc. Each field has a data type, and order where it appears in the list of questions, required or not, if notes field should be displayed and if images should be captured for the question (future feature).

The canvas app is a 2 screen sample app designed for phone form factor. First screen lists the WizAuds available for the user to complete, and also shows draft responses and previous responses. When you select a WizAud to complete, you are take to the second screen which lists the questions/fields the user should complete. Save as Draft will allow you to save a response to be submitted later e.g. because you are offline, and Submit button submits data to backend (CDS). Submit button is not available if offline.

Solution file and overview PPT is in the solution folder.
