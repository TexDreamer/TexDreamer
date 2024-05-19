# TexDreamer: Text-driven Photorealistic and Robust Texture Synthesis via
Multi-View Diffusion

### [Project Page](https://imagebind-3d.github.io/imagebind3d/)  | [GitHub]() | [Paper]()

<p align="center" style="text-align:center;">
  <img width="98%" src="./img/01.png">
</p>
<figcaption style="text-align:justify; margin: 0 auto; display: table;">
In this paper, we present TexDreamer, a novel method for generating high-quality 3D textures on meshes guided by text prompts. We address the limitations of existing text-driven texture synthesis methods by proposing
a hybrid approach that combines the expressiveness of texture field representations with the guidance of a multi-view diffusion model and Score
Distillation Sampling (SDS). Our method utilizes a continuous texture field
to capture fine-grained details and complex material properties while ensuring consistency across different views through a multi-view perceptual
loss. Additionally, we incorporate an SDS loss specifically for intermediate regions to generate complete and accurate textures. We evaluate the
performance of our method on a variety of 3D models and demonstrate
its ability to synthesize high-quality, consistent, and detailed textures that
accurately reflect the input text prompt and exhibit realistic material properties. Through comparisons with state-of-the-art methods, we showcase
the superior quality and consistency achieved by our approach.
</figcaption>

<p align="center">
  <div style="display: inline-block; width: 23%;">
   <span style="display: block; text-align: center;">Napoleon with white hair </span>
    <img width="100%" src="./img/01.gif">    
    <br>
  </div>
  <div style="display: inline-block; width: 23%; margin-left: 2%;">
  <span style="display: block; text-align: center;">A barrel </span>
    <img width="100%" src="./img/02.gif">    
    <br>
  </div>
  <div style="display: inline-block; width: 23%; margin-left: 2%;">
  <span style="display: block; text-align: center;">A wooden eagle</span>
    <img width="100%" src="./img/03.gif">    
    <br>
  </div>
  <div style="display: inline-block; width: 23%;margin-left: 2%;">
  <span style="display: block; text-align: center;">A golden plover </span>
    <img width="100%" src="./img/04.gif">    
    <br>
  </div>
</p>

### Approach
<p align="center">
<figcaption style="text-align: justify;">In this paper, we present TexDreamer, a novel coarse-to-fine approach for text-guided 3D texture synthesis designed to overcome
the limitations of existing methods, as illustrated in Figure 2. Our
TexDreamer employs a texture field representation to achieve a
continuous encoding of texture information. By utilizing physicallybased rendering (PBR) techniques, our approach facilitates the generation of high-quality textures with enhanced realism and detail.
In the initial stage, we employ a multi-view diffusion approach to
promote early consensus among the generated anchor views. This
consensus mechanism promotes consistency in the overall structure
and enables the attainment of coherence across different views. In
the second stage, we propose a method that integrates both MSE
loss and SDS losses to generate novel views while simultaneously
preserving the integrity of neighboring anchor views. This hybrid
loss function leverages the complementary strengths of perceptual
and semantic guidance, ensuring both visual coherence and semantic fidelity within the synthesized textures.</figcaption>
  <img width="98%" src="./img/method.jpg">
</p>
