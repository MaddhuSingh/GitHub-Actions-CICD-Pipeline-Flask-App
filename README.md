# Flask CI/CD Pipeline using GitHub Actions

## ** Overview**

This project demonstrates a complete CI/CD pipeline for a Flask application using GitHub Actions. It automates building, testing, and deployment processes.

---

## ** Workflow Stages**

### 1. Build & Test (CI)

* Installs dependencies using `pip`
* Runs automated tests using `pytest`
* Builds the application after successful tests

<img width="940" height="380" alt="image" src="https://github.com/user-attachments/assets/b266b911-28cf-43a0-8e76-e0be1a726605" />


  

### 2. Staging Deployment

* Triggered when code is pushed to the `staging` branch
* Simulates deployment to a staging environment

<img width="940" height="380" alt="image" src="https://github.com/user-attachments/assets/6c501552-fab8-4a53-bf0a-585140e4d57b" />


### 3. Production Deployment

* Triggered when a release is created (e.g., `v1.0`)
* Simulates deployment to production

<img width="940" height="381" alt="image" src="https://github.com/user-attachments/assets/7bacda66-4789-46bd-b43e-f7112190f8f2" />

After updating Readme file 

<img width="1912" height="847" alt="image" src="https://github.com/user-attachments/assets/af6273d8-afe2-4734-95fc-f85948305708" />

<img width="1902" height="907" alt="image" src="https://github.com/user-attachments/assets/466c6ffd-bde8-48b2-8801-2f35c56f683f" />


---

## ** Branch Strategy
**
* `main` → Production environment
* `staging` → Testing / staging environment

---

## ** Secrets Configuration**

The following secrets are configured in GitHub:

* `DEPLOY_KEY` → Used for staging deployment
* `API_TOKEN` → Used for production deployment

These secrets are securely stored in GitHub and accessed in workflows using:

```
${{ secrets.SECRET_NAME }}
```

---

##  **How It Works
**
* Push to `main` or `staging` → triggers CI pipeline
* Push to `staging` → deploys to staging
* Create a release → deploys to production

---

##**  Tools Used  **
* GitHub Actions
* Python (Flask)
* Pytest

## **Author**

**Madhu Singh**

* GitHub: https://github.com/MaddhuSingh

___________________________________________________________________________________________________________________________________________________________________

