---
marp: true
math: katex
theme: gaia
paginate: true
backgroundColor: #222
color: white
footer: "SMLab Talks | T, Shithij. | The Genomic Code | Sep 9, 2024"  # CHANGEME: ShortNames, dates
size: 16:9 # (16:9, 4:3 etc.)
style: |
  :root {
    font-size: 27px;
    font-family: Kreon, sans-serif;
    line-height: 1.3; /* NOTE: This vertically spaces the text */
    letter-spacing: 1.2px; /* NOTE: This spaces the letters */
  }
  /* Heading Color */
  h1, h3, h2 {
    color: tan;
  }
  /* Link Color */
  a {
    color: #d9b3ff; 
  }
  /* Styles for the Presenter and Lab names */
  .presenter-name {
    text-align: center;
    font-size: 40px;
    color: #e8c583;
  }
  .lab-name {
    text-align: center;
    font-size: 30px;
    color: #4ed092;
  }
  /* List Color */
  p {
    text-align: justify; 
  }
  /* Footer */
  footer {
    font-size: 20px;
    color: #d9b36f;
  }
  /* Pagination */
  section::after {
    content: attr(data-marpit-pagination) '/' attr(data-marpit-pagination-total);
    color: #d9b36f;
  }
  /* CHANGEME: Add more CSS styles here as needed */

---

<!-- NOTE: LEAVE THIS SLIDE AS-IS -->
<!-- _class: lead -->
<!-- _footer: '' -->
<!-- _paginate: false -->
<!-- _backgroundColor: #000 -->
<!-- _backgroundImage: url('./media/slide_bg_dark.png') -->
<!-- NOTE: `scoped` is used to limit the styles to the current slide -->
<style scoped>
  h1 {
    margin-top: 75px;
    font-size: 70px;
    color: #4ed092;
  }
  .socials {
    margin-top: 30px;
    width: 100%;
    text-align: center;
    vertical-align: middle;
    color: red;
  }
  .socials a {
    text-align: center;
  }
  .socials a img {
    width: 60px;
    height: 60px;
  }
  .logos {
    margin-top: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    text-align: center;
  }
  .logos img {
    width: 200px;
    height: 200px;
    background: white;
    border-radius: 50%;
  }
  a {
    margin: 15px;
    font-size: 40px;
    color: #fff;
    text-decoration: none;
  }
</style>

<!-- Title -->
<h1> Subhankar Mishra Lab Weekly Talks </h1>

<!-- Socials -->
<span class="socials">
<!-- Lab-talks website -->
  <a href="https://smlab.niser.ac.in/labtalks/" target="_blank">
    <img src="./media/web.png" alt="Website">
  </a>
  <!-- Lab-talks GitHub -->
  <a href="https://github.com/JeS24/smlab-talks/" target="_blank">
    <img src="./media/gh.svg" alt="GitHub">
  </a>
  <!-- Lab Twitter -->
  <a href="https://twitter.com/mishra_lab" target="_blank">
    <img src="./media/twitter.svg" alt="Twitter">
  </a>
  <!-- Lab public email -->
  <a href="mailto:smlab@niser.ac.in">
    <img src="./media/email.png" alt="Mail">
  </a>
</span>

<!-- Logos -->
<span class="logos">
  <img src="./media/dae_logo.svg" alt="DAE">
  <img src="./media/hbni_logo.png" alt="HBNI">
  <img src="./media/niser_logo_blue.svg" alt="NISER">
  <img src="./media/smlab_logo.svg" alt="SMLab">
</span>

---
<!-- NOTE: A `_` prefix is used to change properties for only the current slide -->

<!-- _class: lead -->
<!-- _footer: '' -->
<!-- _paginate: false -->
<!-- _backgroundColor: #000 -->
<!-- _backgroundImage: url('./media/slide_bg_dark.png') -->
<!-- ![bg right:60% w:75% opacity:55%](./media/bg2.png) -->
<!-- NOTE: Multiple images added here - one in BG, one in FG -->
<!-- 
# **Title Slide Variation 1**

<p class="presenter-name">
  Shithij
</p>
<p class="lab-name">
  Subhankar Mishra Lab<br>
  Sep , 2024
</p>

--- -->
<!-- NOTE: Another example of title slide -->

<!-- _class: lead -->
<!-- _footer: '' -->
<!-- _paginate: false -->
<!-- _backgroundColor: #000 -->
<!-- _backgroundImage: url('./media/slide_bg_dark.png') -->
![bg w:60% opacity:20%](./media/bg2.png)  

# **The Genomic Code**
## The genome instantiates a generative model of the organism

<p class="presenter-name">
  Shithij T
</p>
<p class="lab-name">
  Subhankar Mishra Lab<br>
  Sep 9, 2024
</p>

---

# What is Genomic Code

We usually use some metaphors for capturing the notion of genomic code: 

- Blueprint
- Program
- Recipe
- Resource

---

# What is Genomic Code

The current metaphors fail to provide any insights on these crucial questions:

- How does information get encoded in the genome and what is this information about?
- What is the “data format” of this information in the genome?
- How does such information get decoded through the processes of development?
- How does genotypic variation relate to phenotypic variation?
- How does the genetic architecture of various traits arise?
- How do the underlying encodings evolve through time?

---

# Generative model

