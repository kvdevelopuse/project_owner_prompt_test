# Student & Batch Management Requirements

This is the complete scope. Nothing beyond these three sections is to be built.

## 1. Student Registration

The system shall let users register a new student. **All fields are mandatory.**

| Field | Description |
|---|---|
| Full Name | Student's full name |
| Gender | Selection (e.g., Male / Female) |
| Date of Birth | Date picker |
| Phone Number | Contact number |
| Emirates ID Number | See Emirates ID rules below |

**Emirates ID rules:**

- **Input mask:** As the user types, the field shall format the value as `784-XXXX-XXXXXXX-X` and add the hyphens automatically. The user enters digits only.
- **Format check:** The system shall accept only a 15-digit number that starts with 784, in the format `784-XXXX-XXXXXXX-X`.
- **Uniqueness:** The system shall reject an Emirates ID number that is already registered.

## 2. Batch Master

The system shall let users create and manage batches with the following details:

| Field | Mandatory | Description |
|---|---|---|
| Location | Yes | Where the batch is held |
| Batch Name | Yes | Name of the batch |
| Description | No | Short description of the batch |
| Age Group | Yes | Target age group for the batch |
| Days of the Week | Yes | Checkboxes (Mon–Sun); more than one day can be selected |
| Monthly Fee | Yes | Fee charged per month |
| Number of Sessions per Month | Yes | Fixed number entered by the user |

## 3. Student–Batch Assignment

The system shall support this workflow:

1. Register a student.
2. Create a batch.
3. Assign a registered student to an existing batch.

**Rules:**

- A student can belong to only one batch at a time.
- The system shall not check a student's age against the batch's age group.
