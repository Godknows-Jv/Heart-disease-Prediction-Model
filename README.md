# CardioRisk Classifier – Machine Learning Modules

This repository serves as a central location for storing and documenting machine learning modules developed as part of the research, design, experimentation, and deployment phases of heart disease risk prediction systems. These systems were built with the goal of assisting healthcare professionals and researchers in identifying potential heart disease risks using trained machine learning models. The repository features two primary modules, each of which played a significant and distinct role in the broader development journey.

## jv-cardio.ai-module

The **jv-cardio.ai-module** is the main and most advanced machine learning module within this repository. It was created specifically for the development of the **JV Cardio AI** system, a full system application designed to perform real-time or batch predictions of heart disease risk levels based on input clinical data. This module represents the final and complete implementation of the AI engine behind JV Cardio AI. It includes core model files, data preprocessing routines, prediction logic, and potentially optimized code for deployment purposes.

Unlike the earlier modules that were used during the prototyping and testing phases, the jv-cardio.ai-module was developed after extensive evaluation of model performance, fine-tuning, and validation. It reflects the culmination of lessons learned from previous experiments and serves as the production-level module powering a practical and standalone application.

This module was built individually and independently from the earlier group work, and it was specifically designed to meet higher standards of performance, usability, and readiness for integration into a final product. It may include components such as trained classifiers, serialization formats like joblib or pickle files, evaluation scripts, and inference interfaces tailored for deployment into user-facing applications.

## project-cardio-risk-classifier-module

The **project-cardio-risk-classifier-module** is the original module developed during a group-based academic project titled *Cardio Risk Classifier*. It served primarily as a prototype for the development and testing of various machine learning models intended for heart disease risk prediction. The module includes experimentation with different model types, feature selection techniques, data cleaning methods, and performance evaluation procedures.

As part of a collaborative project, this module was built during the early phases of research and model exploration. The primary objective was to test the feasibility of using supervised learning techniques for predicting the presence or risk of heart disease using publicly available datasets. At this stage, the focus was on experimentation, gathering insights, understanding data behavior, and comparing various models based on metrics such as accuracy, precision, recall, F1 score, and ROC-AUC.

Although it lacks the polish and finality of the jv-cardio.ai-module, this module remains an important part of the repository. It documents the foundation and research work that influenced the final system. It demonstrates how different approaches were tried, what challenges were encountered, and how initial assumptions and findings shaped the subsequent development of the standalone JV Cardio AI system.

## Purpose of the Repository

This repository is structured to provide a clear historical and technical record of the two major phases in the development of a heart disease prediction system. It contains both the prototype module used for testing and validation purposes and the final AI module used for full system deployment. This makes the repository valuable for developers, collaborators, and reviewers who are interested in understanding the full scope of the development process—from concept to production.

The separation of modules also ensures that users can clearly distinguish between experimental and production-ready code. This documentation can help future contributors, researchers, or evaluators quickly identify which components are suitable for extension, optimization, or deployment, and which are more appropriate for reference or study purposes.

Additional documentation, usage instructions, and deployment guides may be added in the future as development progresses or when the final application is made available for public use. For now, this README provides an overview of the contents and their relevance within the context of machine learning application development in the medical domain.
