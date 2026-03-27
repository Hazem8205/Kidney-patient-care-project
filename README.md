# Kidney-patient-care-project
Kidney Patient Care in MRI Images Using CNNs
AI-Powered Diagnostic Support Tool for Renal Pathologies
This project is a comprehensive full-stack application designed to assist radiologists in classifying kidney illnesses from MRI scans. It leverages deep learning to provide accurate, rapid, and objective second opinions for renal diagnosis.

📝 Project Overview
The system addresses the inefficiency and potential for diagnostic variability in manual MRI analysis. It classifies kidney conditions into four primary categories:

Class 0: Normal - MRI scans showing no signs of pathology.

Class 1: Cyst - Simple or complex renal cysts.

Class 2: Tumor - Benign and malignant renal tumors.

Class 3: Stone - Nephrolithiasis (kidney stones).

🏗️ System Architecture
The application follows Clean Architecture principles and a microservices-inspired structure:

Data Layer: Handles acquisition from sources like TCIA, preprocessing (normalization/resizing), and data augmentation.

Model Layer: Core CNN development using EfficientNetB3 with transfer learning and fine-tuning strategies.

Application Layer: A multi-layered web interface connecting users to the AI backend.

🛠️ Technology Stack
Backend (ASP.NET Core 8)

Framework: Built for high performance and strong type safety.

Authentication: JWT (JSON Web Tokens) with ASP.NET Core Identity.

Real-time: SignalR for instant messaging between doctors and patients.

ORM: Entity Framework Core for database management.

AI Service (FastAPI & TensorFlow)

API Framework: FastAPI for high-performance, asynchronous model serving.

DL Framework: TensorFlow/Keras for CNN implementation.

Explainability: Grad-CAM heatmaps to highlight areas influencing the model's decision.

Frontend (React & TypeScript)

UI Library: React 18 with a component-based architecture.

State Management: Redux Toolkit for global application state.

Styling: CSS Modules for maintainable, scoped styling.

🚀 Key Features

Automated Classification: Rapidly detects cysts, tumors, or stones from uploaded images.

Explainable AI: Provides visual heatmaps (Grad-CAM) to build clinician trust.

Doctor-Patient Portal: Includes appointment booking, medical history tracking, and real-time chat.

Health Management: Automated medication and appointment reminders.

Dashboard Analytics: Comprehensive metrics for administrators and healthcare providers.

🔐 Security & Deployment

Data Protection: AES-256 encryption at rest and TLS 1.3 for transit.

Containerization: Fully containerized using Docker and orchestrated with Docker Compose.

CI/CD: Automated testing and deployment pipeline for zero-downtime updates.
