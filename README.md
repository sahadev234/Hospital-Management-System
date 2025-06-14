🏥 Hospital Management System
A full-stack Hospital Management System built using Spring Boot, implementing MVC architecture and JPA for database operations. This project is designed to streamline hospital operations like appointment scheduling and user role management, while maintaining a clean separation of concerns and secure access.

🚀 Features
🗓️ Appointment Scheduling: Patients can book appointments with available doctors.

👨‍⚕️ Doctor Dashboard: View appointments and manage availability.

🛠️ Admin Dashboard: Manage users, doctors, and appointments.

🔒 Session Handling & RBAC: Role-Based Access Control for secure access to features.

✉️ Email Notifications: Appointment confirmation emails are sent automatically.

🎨 Thymeleaf Integration: Server-side view rendering using Thymeleaf templates.

🛡️ Spring Security: Authentication and authorization handled using Spring Security.

🧰 Tech Stack
Backend: Spring Boot (MVC, Spring Security, Spring Data JPA)

Frontend: Thymeleaf (HTML, CSS, Bootstrap)

Database: MySQL (via JPA/Hibernate)

Email: JavaMailSender for sending confirmation emails

Security: Spring Security with session-based authentication and RBAC

📂 Project Structure
bash
Copy
Edit
src/
├── main/
│   ├── java/com/hms/       # Java source code
│   │   ├── controller/      # MVC controllers
│   │   ├── model/           # Entity classes
│   │   ├── repository/      # Spring Data JPA repositories
│   │   ├── service/         # Business logic
│   │   └── security/        # Security configuration
│   └── resources/
│       ├── templates/       # Thymeleaf templates
│       ├── static/          # Static assets (CSS, JS)
│       └── application.properties
⚙️ Setup & Run
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/hospital-management-system.git
cd hospital-management-system
Configure the Database
Update your application.properties file with your MySQL DB credentials.

Run the Application
You can run the project using:

bash
Copy
Edit
./mvnw spring-boot:run
Access the App
Open http://localhost:8080 in your browser.

🔐 Default Roles
Admin: Can manage doctors, patients, and appointments.

Doctor: Can view and manage their appointments.

Patient/User: Can book and view appointments.

📧 Email Configuration
To enable email service, configure the following in application.properties:

properties
Copy
Edit
spring.mail.host=smtp.example.com
spring.mail.port=587
spring.mail.username=your_email@example.com
spring.mail.password=your_password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true
📌 Future Enhancements
Patient medical record management

Prescription module

REST API endpoints for mobile integration

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📄 License
This project is open-source and available under the MIT License.
