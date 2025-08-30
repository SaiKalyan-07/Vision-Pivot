# Vision-Pivot
**Face-Based Attendance System with Real-Time Admin Dashboard**
---
## Project Summary

- **Title:** Vision Pivot
- **Objective:** A secure, automated face recognition attendance system integrated with React-based admin dashboard for real-time monitoring and management.

### Key Features

- **Face Recognition:** Real-time attendance marking using MTCNN + FaceNet.
- **Firebase Backend:** Central storage of attendance logs, user data, and admin authentication.
- **React Admin Dashboard:**
  - Secure login for admins (Firebase Auth).
  - View, edit, and manage attendance logs.
  - Add/remove users and assign roles.
  - Export reports in CSV/PDF.
- **Anti-Spoofing:** Prevents duplicate attendance for the same session.

---

##  Updated Workflow

### Pipeline Overview

1. **Admin Setup**
   - Secure login via React dashboard (Firebase Email/Password Auth).
   - Upload user images through the UI.

2. **Enrollment Phase**
   - `face_embeddings.py` automatically  generates and stores `.npy` face embeddings for new users.

3. **Attendance Marking**
   - `attendance_system.py` runs a live camera feed, matches faces, and logs attendance in Firebase.

4. **Admin Actions**
   - View history, filter records, override or correct entries, and manage users/roles in real-time.

---

