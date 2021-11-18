

# latent-is-all-you-need

Inspired from [@hwalsuklee](https://github.com/hwalsuklee/tensorflow-mnist-VAE) github repository and [video](https://www.youtube.com/watch?v=o_peo6U7IRM), this presents the investigation/reimplementation of VAE/CVAE with different latent space size.

#### **Dataset**

* MNIST
* CIFAR10 (#TODO)

#### **Framework**

* Pytorch + wandb



## Results

|      | Input                             | latent_dim=2                | latent_dim=5                | latent_dim=10                 | latent_dim=20                 |
| ---- | --------------------------------- | --------------------------- | --------------------------- | ----------------------------- | ----------------------------- |
| VAE  | ![input](vae/input.png?raw=true)  | ![2d](vae/2d.png?raw=true)  | ![5d](vae/5d.png?raw=true)  | ![10d](vae/10d.png?raw=true)  | ![20d](vae/20d.png?raw=true)  |
| CAVE | ![input](cvae/input.png?raw=true) | ![2d](cvae/2d.png?raw=true) | ![5d](cvae/5d.png?raw=true) | ![10d](cvae/10d.png?raw=true) | ![20d](cvae/20d.png?raw=true) |



|          | Manifold / Conditional Generation           | Distribution                            |
| -------- | ------------------------------------------- | --------------------------------------- |
| **VAE**  | ![vaewalk](vae/vaewalk.png?raw=true)        | ![manifold](vae/manifold.png?raw=true)  |
| **CVAE** | ![cond_style](cvae/cond_style.jpg?raw=true) | ![manifold](cvae/manifold.png?raw=true) |

| Video    | VAE                                                          | CVAE                                                         |
| -------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Manifold | <img src="vae/manifold.gif?raw=true" alt="manifold" style="zoom:150%;" /> | <img src="cvae/manifold.gif?raw=true" alt="manifold" style="zoom:150%;" /> |

Below result shows CVAE result of fixed latent space vector z, but with different condition (0-9 for MNIST)

| ![vaewalk_0](cvae/condition/vaewalk_0.jpg?raw=true) | ![vaewalk_1](cvae/condition/vaewalk_1.jpg?raw=true) |
| --------------------------------------------------- | --------------------------------------------------- |
| ![vaewalk_2](cvae/condition/vaewalk_2.jpg?raw=true) | ![vaewalk_3](cvae/condition/vaewalk_3.jpg?raw=true) |
| ![vaewalk_4](cvae/condition/vaewalk_4.jpg?raw=true) | ![vaewalk_5](cvae/condition/vaewalk_5.jpg?raw=true) |
| ![vaewalk_6](cvae/condition/vaewalk_6.jpg?raw=true) | ![vaewalk_7](cvae/condition/vaewalk_7.jpg?raw=true) |
| ![vaewalk_8](cvae/condition/vaewalk_8.jpg?raw=true) | ![vaewalk_9](cvae/condition/vaewalk_9.jpg?raw=true) |

