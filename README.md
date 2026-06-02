# Student Dropout Prediction Analysis

Developed by Maia Munich. For questions, reach out via maia.munich@gmail.com

Can we predict which college students are at risk of dropping out, before it's too late? This project applies machine learning to academic, demographic, and financial data from 4,424 students to identify at-risk populations and inform early intervention strategies.

## Project Overview

This project presents a comprehensive analysis of student dropout prediction using machine learning techniques. The analysis aims to identify key factors that influence student retention and academic success in higher education institutions, providing actionable insights for educational policy and intervention strategies.

## 🎯 Objectives

### Primary Goals
- **Predictive Modeling**: Develop accurate models to identify students at risk of dropping out
- **Risk Factor Identification**: Identify key demographic, academic, and socioeconomic factors affecting student success
- **Intervention Strategy**: Provide data-driven recommendations for student retention programs

### Secondary Goals
- **Performance Comparison**: Evaluate multiple machine learning algorithms for optimal prediction accuracy
- **Feature Engineering**: Create meaningful features from raw data for improved model performance
- **Statistical Analysis**: Provide comprehensive statistical insights into student success patterns

## 📊 Dataset Description

### Data Source
- **Institution**: Higher education academic records
- **Sample Size**: 4,424 student records
- **Time Period**: Multi-year academic data
- **Geographic Scope**: International student population

### Key Features
- **Demographics**: Age, gender, nationality, marital status
- **Academic Background**: Previous qualifications, admission grades, course selection
- **Family Background**: Parental education and occupation
- **Financial Factors**: Scholarship status, debt status, tuition payments
- **Academic Performance**: Semester grades, attendance, curricular units
- **Target Variable**: Student outcome (Dropout, Enrolled, Graduate)

## 🏗️ Project Structure

```
CISC4631_Final/
├── README.md                                    # Project documentation
├── data.csv                                     # Original dataset
├── cleaned_data.csv                            # Preprocessed data
├── engineered_data.csv                         # Feature-engineered data
├── Studentdropoutandacademicsuccess.ipynb      # Main analysis notebook
├── attribute_analysis.ipynb                    # Detailed attribute analysis
├── Enchanced_data_looking.ipynb                # Enhanced visualizations
├── attribute_characteristics.txt               # Attribute documentation
├── code_flow_diagram.txt                       # Project workflow
└── Results/
    ├── feature_importance_comparison.csv       # Feature importance results
    ├── feature_selection_results.csv           # Feature selection outcomes
    └── selected_features_analysis.csv          # Selected features analysis
```

## 🔬 Methodology

### 1. Data Preprocessing
- **Data Cleaning**: Handle missing values, outliers, and data inconsistencies
- **Feature Engineering**: Create derived features and transformations
- **Data Filtering**: Remove nationalities with insufficient sample sizes (<5 students)
- **Encoding**: Convert categorical variables for machine learning algorithms

### 2. Exploratory Data Analysis
- **Descriptive Statistics**: Comprehensive statistical summaries
- **Visualization**: Charts and graphs for pattern identification
- **Correlation Analysis**: Identify relationships between features
- **Distribution Analysis**: Examine data distributions and outliers

### 3. Feature Selection and Engineering
- **Statistical Methods**: ANOVA F-tests for feature importance
- **Tree-based Methods**: Random Forest feature importance
- **Domain Knowledge**: Educational theory-driven feature creation
- **Dimensionality Reduction**: Select optimal feature subsets

### 4. Machine Learning Models
- **Gaussian Naive Bayes**: Baseline probabilistic classifier
- **Random Forest**: Ensemble method for robust predictions
- **XGBoost**: Gradient boosting for high-performance predictions
- **Cross-Validation**: 5-fold stratified cross-validation for robust evaluation

### 5. Model Evaluation
- **Performance Metrics**: Accuracy, precision, recall, F1-score
- **Confusion Matrices**: Detailed classification performance analysis
- **ROC Analysis**: Receiver Operating Characteristic curves
- **Cross-Validation**: Robust performance estimation

