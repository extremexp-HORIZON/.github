
# ExtremeXP Project
The ExtremeXP project aims to support the development and operation of complex analytics workflows that are used for taking data-driven decisions in different application domains. By addressing the need for accurate, precise, fit-for-purpose, and trustworthy data-driven insights, ExtremeXP proposes a experimentation-driven analytics paradigm, which puts the end user at the centre of complex analytics processes. In this context the user can set their requirements, preferences, and constraints early in the experimentation process and/or ask for explanations and feedback, accounting for novel interactions with the system.

## Key Concepts in ExtremeXP framework

1. **Complex Analytics Workwflow (CAW)**: is an abstraction over different types of data-driven analytics workflows that includes (possibly combinations of):
  - machine learning (ML) lifecycle workflows,
  - job scheduling and task automation workflows,
  - data-analysis scripts,
  - ETL pipelines
  - etc.   
2.  **Intent**: is a specification of the result (functional requirement) of the CAW, in the form of a natural language prompt, e.g., “find a classifier with at least 90% accuracy on this test dataset”. It may further contain non-functional requirements, e.g., “the computation should not take too much CPU/GPU resources”.
4.  **Experiment**: Experiments are used within ExtremeXP to systematically develop, automate, reuse, setup, execute, track, explain, compare, and optimize CAWs. For simplicity, we refer to this henceforth as just “experiment”.
5.  **Experiment Specification** includes: 
- **description of the CAW itself**, i.e. tasks to be performed and their data and control dependencies.
-  Any **variability points**. A variability point is an aspect of the CAW that can be changed and can refer to (i) different task implementations (e.g., different ML algorithms), (ii) different task inputs (e.g., different datasets), (iii) different hyperparameters, (iv) different task/workflow deployments (e.g., on CPUs/GPUs).
-   **Metrics** to be computed. A metric refers to a measurable property (i) of the whole CAW (e.g., end-to-end execution time), (ii) of a particular task (e.g., memory consumption of ML training), or (iii) of an output of a task (e.g., accuracy of produced ML model, user satisfaction level given a task’s outcome).
-  Any **soft and hard constraints** related to the execution of the CAW. A hard constraint should never be violated (e.g., memory consumed below a certain limit), while a soft constraint is essentially an optimization objective (e.g., minimize memory consumption). A constraint can be defined with reference to e.g., a metric and/or deployment option.
       
## User Roles in ExtremeXP
- **Data engineer**: runs one or more experiments to develop optimized and trustworthy CAWs. Data engineers realize the requirements of domain experts by specifying experiments, specifying access control processes, and controlling the execution of experiments.
- **Domain expert**: Provides the requirements for the experiments to be specified and run (e.g. which CAW workflow to be optimized, which metrics to use in doing so), consumes the results of the CAW (including the visualization and explainability ones), needs to trust the experimentation process followed by the framework.
- **Data creator**: Provides the datasets acting as inputs to the CAWs involved in the experiments; has certain privacy and confidentiality requirements that need to be preserved during the experimentation process. 

## ExtremeXP Framework Architecture

**_TO BE UPDATED AFTER FINAL ARCHITECTURE IS RELEASED_**

<img width="1367" height="865" alt="Image" src="https://github.com/user-attachments/assets/2e0a0197-f6f0-4a01-8d6d-8eaa60fc3401" />

## Main Repositories

- **ExtremeXP Portal**: https://github.com/extremexp-HORIZON/extremexp-portal
  
- **DSL Editor**:  https://github.com/extremexp-HORIZON/extremexp-ide

- **Experimentation Engine**: https://github.com/extremexp-HORIZON/extremexp-experimentation-engine

- **Decentralized Data Management**: https://github.com/extremexp-HORIZON/DDM
  
- **ProActive Executionware/Scheduler**: https://github.com/eu-nebulous/nebulous/wiki/1.1-Installation-Walk%E2%80%90trough-for-Development-&-Evaluation#proactive-scheduler 
   
- **Visualization Dashboard**: https://github.com/extremexp-HORIZON/experiment-lens

- **Access Control**: 

- **Analytics Catalogue**

- **Intent Capture and Anticipation Module**: https://github.com/extremexp-HORIZON/extremexp-intents2workflows 




## Getting Started 
1. **Register and Login in the ExtremeXP Portal**: Go to [ExtremeXP Portal](https://portal.extremexp-icom.intracom-telecom.com	), and
     - Register a new user
     - Log in with your credentials

The ExtremeXP portal acts as the main entry point for all ExtremeXP users. A registered user of the Portal can access both a Graphical (Experiments tab) and the Textual Editors (Tasks tab - aka DSL Editor) to design and specify workflows and experiments.

2. **Specify Workflows and Experiments**
There are two ways to specify a workflow; either via the Graphical Editor or the DSL Editor

    2.1 **Graphical Editor**: 


   2.2 **DSL Editor**: Go to https://ide.extremexp-icom.intracom-telecom.com/  

 
   
   

4. **Data Upload and Exploration via the Decentralized Data Management**
The user can access the Decentralized Data Management (DDM) system via https://ddm.extremexp-icom.intracom-telecom.com/.
DDM provides a robust framework for handling heterogeneous data and metadata assets across the project’s distributed modules. Designed to support varying storage and access requirements among machines operating in diverse geographic and operational environments, the system ensures scalable, low-latency data handling through a decentralized architecture built on Zenoh.


5. **Experimentation Engine** : 
   
6. **Experiment Execution via Proactive**: https://proactive.extremexp-icom.intracom-telecom.com 
  
7. **Experiment and Workflow Visualization**
Via the Visualization Dashboard, ExtremeXP users can monitor experiment progress, analyze workflow metrics and results, and compare workflows. ​The Vizualization Dashboard also facilitates human-in-the-loop interaction by enabling experiment lifecycle control, user rating of workflows, and experiment execution adjustments.






