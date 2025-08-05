# Student_Academic_Performance_Prediction-_roject

# 🎓 Student Performance Prediction Analysis
A comprehensive machine learning project that predicts student academic performance using demographic, social, and academic features. This analysis examines Mathematics and Portuguese language course performance to identify key factors influencing student success.

## 📊 Project Overview

This project analyzes student performance data from two Portuguese schools, focusing on Mathematics and Portuguese language courses. Using various machine learning algorithms, we predict final grades (G3) and identify the most influential factors affecting academic success.

### Key Highlights
- **📈 Predictive Models**: Random Forest, Decision Tree, and Linear Regression
- **🎯 Performance**: R² scores of 0.18-0.22 across subjects
- **🔍 Feature Analysis**: 30+ features including family background, study habits, and social factors
- **📋 Datasets**: 395 Mathematics students, 649 Portuguese students (382 overlap)

## 🚀 Quick Start

### Prerequisites
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### Installation
```bash
git clone https://github.com/yourusername/student-performance-prediction.git
cd student-performance-prediction
pip install -r requirements.txt
```

### Usage
```python
# Run the complete analysis
python student_performance_analysis.py

# For just the modeling part
python models.py

# Generate reports
python generate_report.py
```

## 📁 Dataset Information

### Data Sources
- **Mathematics Dataset**: `student-mat.csv` (395 students, 33 features)
- **Portuguese Dataset**: `student-por.csv` (649 students, 33 features)

### Key Features
| Category | Features | Examples |
|----------|----------|----------|
| **Demographic** | age, sex, address, famsize | Urban/Rural, Family size |
| **Family Background** | Medu, Fedu, Mjob, Fjob | Parent education & jobs |
| **Academic** | studytime, failures, absences | Study hours, past failures |
| **Social** | freetime, goout, romantic | Social activities, relationships |
| **Health & Lifestyle** | health, Dalc, Walc | Health status, alcohol consumption |

### Target Variable
- **G3**: Final grade (0-20 scale)

## 🔬 Methodology

### 1. Data Preprocessing
- ✅ No missing values detected
- ✅ Categorical encoding (binary and label encoding)
- ✅ Feature standardization for linear models
- ✅ Train-test split (80-20)

### 2. Model Development
```python
models = {
    'Linear Regression': LinearRegression(),
    'Decision Tree': DecisionTreeRegressor(),
    'Random Forest': RandomForestRegressor()
}
```

### 3. Hyperparameter Optimization
- Grid Search with 3-fold cross-validation
- Optimized parameters for Random Forest and Decision Tree
- Performance validation across multiple random states

### 4. Model Evaluation
- **R² Score**: Variance explained
- **MAE**: Mean Absolute Error
- **RMSE**: Root Mean Square Error
- **Cross-validation**: 5-fold CV for robustness

## 📈 Key Results

### Model Performance

| Subject | Best Model | R² Score | MAE | RMSE |
|---------|------------|----------|-----|------|
| **Mathematics** | Random Forest | 0.184 | 3.36 | 4.09 |
| **Portuguese** | Random Forest | 0.216 | 2.01 | 2.77 |

### 🎯 Top Predictive Features

**Mathematics Performance:**
1. **Absences** (19.4%) - Class attendance
2. **Failures** (14.2%) - Previous academic failures
3. **Health** (5.4%) - Student health status
4. **Going Out** (5.1%) - Social activities frequency
5. **Age** (4.3%) - Student age

**Portuguese Performance:**
1. **Failures** (20.6%) - Previous academic failures
2. **Absences** (7.1%) - Class attendance
3. **School** (5.0%) - School type (GP vs MS)
4. **Father's Education** (5.0%) - Paternal education level
5. **Weekend Alcohol** (4.4%) - Weekend drinking

### 📊 Academic Performance Comparison
- **Portuguese**: Higher average grade (11.91 vs 10.42)
- **Mathematics**: More variable performance (σ = 4.58 vs 3.23)
- **Correlation**: 0.48 between Math and Portuguese grades

## 🎨 Visualizations

The project includes comprehensive visualizations:
- 📊 Grade distribution histograms
- 🔥 Correlation heatmaps
- 📈 Model performance comparisons
- 🎯 Feature importance plots
- 📉 Learning curves
- 🔍 Residual analysis

## 💡 Key Insights

### 🚨 Critical Success Factors
1. **Attendance is King**: Most important factor across both subjects
2. **Early Intervention**: Previous failures strongly predict future performance
3. **Family Matters**: Parental education significantly impacts outcomes
4. **Balance is Key**: Social activities affect academic performance
5. **Health Awareness**: Physical wellbeing influences grades

### 🎓 Educational Implications
- **For Schools**: Implement early warning systems for absences
- **For Students**: Focus on consistent attendance and seek help after failures
- **For Parents**: Engage in educational planning and support

## 🔧 Technical Details

### Dependencies
```
numpy >= 1.21.0
pandas >= 1.3.0
matplotlib >= 3.4.0
seaborn >= 0.11.0
scikit-learn >= 1.0.0
```

### Project Structure
```
student-performance-prediction/
├── data/
│   ├── student-mat.csv
│   └── student-por.csv
├── src/
│   ├── student_Grade_prediction
│   
├── reports file
│   
├── requirements.txt
└── README.md
```

## 📋 Model Limitations

- **Moderate Predictive Power**: 18-22% variance explained
- **Complex Interactions**: Human factors not fully captured
- **Domain Specific**: Results specific to Portuguese educational context
- **Feature Scope**: Limited to available demographic/behavioral variables

## 🔮 Future Enhancements

### Data Collection
- [ ] Learning style assessments
- [ ] Socioeconomic detailed indicators
- [ ] Teacher-student relationship metrics
- [ ] Real-time study behavior tracking

### Advanced Modeling
- [ ] Deep learning approaches (Neural Networks)
- [ ] Time-series analysis for grade progression
- [ ] Ensemble methods combining multiple algorithms
- [ ] Feature interaction modeling

### System Integration
- [ ] Real-time monitoring dashboard
- [ ] Early intervention trigger systems
- [ ] Personalized learning recommendations
- [ ] Mobile app for students and parents

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 📚 References
- UCI Machine Learning Repository: Student Performance Dataset

## 📧 Contact

Your Name - [kottusaikumar@2003](kottusaikumar@2003) - email@example.com

Project Link: [https://github.com/kottusaikumar/Student_Academic_Performance_Prediction-_Project)

---

⭐ **Star this repository if it helped you!** ⭐
