# Project in Jira : OrangeHRM 

The scope of the project is to use all gained knowledge throught the course and apply them in practice, using a live application.

Application under test:  <a href="https://duckduckgo.com](https://opensource-demo.orangehrmlive.com/web/index.php/auth/login" target="_blank"> OrangeHRM</a>

API Documentation: chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://www.orangehrm.com/assets/Files/Complete-Administrative-User-Guide.pdf?url=/Files/Complete-Administrative-User-Guide.pdf

Tools used: Jira Scrum Zephyr

# # OrangeHRM Functional Specifications

## 1. Employee Information Management

**Description**: A centralized system where all employee data (personal and professional) is stored, managed, and accessible by HR personnel and managers.

### Use Case:
- As an HR manager, I want to view and update an employee's information (name, contact details, position, department) to ensure records are accurate.

### Functional Requirements:
- The system must allow HR to create new employee profiles, edit existing profiles, and deactivate profiles.
- The system must store personal details like full name, address, contact details, and professional details such as job title, department, hire date, and salary.
- HR personnel must be able to upload documents (e.g., contracts, performance reviews) to the employee's profile.
- Search functionality should allow users to search for employees by name, department, or job title.

### Acceptance Criteria:
- When a new employee is added, all required fields (name, hire date, position) must be filled before saving.
- The system should send a confirmation email to HR upon creating or updating an employee profile.
- An error message should be shown if any required fields are missing.
- HR should be able to deactivate employees, and deactivated profiles should not appear in active employee lists.

### Dependencies:
- This feature must be integrated with the Payroll system for salary information.

---

## 2. Leave Management

**Description**: A feature that allows employees to request leave, and managers to approve or reject these requests.

### Use Case:
- As an employee, I want to apply for leave online and get notified of the approval or rejection by my manager.
- As a manager, I want to view all pending leave requests and approve or reject them.

### Functional Requirements:
- Employees must be able to select the type of leave (sick leave, vacation, unpaid leave).
- The system must allow employees to specify the start and end date for the requested leave.
- Managers should receive notifications for pending leave requests and be able to approve or reject them.
- The system should display the employee's leave balance before submitting the request.

### Acceptance Criteria:
- Employees must not be able to request more leave days than their available balance.
- Once a leave request is submitted, it must be reflected in the employee's leave balance.
- Managers must receive notifications about pending requests, and employees must receive notifications about the decision.
- If a manager rejects a leave request, a reason for rejection must be provided.

### Dependencies:
- Integrated with the Employee Management module to access employee leave balances.

---

## 3. Recruitment Management

**Description**: A module that manages the end-to-end recruitment process, from job posting to candidate selection.
Use Case:
- As a recruiter, I want to post job vacancies and track applications from potential candidates.
- As a hiring manager, I want to shortlist candidates and schedule interviews.
- 
### Functional Requirements:
- The system must allow recruiters to create and post job openings, specifying title, department, location, and required skills.
- Candidates must be able to submit applications online, including their resume and cover letter.
- Recruiters must be able to review applications, shortlist candidates, and send interview invitations.
- The system must track the status of each job (open, closed) and each candidate (applied, shortlisted, interviewed, rejected).

### Acceptance Criteria:
- Candidates should receive confirmation emails upon submitting applications.
- Recruiters must be able to update the status of candidates at every stage (e.g., application received, shortlisted, interview scheduled).
- The system must prevent duplicate job postings with the same title and department.
- 
### Dependencies:
- Integrated with the Employee Information module for onboarding candidates after selection.

  ---

  ## 4.Feature: Performance Management
  
**Description**: A system for tracking and evaluating employee performance based on goals and feedback.

### Use Case:
- As an employee, I want to view my performance objectives and see feedback from my manager.
- As a manager, I want to set performance goals for my team and provide feedback regularly.
### Functional Requirements:
- Managers must be able to set performance goals for each employee.
- Employees should be able to view their goals and track their progress.
- The system must allow managers to provide feedback and ratings for each goal.
- A final performance evaluation should be calculated based on the individual ratings.
### Acceptance Criteria:
- Employees should receive notifications when new goals are set.
- Managers must be able to modify goals and provide feedback throughout the evaluation period.
- The system should calculate the overall performance score based on individual ratings.
### Dependencies:
Integrated with the Employee Information module to link evaluations to specific employees.