## 📈 Key Findings

### Academic Performance Patterns
- **Grade Progression**: Students who maintain or improve grades between semesters show higher success rates
- **Admission Grades**: Higher admission grades correlate with better outcomes
- **Course Load**: Appropriate curricular unit loads impact success rates

### Demographic Insights
- **Nationality Impact**: Certain nationalities show different dropout patterns
- **Age Factors**: Non-traditional students (older) may face different challenges
- **Gender Patterns**: Gender-based performance differences identified

### Financial Factors
- **Scholarship Impact**: Scholarship recipients show different success patterns
- **Debt Status**: Students with financial obligations face higher dropout risks
- **Payment Status**: Tuition payment patterns correlate with academic outcomes

### Family Background
- **Parental Education**: Parental education levels influence student success
- **Socioeconomic Status**: Family background impacts academic performance

## 🛠️ Technical Implementation

### Libraries Used
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: scikit-learn, xgboost
- **Statistical Analysis**: scipy, statsmodels

### Model Performance
- **Best Performing Model**: Random Forest (67.7% accuracy)
- **Cross-Validation Score**: 68.4% mean accuracy
- **Feature Importance**: Academic performance metrics are strongest predictors

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost
```

### Running the Analysis
1. **Main Analysis**: Execute `Studentdropoutandacademicsuccess.ipynb`
2. **Attribute Analysis**: Run `attribute_analysis.ipynb` for detailed feature examination
3. **Enhanced Visualizations**: Use `Enchanced_data_looking.ipynb` for advanced charts

### Data Requirements
- Ensure `data.csv` is in the project directory
- Data should be semicolon-separated format
- Required columns: All demographic, academic, and outcome variables

## 📊 Results and Interpretations

### Model Performance Summary
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Gaussian Naive Bayes | 65.5% | 49.0% | 52.0% | 49.0% |
| Random Forest | 67.7% | 57.1% | 66.0% | 59.0% |
| XGBoost | N/A | N/A | N/A | N/A |

### Feature Importance Rankings
1. **Curricular units 2nd sem (grade)** - 33.8% importance
2. **Curricular units 1st sem (grade)** - 24.4% importance
3. **Course** - 14.0% importance
4. **Father's qualification** - 8.8% importance
5. **Mother's qualification** - 8.6% importance

## 🎓 Academic Applications

### For Educational Institutions
- **Early Warning Systems**: Implement predictive models for at-risk student identification
- **Intervention Programs**: Target specific demographic and academic risk factors
- **Resource Allocation**: Focus support services on high-risk student populations
- **Policy Development**: Use data insights for retention policy formulation

### For Students
- **Self-Assessment**: Students can understand factors affecting their success
- **Academic Planning**: Better course selection and academic planning
- **Support Seeking**: Early identification of need for academic support

## 🔮 Future Enhancements

### Model Improvements
- **Deep Learning**: Implement neural networks for complex pattern recognition
- **Ensemble Methods**: Combine multiple models for improved accuracy
- **Time Series Analysis**: Incorporate temporal patterns in academic performance
- **Real-time Prediction**: Develop systems for continuous risk assessment

### Data Enhancements
- **Additional Features**: Include more demographic and academic variables
- **Longitudinal Data**: Track students across multiple semesters
- **External Data**: Incorporate economic and social factors
- **Behavioral Data**: Include student engagement and activity metrics

## 📚 References and Methodology

### Educational Theory
- Tinto's Student Integration Model
- Astin's Theory of Student Involvement
- Bean and Metzner's Nontraditional Student Model

### Statistical Methods
- Cross-validation for robust model evaluation
- Feature importance analysis using multiple techniques
- Confusion matrix analysis for detailed performance assessment
- ROC curve analysis for threshold optimization


**Note**: This analysis provides insights for educational research and policy development. All findings should be interpreted within the context of the specific institution and student population studied.
