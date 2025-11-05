# Healing-Hands

## Simple doctor appointment system (Express + MongoDB backend, React frontend build included).

### features
- User registration & login (JWT auth)
- Apply to be a doctor & admin approval flow
- View doctors and doctor details
- Book appointments and check availability
- Doctor dashboard: view and update appointments
- Notifications for users and doctors
- Admin: list users/doctors and change account status
- Uses Mongoose models for users, doctors and appointments
- Frontend production build served from client/build

### Quick start
- Install:
- ``` bash
  npm install
  ```
- Env: set MONGO_URL and JWT_SECRET (optional PORT)
- Run:
```bash
  npm start
```

### API notes
- Base path: /api/v1
- Protected routes require header: Authorization: Bearer <token>

### Project layout (important)
- server.js, config/db.js
- controllers/, routes/, middlewares/ (authMiddleware verifies JWT)
- models/: userModels.js, doctorModel.js, appointmentModel.js
- client/build included (production React)
