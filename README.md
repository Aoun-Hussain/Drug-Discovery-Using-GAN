# Drug-Discovery-Using-GAN

The model implements deep learning and reinforcement learning approaches. It integrates two different deep neural networks - generator and discriminator with reinforcement learning. These two models are trained separately but are used jointly to generate novel targeted chemical libraries.

The model uses string representation of molecules by their simplified molecule-input line entry-system (SMILES). In this system, the generative model is used to produce novel chemically feasible molecules, that is, it plays a role of an agent, whereas the discriminative model (that predicts the properties of novel compounds) plays the role of a critic, which estimates the agent’s behavior by assigning a numerical reward (or penalty) to every generated molecule.

The reward is a function of the numerical property generated by the predictive model, and the generative model is trained to maximize the expected reward. In the first phase of the method, generative and discriminator models are trained separately with a supervised learning algorithm. In the second phase, both models are trained jointly with the RL approach to bias the generation of new chemical structures toward those with the desired physical and/or biological properties.

We have used GAN model integrated with RL to design chemical molecules with specific range of physical properties, such as solubility, novelty, synthesizability.
