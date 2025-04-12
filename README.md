# WRNL Volunteer Attendance Portal WebApp 

## wearenotlemons.github.io
This repository contains static assets (eg. images) used by the various frontend deployments and provides a simple URL redirect to the NYJC We Are Not Lemons (WRNL) Volunteer Attendance Portal.

- [wearenotlemons.github.io](https://wearenotlemons.github.io) redirects to WRNL Attendance Portal v2.1 (Hosted on Vercell)
- [wearenotlemons.github.io/v2](https://wearenotlemons.github.io/v2) redirects to WRNL Attendance Portal v2 (Hosted on Render)
- [wearenotlemons.github.io/attendance](https://wearenotlemons.github.io/attendance) redirects to WRNL Attendance Portal v1.1 (Hosted on Google Apps Script)

## Overview
The WRNL Volunteer Attendance Portal WebApp provides a centralised platform for displaying volunteer attendance data and tracking total volunteer hours. It is designed to provide a convenient view of session participation and volunteer contributions.

## Components

**v2.1:** Vercel (Frontend deployment) -> Github (Codebase) -> Google Apps Script (API) -> Google Sheet

**v2:** Render (Frontend deployment) -> Github (Codebase) -> Google Apps Script (API) -> Google Sheet

**v1.1:** Google Apps Script -> Google Sheet

### Version 2 
- **Frontend:** Developed using HTML, CSS, and JavaScript, with all static assets stored in this Github repository, and code stored in the respective GitHub repositories.
  - The frontend captures user input (e.g. volunteer name) and queries the backend for relevant attendance data, which is dynamically rendered on the user interface. It communicates with the backend via API calls to retrieve data.
- **Backend:** Built using Python (Flask), with the application code stored in the respective GitHub repositories and deployed on **Vercel/Render**.
  - The backend processes frontend requests, retrieves necessary data from Google Sheets via Google Apps Script, and serves it to the frontend.
- **Google Apps Script API:** Facilitates data access and retrieval, enabling the backend to query the sheet for real-time information.
- **Google Sheets Integration:** Acts as the real-time data store for volunteer attendance records.
  - All volunteer-related data, including volunteer information and session details, is stored in Google Sheets. The Google Sheets integration provides the WRNL organising committee with a no-code solution for updating volunteer attendance entries.
- **GitHub Integration:** Serves as the code repository for both frontend and backend components, facilitating version control, collaboration, and deployment.
  - In this repository:
    1. Stores static assets (eg. favicon, header image)
    2. Uses Github pages for URL redirect to various versions of the WebApp
  - Within respective repositories:
    1. Stores the complete source code for the web application, including HTML files (frontend) and Python scripts (backend). 

## Portal Link
- [Access the Portal](https://wearenotlemons.github.io)
