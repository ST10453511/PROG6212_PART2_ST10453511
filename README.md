ST10453511
Moegammad Alexander 
PROG6212
POE PART 2

GitHub Link:
https://github.com/ST10453511/PROG6212_PART2_ST10453511.git 

YouTube Link:
https://youtu.be/gpLDhu-UuL4

Contract Monthly Claim System (CMCS)
A .NET Core MVC Web Application for Streamlining Lecturer Claim Submissions and Approvals

Overview:
The Contract Monthly Claim System (CMCS) is a practical ASP.NET Core MVC web application designed to simplify and automate the monthly claim process for Independent Contractor (IC) lecturers at tertiary institutions. The system simulates a real-world administrative workflow where lecturers submit claims for hours worked, Programme Coordinators verify them, and Academic Managers finalize approvals. CMCS provides a clean, role-based user interface for efficient claim tracking, document uploading, and secure data management — focusing on usability, responsiveness, and transparency.

Objectives:
This project forms Part 2 of the PROG6212 Portfolio of Evidence (PoE). The objectives are to demonstrate practical implementation of C# GUI development using ASP.NET Core MVC, apply concepts of authentication, authorization, validation, and file management, create a functional multi-role web platform reflecting a real administrative workflow, and showcase UI design, user experience, and logical integration of business rules.

Key Features:
Lecturer Functions:
Lecturers can submit new claims for the hours they have worked. Each claim includes the date worked, hours worked, hourly rate, activity description (such as lecturing or marking), and optional supporting documents in formats like PDF, DOCX, or XLSX. Notes can also be added for extra details. The total amount is automatically calculated in real-time based on hours multiplied by the hourly rate. Uploaded documents are securely stored and linked to the respective claim.

On the dashboard, lecturers can view their most recent submissions, showing details such as the date, activity, total amount, and claim status. A progress bar visually indicates the current claim stage, such as “Submitted”, “Under Review”, or “Approved/Rejected”.

In the “My Claims” view, lecturers can see a complete overview of all their claims with search and filter options. This allows them to check progress, verify statuses, and confirm that their claim was reviewed or approved.

Programme Coordinator Functions:
Programme Coordinators serve as the first level of review for lecturer claims. They can view all pending claims on a dedicated dashboard and open each claim to verify details, review uploaded documentation, and ensure the information is accurate. Coordinators can approve valid claims or reject incomplete or incorrect ones, leaving a comment or note where necessary. Once approved, the claim automatically moves to the Academic Manager’s review list for final approval.

Academic Manager Functions:
Academic Managers review the claims that have been verified by Programme Coordinators. They are responsible for the final stage of the process — reviewing, approving, or rejecting the claims to ensure compliance with institutional and budgetary policies. They have access to detailed claim information and supporting documentation. Any changes made at this stage are reflected in real-time on the lecturer’s dashboard, maintaining transparency and accountability throughout the system.

Claim Status Tracking:
The CMCS includes a transparent claim tracking system that updates in real-time. Each claim moves through several statuses, beginning as “Submitted”, then “Under Review”, and finally being marked as either “Approved” or “Rejected”. The status is displayed both as a text label and through a visual progress bar that updates automatically whenever a coordinator or manager performs an action on a claim. This ensures lecturers can track their claims at every step until settlement.

System Architecture:
The system follows the MVC (Model-View-Controller) architecture. The controllers handle user requests and link them to views and models. The models define all necessary data structures, such as Claim, ClaimStatus, and User. The Razor Views provide interactive, responsive interfaces using Bootstrap and custom CSS. Data is managed using in-memory stores for simplicity, such as InMemoryUserStore and InMemoryClaimStore. File uploads are handled securely through LocalFileStorage, which stores uploaded documents and links them to the correct claims.

Authentication & Roles:
The CMCS uses Cookie Authentication to handle user sessions. Each user role has specific permissions and available features. Lecturers can submit and track claims, Programme Coordinators can verify and comment on claims, and Academic Managers provide the final approval or rejection. There is also an admin account for demonstration purposes. For simplicity in testing, the password for each demo user is the same as their username.

File Upload & Validation:
The file upload system is designed for simplicity and security. Users can upload only PDF, DOCX, or XLSX files, with a maximum file size of 5 MB. The uploaded documents are validated on both the client and server sides before being securely stored. The IFileStorage interface ensures all uploads are properly linked to the relevant claim record. Error messages are displayed if uploads fail validation, ensuring the user is guided to correct any issues.

Error Handling:
The application provides robust error handling for common issues such as incomplete forms, missing required data, invalid file types, and unauthorized access attempts. Validation messages guide the user through form completion, while Bootstrap toast notifications provide immediate feedback on successful submissions or errors. This ensures the application remains stable and user-friendly throughout.

User Interface Design:
The interface is designed to be modern, clean, and intuitive. A black navbar at the top includes a small CMCS brand logo for easy recognition. The welcome page features a gradient background and rounded, shadowed cards for a modern feel. Icons are used throughout to visually represent different user roles and functions, making navigation straightforward and engaging. Typography is minimal and professional, ensuring a visually consistent and readable experience for all users. The layout automatically adapts to different screen sizes, ensuring full responsiveness across devices.

Technologies Used:
The CMCS web application is built using ASP.NET Core MVC 8 and C#. The frontend design uses Bootstrap 5 and custom CSS for styling. Cookie Authentication is implemented for secure login sessions. Data is temporarily stored using in-memory lists and local file storage instead of a database. The project is developed in Visual Studio 2022 and version-controlled using Git and GitHub.

Testing & Validation:
All user flows have been manually tested, including login, claim submission, file uploads, and role-based navigation. Form validation was tested using required, range, and data type attributes. File uploads were tested with valid and invalid files to ensure correct validation behavior. The navigation structure was verified to show only the correct options for each user role. Real-time status updates were simulated and confirmed to update promptly after each action.

Submission & Deliverables:
The final submission includes the complete CMCS source code, documentation, and demonstration screenshots. A Word document is provided separately to include lecturer feedback and explanations of how improvements were implemented based on recommendations. The GitHub repository hosts all code and documentation, ensuring transparency and version history.

Conclusion:
The Contract Monthly Claim System is a fully functional ASP.NET Core MVC web application that demonstrates the integration of authentication, authorization, validation, and file management within a modern GUI. It models real-world academic administrative workflows and provides an efficient, transparent, and user-friendly system for claim management. The application meets the requirements of the PROG6212 Part 2 assessment and provides a solid foundation for further development in future project stages.
