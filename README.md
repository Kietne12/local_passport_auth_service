# Test local_passport_auth_service

1. Register  
POST http://localhost:3000/auth/register
Body: { "username": "admin2", "password": "12345" }
![Register Request](public/results/register.png)

2. Login  
POST http://localhost:3000/auth/login  
Body: { "username": "admin2", "password": "12345" }
![Login Request](public/results/login.png)

3. Profile (sau khi login)  
GET http://localhost:3000/auth/profile 
![Profile Response](public/results/profile.png)

4. Logout  
GET http://localhost:3000/auth/logout
![Logout Response](public/results/logout.png)

5. Profile sau khi logout  
GET http://localhost:3000/auth/profile
![Profile After Logout](public/results/profile_after_logout.png)
