
# AI-Based Attendance Software

This repository contains the code for an AI-based attendance tracking system that uses facial recognition for automated attendance. The backend is built using Django, while the deep learning model for facial recognition ensures accurate identification. The system stores and retrieves data using MySQL, with seamless integration via RESTful APIs.

## Features

- **Automated Attendance Tracking:** Utilizes a deep learning model for facial recognition to automatically mark attendance.
- **Real-Time Data Processing:** Provides real-time attendance tracking with swift and accurate facial recognition.
- **RESTful APIs:** Designed for smooth communication and data exchange between the frontend and backend.
- **User-Friendly Interface:** An intuitive interface for educators to easily manage and track attendance.
- **Secure Data Storage:** MySQL database used for efficient storage and retrieval of student attendance records.

## Technologies Used

- **Backend Framework:** Django
- **Deep Learning Model:** TensorFlow/PyTorch (for facial recognition)
- **Database:** MySQL
- **API:** RESTful APIs
- **Facial Recognition Libraries:** OpenCV, dlib, face_recognition

## Prerequisites

Before running the project, ensure you have the following installed:

- Python 3.8+
- Django
- MySQL
- TensorFlow/PyTorch
- OpenCV
- dlib
- face_recognition

## Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/ai-attendance-software.git
   cd ai-attendance-software
   ```

2. **Install dependencies**  
   Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up MySQL database**  
   Create a database in MySQL and update the `settings.py` file with your database credentials:
   ```python
   DATABASES = {
       'default': {
           'ENGINE': 'django.db.backends.mysql',
           'NAME': 'your_database_name',
           'USER': 'your_mysql_username',
           'PASSWORD': 'your_mysql_password',
           'HOST': 'localhost',
           'PORT': '3306',
       }
   }
   ```

4. **Run migrations**  
   ```bash
   python manage.py migrate
   ```

5. **Start the development server**  
   ```bash
   python manage.py runserver
   ```

## Usage

1. **Upload Student Data:**  
   Use the web interface to upload student data with their corresponding images.

2. **Run Attendance:**  
   The system captures images or video input and runs facial recognition to mark attendance automatically.

3. **View Attendance Records:**  
   Educators can view and manage attendance records through the dashboard.

## Project Structure

- `/attendance/` - Main Django application containing models, views, and URLs.
- `/static/` - Static files for the web interface.
- `/templates/` - HTML files for the frontend.
- `/media/` - Directory for storing student images.
- `requirements.txt` - Python dependencies for the project.

## Future Improvements

- Integration with existing educational platforms like Google Classroom or Moodle.
- Mobile app interface for better accessibility.
- Advanced analytics and reporting on attendance trends.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request if you'd like to contribute.
