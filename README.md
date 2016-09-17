# Asynchronous Multi-Task Learning 

Abstract—Many real-world machine learning applications involve many learning tasks that are inter-related. For example, in the healthcare domain, we need to learn a predictive model of a certain disease for many hospitals. The models for each hospital can be different because of the inherent differences in the distributions of the patient populations. However, the models are also closely related because of the nature of the learning tasks namely modeling the same disease. By simultaneously learning all the tasks, the multi-task learning (MTL) paradigm performs inductive knowledge transfer among tasks to improve the generalization performance of all tasks involved. When datasets for the learning tasks are stored in different locations, it may not always be feasible to move the data to provide a data-centralized computing environment, due to various practical issues such as high data volume and data privacy. This has posed a huge challenge to existing MTL algorithms. In this paper, we propose a principled MTL framework for distributed and asynchronous optimization. In our framework, the gradient update does not depend on and hence does not require waiting for the gradient information to be collected from all the tasks, making it especially attractive when the communication delay is too high for some task nodes. We show that many regularized MTL formulations can benefit from this framework, including the low-rank MTL for shared subspace learning. Empirical studies on both synthetic and real-world datasets demonstrate the efficiency and effectiveness of the proposed framework.
