

```md
# Doctors Appointment System

## Overview
This system allows patients to book doctor appointments. It provides an API to manage appointments, including booking, updating, viewing, and deleting appointments.

## Features
- **Book Appointments**: Patients can schedule appointments by providing their name, doctor’s name, and appointment date.
- **View Appointments**: Retrieve a list of all scheduled appointments.
- **Get Appointment Details**: Fetch details of a specific appointment by ID.
- **Update Appointment Status**: Change the status of an appointment to **Scheduled, Completed, or Canceled**.
- **Delete Appointments**: Only canceled appointments can be deleted.
- **Database Storage**: All appointment data is stored in a database.

## API Endpoints
### 1. **Create an Appointment**
   **Endpoint:** `POST /api/appointments/create`  
   **Body:**
   ```json
   {
     "patientName": "Ali",
     "doctorName": "Dr. Shahzaib",
     "appointmentDate": "2025-03-01",
     "status": "Scheduled"
   }
   ```

### 2. **View All Appointments**
   **Endpoint:** `GET /api/appointments/all`

### 3. **Get a Specific Appointment**
   **Endpoint:** `GET /api/appointments/{id}`  

### 4. **Update Appointment Status**
   **Endpoint:** `PUT /api/appointments/{id}/update-status?status=Completed`

### 5. **Delete an Appointment**
   **Endpoint:** `DELETE /api/appointments/{id}/delete`  
   *(Only possible if the status is `Canceled`)*






