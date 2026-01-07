---
title: Regularización con cotas de Lipschitz
subtitle: Reduciendo el sobreajuste en redes neuronales

event: Workshop en Ciencias de la Computación

location: Universidad Nacional de Colombia
address:
  street: Campus la Nubia
  city: Manizales
  country: Colombia

summary: En esta charla se introduce un metodo para reducir el sobreajuste en redes neuronales usando una regularización adaptativa basada en cotas de Lipschitz (LBA).
abstract: 'Las redes neuronales profundas son modelos ampliamente utilizados en aprendizaje automático y sustentan la mayoría de los sistemas actuales de IA. Estos modelos, sin embargo, son propensos a aprender particularidades del conjunto de entrenamiento que deterioran su desempeño en datos no vistos. Para mitigar este problema, presento un enfoque de regularización adaptativa basado en cotas de Lipschitz (LBA) que controla la sensibilidad del modelo ante perturbaciones de entrada. En experimentos con datos de imágenes y tabulares, el método propuesto reduce sistemáticamente la brecha entrenamiento–validación, mantiene un rendimiento competitivo. El método también mostró un desempeño sólido frente a ataques adversariales. En la charla se abordarán: (i) los fundamentos teóricos del sobreajuste, (ii) la descripción del método LBA, (iii) los resultados experimentales y una introducción a los ataques adversariales, y (iv) posibles líneas de investigación futura.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2025-11-27'
#date_end: '2030-06-01T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
#publishDate: '2017-01-01T00:00:00Z'

authors:
  - admin

tags: [Neural Networks, Overfitting]

# Is this a featured talk? (true/false)
featured: true

image:
    filename: imagen_workshop_2.jpeg
    focal_point: "center"
    preview_only: true

links:
  - type: slides
    url: "slides.pdf"


# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: "slides.pdf"

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
#projects:
#  - example
---

### ✨ Summary

In this talk, I presented my master’s research, which focuses on addressing overfitting in deep neural networks through an adaptive regularization strategy based on Lipschitz Bounds Adaptation (LBA). This work is grounded in our research paper, which provides the theoretical foundation and experimental validation of the proposed method [(paper on LBA)](/publications/jcam-2025/).

The motivation behind this work stems from the tendency of deep neural networks to overfit training data, capturing spurious patterns that negatively affect generalization. The LBA approach mitigates this issue by adaptively controlling the sensitivity of the model to input perturbations via Lipschitz bounds. Through experiments on image and tabular datasets, the method consistently reduces the training–validation gap while preserving competitive performance, and it also exhibits solid robustness against adversarial attacks.

During the talk, I discussed the theoretical foundations of overfitting, detailed the proposed LBA method, and presented experimental results alongside an introduction to adversarial attacks, concluding with potential directions for future research. The support received throughout the talk was excellent, and returning to the university to present my master’s work was a genuinely meaningful and rewarding experience.

<div class="poster-grid">
  <div class="poster-column gif-col">
    <img src="slides.png" alt="Some slides" class="poster-gif"/>
  </div>
  <div class="poster-column">
    <img src="imagen_workshop_2.jpeg" alt="Presenting the talk" class="poster-photo"/>
  </div>
</div>
<div class="poster-button-container">
  <a class="poster-button" href="slides.pdf" target="_blank">📄 View Full Slides (PDF)</a>
</div>