![bg right:45% w:90%](https://theaisummer.com/static/25f603171034d2fc8f6a518b8537f85a/ee604/vae.png)

The genome instantiates a generative model of the organism

- An encoding of latent variables
- A mean of decoding them


---

# Generative model

<style scoped>
  img {
    border-radius: 50px;
  }
</style>

![w:1000 h:450 opacity:1.0](media/GenomeGenerativeModel.png)

---

# The Latent Variable

The latent variable of the genome are the the DNA nucleotides themselves, which, over sequences of varying length: 

- Encode RNA and protein molecules that do the work in the cellular economy, including the regulation of gene expression
- Comprise binding sites for regulatory factors

With respect to the form of the organism, these variables are “latent” because the relationship of the genomic sequence to the form of the organism is distributed, non-linear, and extremely indirect.

---

# The Decoder

- The cells of the developing embryo take the compressed information encoded in the genome and use it to build a fully formed organism.

- Unlike the regular machine learning models, these models have to build their own decoders along the way.

![bg right:45% bottom:70% w:90%](./media/Development.png)

---

# The Decoder

- Initial Conditions
- Cell differentiation and division
- Temporal and Spatial Coordination
- Self Organisation

---

# Initial Condition

- The genetic code is packaged into chromatin, making some part of it inaccessible (Changes the landscape of latent variable)
- Zygote inherits some nuclear, cytoplasmic and membrane proteins - the elements that actively do the decoding

---

# Cell division and differentiation

- With each division, the initial conditions and the configuration of the decoder change.
- This determines which elements of the generative model will be active in any newly generated cell, allowing the decoder to generate the appropriate cell type.

![bg right height:90%](./media/Differentiation.png)

---

# Spatial and Temporal Coordination

- All the cellular differentiation has to be spatially and temporally coordinated.
- Generative model encoded in the genome must also direct processes like proliferation, differentiation, cell signaling, and morphogenetic movements to ensure the emergence of the three-dimensional form of the organism.

---

# Self-Organisation

- While the genome provides a set of constraints, it does not encode all the physical parameters and self-organizing dynamics required for development.
- The genome only needs to encode constraints that channel these processes along specific trajectories

![bg right height:85%](./media/ProteinFolding.png)

---

# Gene Regulatory Network

<style scoped>
  img {
    border-radius: 50px;
  }
</style>

<!-- NOTE: Setting a background image of a particular width and height -->
![w:800 h:500 opacity:1.0](./media/GRN.png)

---

# Gene Regulatory Network

- Gene regulatory networks are complex systems where genes interact with each other to control various biological processes, particularly development.

- These networks can be understood as graphs where genes are nodes, and the edges represent the regulatory interactions between them, either activating or repressing each other

- The regulatory elements of a gene can be seen as performing logical operations based on the signals received from other regulators.

- However, unlike simple logic gates, genes operate in a more graded, probabilistic, and dynamic fashion within this interconnected network.

---

# Attractor States

- Attractor states emerge from the dynamic nature of gene regulatory networks.

- Instead of settling into a single static state, these networks can tend towards multiple stable states called attractor states.

- Visualize this as a ball rolling down a bumpy hill, eventually settling into one of several valleys. Each valley represents a stable attractor state

![bg right:45% width:90%](./media/Attractor.png)

---

# Energy Landscapes

- Waddington's epigenetic landscape is a foundational concept in developmental biology
- He represented cells as balls traversing this landscape during development.
- The landscape itself, with its valleys and ridges, is shaped by the collective influence of the genome, influencing which cell fates are more likely

<!-- NOTE: Setting a background image of a particular width and height -->
![bg right:45% width:90%](media/EnergyLandscape.png)

---

# The Encoder

- Evolution functions as a learning algorithm, similar to those used in machine learning.
- Natural selection plays a crucial role in shaping this generative model over time. Variations arise in the genome, leading to phenotypic differences among organisms.
- Those with traits better suited to the environment have higher reproductive success, increasing the frequency of their genes in the next generation

![bg right:45% width:90%](./media/peppermoth.jpg)

---

# Properties of Generative model

1. Compression through a bottleneck layer.
2. Encoding in a latent variable space.
3. Abstract, indirect representations.
4. Intrinsic variability of outputs.
5. Robustness.
6. Evolvability.

---

# Properties are interrelated

- Compression enforces the abstraction and encoding of latent variables.
- Alteration of individual latent variables is often tolerated by the system, which gives rise to robustness.
- The noise is not simply a flaw; it's an integral part of the system that enables robustness and evolvability.
- Paradoxically, robustness leads to evolvability.

---

# Emergent modularity, Disentangled representations

<style scoped>
  h1 {
    font-size: 24px;
  }
  img {
    border-radius: 50px;
  }
</style>

![w:800 h:540 opacity:1.0](media/Modularity.png)

---

# Future Prospects

- Revolutionizing Developmental Biology Research
  - Moving Beyond Reductionism
  - Formalizing Waddington's Landscape
  - Leveraging Deep Learning
- Advancing the Field of Artificial Life
  - More Realistic Encoding Schemes
  - Harnessing Machine Learning for ALife
- Deeper Understanding of Evolution and Genetic Architecture
  - Explaining Complex Trait Evolution
  - Predicting Evolutionary Trajectories
---

# References 

1. Mitchell, Kevin J., and Nick Cheney. "The Genomic Code: The genome instantiates a generative model of the organism." arXiv preprint arXiv:2407.15908 (2024).


---

<!-- _paginate: false -->
<!-- _footer: '' -->
<style scoped>
  h1 {
    color: #F8F16F;
    margin-top: 250px;
    text-align: center;
  }
</style>

# _Questions?_
