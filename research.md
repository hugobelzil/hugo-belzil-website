---
title: Research
permalink: /research/
wide: true
---

<div class="research-intro">
  <p>
    During the summer 2025, I had the chance to be an undergraduate researcher in the mathematics and statistics department of McGill, under <a href="https://www.math.mcgill.ca/neslehova/">Dr. Johanna Nešlehová</a> and Dr. Nicolas Lafon.
  </p>
  <p>
    Our research investigated how to generate heavy-tailed data in high dimensions carrying a structure dependence and different tail indices. This turns out to be a challenging problem as dimensions get larger than 5 or 10.
  </p>
  <p>
    Several generative techniques have been proposed in the literature, using different tools such as generative adversarial networks (<a href="https://inria.hal.science/hal-04416809v1/file/Simulation-extreme-neural-networks-HAL.pdf"><em>Allouche, Girard and Gobet, 2024</em></a>) or variational autoencoders (see <a href="https://arxiv.org/pdf/2306.10987"><em>Lafon, Naveau and Fablet, 2023</em></a>). In particular, our approach was to use and experiment with variational autoencoders, as done in this last paper. However, we proposed to tackle this problem by trying to make our adapted VAEs learn the copula distribution of the data instead, allowing us to reconstruct the data using the marginal densities.
  </p>
  <p>
    This work is still ongoing at INRAE in France by Dr. Lafon.
  </p>
</div>

<section class="research-feature" aria-label="Variational autoencoder method">
  <figure>
    <img src="{{ '/assets/img/vae.png' | relative_url }}" alt="Architecture of the variational autoencoder used in the research" loading="lazy">
  </figure>
  <div>
    <p><em><a href="https://en.wikipedia.org/wiki/Variational_autoencoder">Variational autoencoders</a> are neural networks which are able to learn parametric distributions in a latent space in order to sample from this latent space, and thus generate new data. The objective of the network is therefore a likelihood function.</em></p>
    <p><em>We implemented the VAEs using TensorFlow.</em></p>
  </div>
</section>

<hr class="research-divider">

<section class="research-feature research-feature--result" aria-label="Learned copula result">
  <div>
    <p>
      Here is an example of a five-dimensional copula learned by a VAE, where the training data originated from a Hüsler–Reiss copula. These results were achieved by experimenting with the distribution in the latent space and applying an appropriate transform to the output of the VAE.
    </p>
  </div>
  <figure>
    <img src="{{ '/assets/img/learned-copulas.png' | relative_url }}" alt="Pairwise scatterplots from a five-dimensional copula learned by a variational autoencoder" loading="lazy">
  </figure>
</section>
