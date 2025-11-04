
# ExtremeXP Project
The ExtremeXP project aims to support the development and operation of complex analytics workflows that are used for taking data-driven decisions in different application domains. By addressing the need for accurate, precise, fit-for-purpose, and trustworthy data-driven insights, ExtremeXP proposes a experimentation-driven analytics paradigm, which puts the end user at the centre of complex analytics processes. In this context the user can set their requirements, preferences, and constraints early in the experimentation process and/or ask for explanations and feedback, accounting for novel interactions with the system.

## Key Concepts in ExtremeXP framework

1. **Complex Analytics Workwflow (CAw)**: is an abstraction over different types of data-driven analytics workflows that includes (possibly combinations of):
  - machine learning (ML) lifecycle workflows,
  - job scheduling and task automation workflows,
  - data-analysis scripts
  - ETL pipelines
  - etc.   
2.  **Intent**: is a specification of the result (functional requirement) of the CAW, in the form of a natural language prompt, e.g., “find a classifier with at least 90% accuracy on this test dataset”. It may further contain non-functional requirements, e.g., “the computation should not take too much CPU/GPU resources”.
4.  **Experiment**: Experiments are used within ExtremeXP to systematically develop, automate, reuse, setup, execute, track, explain, compare, and optimize CAWs. For simplicity, we refer to this henceforth as just “experiment”.
5.  **Experiment Specification**. This includes
  - **description of the CAW itself**, i.e. tasks to be performed and their data and control dependencies.
  - Any **variability points**. A variability point is an aspect of the CAW that can be changed and can refer to (i) different task implementations (e.g., different ML algorithms), (ii) different task inputs (e.g., different datasets), (iii) different hyperparameters, (iv) different task/workflow deployments (e.g., on CPUs/GPUs). 
  -	**Metrics** to be computed. A metric refers to a measurable property (i) of the whole CAW (e.g., end-to-end execution time), (ii) of a particular task (e.g., memory consumption of ML training), or (iii) of an output of a task (e.g., accuracy of produced ML model, user satisfaction level given a task’s outcome).
  -	Any **soft and hard constraints** related to the execution of the CAW. A hard constraint should never be violated (e.g., memory consumed below a certain limit), while a soft constraint is essentially an optimization objective (e.g., minimize memory consumption). A constraint can be defined with reference to e.g., a metric and/or deployment option.






