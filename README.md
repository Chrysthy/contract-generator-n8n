<h1 align="center">Automated Contract Generator 🗂️</h1>

<p align="center">
 An n8n workflow designed to automate the creation and delivery of rental contracts (built for event venues/properties). 
This system eliminates manual document generation by integrating web forms with the Google Workspace ecosystem.
</p>

<p align="center">  
  <a href="#-screenshots">Screenshots</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-overview">Overview</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-tools">Tools</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-how-to-run">How to Run</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-project">Project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-license">License</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-contributing">Contributing</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#support">Support</a>  
</p>

<br>

## 📸 Screenshots

<img src=".github/gif-do-projeto.gif" alt="gif do projeto">

<br>

## 🔗 Overview

1. ⚡ **Trigger:** Automatically starts when a client submits a booking form.
2. 📄 **Processing:** Fetches a contract template from Google Docs and clones it into Google Drive.
3. ✍️ **Population:** Updates the newly created document by dynamically inserting form data (names, dates, amounts).
4. 🔗 **Sharing:** Adjusts file permissions to allow viewing.
5. ✉️ **Delivery:** Runs a logical check and automatically emails the finalized contract to the client via Gmail.

**Integrations used:** n8n, Google Docs, Google Drive, and Gmail.

<br>

## 🛠 Tools

* **Google Forms** 
* **Google Docs**
* **Google Drive**
* **Gmail** 
* **n8n Nodes**


<br>

## ⚙ How to Run

1. Install [n8n](https://docs.n8n.io/hosting/installation/).
2. Import the workflow JSON file.
3. Google Cloud Console: Create a project and enable the Google Drive, Google Docs, and Gmail APIs.
4. Credentials: In n8n, set up Google OAuth2 credentials to allow access to the services.
5. Template: Create a Google Doc with placeholders in double curly braces (e.g., {{name}}, {{date}}) for the n8n node to replace.
6.  Form: Set the trigger node to your preferred form builder (Google Forms, Typeform, etc.).
7.  File ID: In the "Copy file" node, paste the ID of your master template document.


<br>

## 📜 License

* This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/)
  
<br>
