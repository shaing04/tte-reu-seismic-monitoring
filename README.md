# Seismic Phase Picking Automation Using An Implicit Deep Learning Model

The project is to explore the idea of using the state-driven implicit modeling framework and SAFE feature elimination technique to shrink large deep learning models down to a deployable size for edge devices (e.g. RasberryShake). The goal was to train on an implicit model and Seisbench's ETHZ dataset to apply the SAFE feature elimination technique developed for implicit models. 

### Background 
Many state-of-the-art deep learning models require powerful hardware in the form of servers with multiple GPUs. However, not everyone has access to these, especially given the limited computing power of mobile or edge devices. Hence, liberating deep learning from such static servers has plenty of benefits. The current project will explore this idea with the EQTransformer model [1], a deep-learning-based earthquake signal detection and seismic phase picking model, and RaspberryShake, a professional-grade seismograph and infrasound monitor that is low-cost and open-sourced. The successful implementation of compact deep neural network models on RaspberryShake devices will facilitate a wide range of applications, encompassing urban environmental monitoring, earthquake early warning systems, scientific educational outreach, and event monitoring in developing countries such as Haiti, where costly seismographs and monitors are often out of reach for local communities [2].
Specifically, we consider using the implicit model with the state-driven approach [3]. Implicit models are capable of capturing any type of classical feedforward-based neural network. With the state-driven approach, the baseline model can be transformed into an implicit model without expensive re-training. Various compression techniques such as can be imposed on the training problem to compress the model down to the desired size. In this project, we consider applying the SAFE feature elimination [4] technique to the implicit model and the earthquake dataset. 

[1] Mousavi, S.M., Ellsworth, W.L., Zhu, W. et al. “Earthquake transformer—an attentive deep-learning model for simultaneous earthquake detection and phase picking”. Nat Commun 11, 3952 (2020).

[2] Calais, E., 2022, “Haiti earthquake captured by citizen-seismologists”. Temblor (2022), http://doi.org/10.32858/temblor.245

[3] Tsai, Alicia Y., et al. "State-driven implicit modeling for sparsity and robustness in neural networks." arXiv preprint arXiv:2209.09389 (2022).

[4] Ghaoui, Laurent El, Vivian Viallon, and Tarek Rabbani. "Safe feature elimination for the lasso and sparse supervised learning problems." arXiv preprint arXiv:1009.4219 (2010).

