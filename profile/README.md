
# DiscoverMe Project

Welcome to the DiscoverMe project! DiscoverMe is a comprehensive web-based application designed to help users track their mood, log journal entries, set personal goals, and gain insights into their mental health trends. The project consists of three main repositories, each focusing on a different aspect of the application.

## Project Repositories

1. **DiscoverMe-GUI**: The frontend user interface built with Vue.js.
   - Repository Link: [DiscoverMe-GUI](https://github.com/DiscoverMe-Team/DiscoverMe-GUI)
   - Key Features:
     - Custom Dashboard for tracking mood, journal entries, and goals.
     - Dynamic navigation using PrimeVue components.
     - API integration for fetching and displaying user data.

2. **DiscoverMe-API**: The backend API built with Django.
   - Repository Link: [DiscoverMe-API](https://github.com/DiscoverMe-Team/DiscoverMe-API)
   - Key Features:
     - Provides RESTful endpoints for managing user data.
     - Handles user authentication using JWT tokens.
     - Manages models for moods, mood logs, journal entries, goals, and insights.

3. **DiscoverMe-Infra**: Infrastructure as code using AWS CDK for cloud deployment.
   - Repository Link: [DiscoverMe-Infra](https://github.com/DiscoverMe-Team/DiscoverMe-Infra)
   - Key Features:
     - Deploys the application to AWS using services like EC2, RDS, and Cognito.
     - Manages infrastructure resources for scalability and reliability.
     - Automates deployment using AWS CloudFormation.

## Project Overview

DiscoverMe helps users:
- Log and track their daily moods.
- Write journal entries for self-reflection.
- Set and monitor personal goals related to mental health and self-improvement.
- Analyze trends with mood insights and personalized suggestions.

## Getting Started

To get started with the entire DiscoverMe project, follow these steps:

### 1. Clone the Repositories

```bash
git clone https://github.com/DiscoverMe-Team/DiscoverMe-GUI.git
git clone https://github.com/DiscoverMe-Team/DiscoverMe-API.git
git clone https://github.com/DiscoverMe-Team/DiscoverMe-Infra.git
```

### 2. Install Dependencies

- **Frontend (Vue.js)**
  ```bash
  cd DiscoverMe-GUI
  npm install
  ```

- **Backend (Django)**
  ```bash
  cd ../DiscoverMe-API
  pip install -r requirements.txt
  ```

- **Infrastructure (AWS CDK)**
  ```bash
  cd ../DiscoverMe-Infra
  npm install
  ```

### 3. Configure Environment Variables

Set up the `.env` files for both the frontend and backend:

- **Frontend (`.env`)**
  ```
  VUE_APP_API_BASE_URL=http://localhost:8000/api
  ```

- **Backend (`.env`)**
  ```
  SECRET_KEY=your_secret_key
  DEBUG=True
  DATABASE_URL=your_database_url
  ```

### 4. Run the Application

- **Start the Django API Server**
  ```bash
  cd DiscoverMe-API
  python manage.py runserver
  ```

- **Start the Vue Development Server**
  ```bash
  cd ../DiscoverMe-GUI
  npm run serve
  ```

- **Deploy Infrastructure (AWS)**
  ```bash
  cd ../DiscoverMe-Infra
  cdk deploy
  ```

### 5. Access the Application

Open your browser and go to:
```
http://localhost:8080
```

## Project Structure

- **DiscoverMe-GUI**
  - `src/components/`: Reusable Vue components.
  - `src/views/`: Main pages of the application.
  - `src/services/`: API service files for data fetching.

- **DiscoverMe-API**
  - `base/models.py`: Django models for moods, journal entries, mood logs, etc.
  - `base/views.py`: API views for handling requests.
  - `base/serializers.py`: Data serializers for API responses.

- **DiscoverMe-Infra**
  - `lib/`: AWS CDK infrastructure definitions.
  - `bin/`: Entry point for the CDK application.

## Documentation

- [How to Add a New Page](https://github.com/DiscoverMe-Team/DiscoverMe-GUI/wiki/How-to-Add-a-New-Page)
- [API Integration Guide](https://github.com/DiscoverMe-Team/DiscoverMe-GUI/wiki/API-Integration)
- [Component Guide](https://github.com/DiscoverMe-Team/DiscoverMe-GUI/wiki/Component-Guide)

## Team Members

- **William Alston**: Project Lead
- **Zach**: Frontend Developer & UI/UX Design
- **Connor**: Backend & API Integration Specialist
- **Anisa**: Infrastructure & Deployment

## Troubleshooting

- Ensure all services are running and configured correctly.
- Check the browser console and Django logs for error messages.
- If you encounter deployment issues, verify your AWS credentials and configuration.

## Contact

For any questions or issues, please open an issue on the relevant GitHub repository or contact the project lead.

---

Thank you for using DiscoverMe! We hope this project helps you track your mental health journey effectively.
