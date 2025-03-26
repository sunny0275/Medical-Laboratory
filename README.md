# Medical-Laboratory
MedTest Lab Database Management System
echo '# MedTest Lab System

## Overview

MedTest Lab is a comprehensive laboratory management system designed to streamline the process of managing medical tests, patients, and results. The system provides an efficient way for healthcare providers to order tests, track patient information, and manage test results in a secure environment.

## Features

- **Patient Management**: Register and manage patient information
- **Test Ordering**: Create and track medical test orders
- **Result Management**: Record and retrieve test results
- **User Authentication**: Secure login system with role-based access
- **Reporting**: Generate reports on test results and patient history
- **Notification System**: Alert patients and healthcare providers about test results

## Technology Stack

- **Backend**: Python with Flask framework
- **Database**: SQLite for development, PostgreSQL for production
- **Frontend**: HTML, CSS, JavaScript with Bootstrap for responsive design
- **Authentication**: JWT (JSON Web Tokens)
- **Testing**: Pytest for unit and integration tests
- **Containerization**: Docker for easy deployment

## Installation

### Standard Installation

1. Clone the repository:

git clone https://github.com/yourusername/medtest_lab_final.git

2. Navigate to the project directory:

cd medtest_lab_final

3. Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

4. Install dependencies:

pip install -r requirements.txt

5. Set up the database:

flask db init
flask db migrate
flask db upgrade

6. Start the application:

flask run

### Docker Deployment

1. Clone the repository:

git clone https://github.com/yourusername/medtest_lab_final.git

2. Navigate to the project directory:

cd medtest_lab_final

3. Build the Docker image:

docker build -t medtest-lab .

4. Run the container:

docker run -p 5000:5000 medtest-lab

5. For Docker Compose deployment:

docker-compose up -d

This will start the application along with a PostgreSQL database container.

## Usage

1. Access the application at `http://localhost:5000`
2. Log in with your credentials
3. Navigate through the dashboard to access different features:
   - Patient registration
   - Test ordering
   - Result management
   - Reports
   - 
## Configuration

Configuration settings can be modified in the `config.py` file. The application supports different environments:

- Development
- Testing
- Production

Environment variables can be set in the Docker environment or through a .env file for Docker Compose.

## Testing

Run the test suite with:

pytest

For Docker:

docker run medtest-lab pytest

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m '"'"'Add some feature'"'"'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
