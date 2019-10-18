# Machine learning/deep learning in molecular dynamics

A repository of update in molecular dynamics field by recent progress in machine learning and deep learning. Those efforts are cast into the following categories: 
1. Learn force field or molecular interactions;  
2. Enhanced sampling methods;
3. Learn collective variable to bias enhanced sampling;  
4. Capture dynamics of molecular system; 
5. Map between all atoms and coarse grain;


&nbsp;  

<img src="https://pubs.rsc.org/en/Content/Image/GA/C7SC02267K" align="center" alt="Machine learning molecular dynamics for the simulation of infrared spectra">
(Picture from Machine learning molecular dynamics for the simulation of infrared spectra. )
&nbsp;  


### 1. Learn force field or molecular interactions  
[ANI-1: an extensible neural network potential with DFT accuracy at force field computational cost](https://doi.org/10.1039/c6sc05720a)   
J. S. Smith, Isayev, A. E. Roitberg. (2017)   
This paper from Univ. of Florida and Univ. of North Carolina presented ANI-1, which used Behler and Parrinello symmetry functions to build single-atom atomic environment vectors (AEV) as molecular representation. This is similar to the context representation of work in NLP.  

[Neural Message Passing with Edge Updates for Predicting Properties of Molecules and Materials](https://arxiv.org/abs/1806.03146)   
Peter Bjørn Jørgensen, Karsten Wedel Jacobsen, Mikkel N. Schmidt. (2018)   
This paper from Univ. of Denmark extended neural message passing model with an edge update NN, so that information exchanges between atoms depend on hidden state of the receiving atom. They also explored ways to construct the graph. 

[SchNet – A deep learning architecture for molecules and materials](https://aip.scitation.org/doi/10.1063/1.5019779)    
K. T. Schütt, H. E. Sauceda, P.-J. Kindermans, A. Tkatchenko, K.-R. Müller. (2018)   
This paper from Technische Universita ̈t Berlin, Univ. of Luxembourg, Max Planck Institute, and Korea University presented SchNet, a variant of DTNN to learn the molecular properties and studied local chemical potential and the dynamics of C20-fullerene.  

[Message-passing neural networks for high-throughput polymer screening](https://aip.scitation.org/doi/10.1063/1.5099132)  
Peter C. St. John1, Caleb Phillips, Travis W. Kemper, A. Nolan Wilson, Yanfei Guan,  Michael F. Crowley, Mark R. Nimlos, Ross E. Larsen. (2019)  
This paper from National Renewable Energy Lab, USA, used message-passing NN to predict polymer properties for screening purpose. They focused on larger molecules and tested the model with/without 3D conformation information, since accurate 3D structure calculation is also expensive. 

[Accurate and transferable multitask prediction of chemical properties with an atoms-in-molecules neural network](https://advances.sciencemag.org/content/5/8/eaav6490)   
Roman Zubatyuk, Justin S. Smith, Jerzy Leszczynski and Olexandr Isayev. (2019)   
This paper from Univ. of North Carolina, Los Alamos National Lab, and Jackson State Univ presented AIMNet to leearn implicit solvation energy in MNSol database. Atoms in molecules are embedded and interact with each in several layers. 

### 4. Capture the dynamics of the molecular system 

[Equivariant Hamiltonian Flows](https://arxiv.org/abs/1909.13739)   
Danilo Jimenez Rezende, Sébastien Racanière, Irina Higgins, Peter Toth.  
This paper from Google uses Lie algebra to prove what hamiltonian flow learns and how addition of symmetry invariance constraints can improve data efficiency. 

[Symplectic ODE-NET: learning Hamiltonian dynamics with control](https://arxiv.org/abs/1909.12077)    
Yaofeng Desmond Zhong, Biswadip Dey, Amit Chakraborty.    
This paper from Princeton University and Siemens Corp infers the dynamics of a physical system from observed state trajectories. They embedded high dimensional coordinates into low dimensions and velocity into general momentum. 

[Hamiltonian Neural Networks](https://arxiv.org/abs/1906.01563)   
Sam Greydanus, Misko Dzamba, Jason Yosinski.    
This paper from Google, PetCube and Uber trains models to learn conservation law of Hamiltonian in unsupervised way.  


[Symplectic Recurrent Neural Networks](https://arxiv.org/abs/1909.13334)   
Zhengdao Chen, Jianyu Zhang, Martin Arjovsky, Léon Bottou.   
The authors from NYU, Tianjin University, and Facebook proposes SRNN to capture the dynamics of physical systems from observed trajectories.  

[Physical Symmetries Embedded in Neural Networks](https://arxiv.org/abs/1904.08991)   
M. Mattheakis, P. Protopapas, D. Sondak, M. Di Giovanni, E. Kaxiras.   
The authors from Harvard and Polytechnic Milan used symplectic neural network to embed physics symmetry in the neural network to characterize the dynamics. 

