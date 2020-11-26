# Learning Vulnerability Discovery with Global-Relational Models

A promising direction for automatic discovery of vulnerabilities is Machine Learning [1, 2]. 
Early work has shown that ML-Methods are able to perform similarly to static analysis tools using sequence models, such as Recurrent Neural Networks (RNNs) [2]. 
More recent work has shown that graph models, such as Graph Neural Networks (GNNs) operating on a graph source code representation are a better-suited for this task [1, 3]: By forming neural messages and passing them iteratively within the graph structure, task-relevant features of the programs can be learned.

However, compared to sequence models, this information propagation scheme is limited in its reach, resulting in local program features only. To overcome this issue, Hellendoorn et al. [4] combined GNNs with RNNs and Transformers to propagate information in a global scheme, resulting in global program features. This has shown to outperform GNNs and RNNs in Software Engineering tasks, setting a new state-of-the-art. 
To make this model usable and enable further evaluation in compiler and software engineering tasks, it shall be implemented in ComPy-Learn, a framework decoupling representations, models, and tasks [5].
While many ML-Models have been proposed for the task of vulnerability discovery, they don’t generalize
well to non-synthetic programs [3]. The recent advances in GNNs and global-relational models are a
promising step towards discovering real-world vulnerabilities, motivating this research project. Therefore,
a second focus of this project will be the careful selection of a proper dataset.

Therefore, the tasks of this research project are:
1. Review of the existing datasets for automatic vulnerability discovery
2. Implementation of the model of Hellendoorn et al. in the ComPy-Learn framework
3. Evaluation of the model in a real-world vulnerability dataset

### References
[1] Guixin Ye, Zhanyong Tang, Huanting Wang, Dingyi Fang, Jianbin Fang, Songfang Huang, and Zheng Wang. Deep program structure modeling through multi-relational graph-based learning. In Proceedings of the ACM International Conference on Parallel Architectures and Compilation Techniques, pages 111–123, 2020.  
[2] Zhen Li, Deqing Zou, Shouhuai Xu, Xinyu Ou, Hai Jin, Sujuan Wang, Zhijun Deng, and Yuyi Zhong. Vuldeepecker: A deep learning-based system for vulnerability detection. arXiv preprint arXiv:1801.01681, 2018.  
[3] Saikat Chakraborty, Rahul Krishna, Yangruibo Ding, and Baishakhi Ray. Deep learning based vulnerability detection: Are we there yet? arXiv preprint arXiv:2009.07235, 2020.   
[4] Vincent J Hellendoorn, Charles Sutton, Rishabh Singh, Petros Maniatis, and David Bieber. Global relational models of source code. In International Conference on Learning Representations, 2019.  
[5] Alexander Brauckmann, Andr´es Goens, and Jeronimo Castrillon. Compy-learn: A toolbox for exploring machine learning representations for compilers. In 2020 Forum for Specification and Design  

