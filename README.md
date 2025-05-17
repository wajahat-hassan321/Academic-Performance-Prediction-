🎓 Student Exam Score Prediction Model
This project builds a machine learning pipeline to predict students' exam scores based on a range of academic, lifestyle, and demographic features. The model is trained using Linear Regression and evaluated through cross-validation.

📊 Dataset Overview
The dataset includes the following features:

Demographics: age, gender, parental_education_level

Habits: study_hours_per_day, social_media_hours, netflix_hours, sleep_hours, exercise_frequency

School factors: attendance_percentage, part_time_job, extracurricular_participation

Well-being: diet_quality, mental_health_rating, internet_quality

Target: exam_score (numerical)

🛠️ Preprocessing Steps
Missing Value Handling:

parental_education_level: imputed with the most frequent value

Encoding:

Ordinal Encoding:

parental_education_level: ['High School', 'Bachelor', 'Master']

diet_quality: ['Poor', 'Fair', 'Good']

internet_quality: ['Poor', 'Average', 'Good']

One-Hot Encoding:

gender, part_time_job, extracurricular_participation (with drop='first' to avoid multicollinearity)

Feature Scaling:

All numerical features (excluding the target) are scaled using MinMaxScaler

🧠 Model
The model uses Linear Regression, implemented within a scikit-learn Pipeline to ensure end-to-end preprocessing and modeling.

🔁 Model Evaluation
The model is evaluated using 10-fold cross-validation, measuring:

R² Score

Mean Absolute Error (MAE)

Mean Squared Error (MSE)
