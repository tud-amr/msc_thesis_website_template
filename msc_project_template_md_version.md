---
title: "Sampling Based MPC for Motion Planning of Autonomous Vehicles"
authors:
    - name: "John Doe"
      url: "https://andreumatoses.github.io/"
      superscript: "*1"
    - name: "Luzia Knödler"
      url: "https://andreumatoses.github.io/"
      superscript: "1"
    - name: "Ludwig van Beethoven"
      url: "https://andreumatoses.github.io/"
      superscript: "†"
affiliations:
    - name: "Equal contribution"
      superscript: "*"
    - name: "TU Delft"
      superscript: "1"
      url: "https://tudelft.nl"
    - name: "Wien Opera House"
      superscript: "†"
end_date: 2022-01-01 # end date if ended, approximated if not sure. Just for display purposes and ordering.
# This is the short project description, displayed in the project's card"
description: "This project explores the use of Model Predictive Path Integral (MPPI) control algorithm to enable autonomous robots to navigate complex environments. MPPI is a sampling-based control method that combines path planning and control into a single optimization problem. By iteratively sampling and optimizing trajectories, the algorithm generates control inputs that minimize a cost function while satisfying system dynamics and constraints. The project aims to implement and evaluate the performance of MPPI on a robot platform, showcasing its effectiveness in real-world scenarios."
cover_image: /assets/images/msc_projects/msc_project_template/jackal.jpg # Image displayed in the project's card, make it aspect ratio 1x1 (square) for best results, and keep it a reasonable size (like 1-2MB). Can also be a gif
links: # If you have other website for the project, github repos, datasets, etc. put it here. You can also add an icon from https://icons.getbootstrap.com/
    - name: Paper
      icon: bi-file-earmark-pdf
      url: "/"
    - name: arXiv
      url: "/"
    - name: Code
      icon: bi-github
      url: "/"
    - name: Video
      icon: bi-youtube
      url: "/"
---

All the content in the front matter will be rendered automatically. In this local version, it just shows the content of the front matter as text so ignore it, just make sure you fill the front matter with all the info correctly. You can see an example [here](https://andreumatoses.github.io/amr-website-new/msc_projects_finished/msc-project-template).


<div class="teaser-video d-flex justify-content-center mb-3">
  <div class="ratio ratio-16x9">
    <video id="teaser" autoplay="" muted="" controls="" loop="" playsinline="">
      <source
        src="/assets/images/msc_projects/YY_my-title/sample_video.mp4"
        type="video/mp4">
    </video>
  </div>
</div>

## Summary of the Work

Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat consequatur libero omnis dolore voluptatem.

Sequi nesciunt veniam, ea laboriosam quas corporis quae nobis esse doloremque in aperiam excepturi dignissimos quis? Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi repudiandae vero aliquid molestias at consequatur tempore autem ullam illo provident?


<div class="single-image d-flex justify-content-center mb-3">
  <img src="https://www.migmawei.ca/system/wp-content/uploads/2017/04/Placeholder_16_9-1.png" class="img-fluid" width="600" alt="lab">
</div>

## Showcase 1

Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat consequatur libero omnis dolore voluptatem. Sequi nesciunt veniam, ea laboriosam quas corporis quae nobis esse doloremque in aperiam excepturi dignissimos quis? Lorem ipsum dolor sit amet consectetur adipisicing elit.

Sequi repudiandae vero aliquid molestias at consequatur tempore autem ullam illo provident?

<!-- This basically puts images in a grid of X columns. row-cols-md-X, where X means how many columns. md means until the screen is smaller than medium (ipad). Change X for 2,3,4,6,8,12 -->
<div class="image-grid text-center mb-2">
  <div class="row row-cols-1 row-cols-sm-2 row-cols-md-2 g-2">
    <div class="col">
      <img class="img-fluid object-fit-contain"
        src="/assets/images/msc_projects/YY_my-title/hackathon-team.jpg"
        alt="Image 1">
    </div>
    <div class="col">
      <img class="img-fluid object-fit-contain"
        src="/assets/images/msc_projects/YY_my-title/lab-hackathon.jpg"
        alt="Image 2">
    </div>
  </div>
</div>


Some code that explains something important. Use the highlight tag to highlight code. You can use `inline code`. NOTE: code blocks will not render correctly in the local template.

```python
import torch
import torch.nn as nn

class VAE(nn.Module):
def __init__(self, input_dim, hidden_dim, latent_dim):
super(VAE, self).__init__()

self.encoder = nn.Sequential(
nn.Linear(input_dim, hidden_dim),
nn.ReLU(),
nn.Linear(hidden_dim, latent_dim * 2) # Output mean and log variance
)

return reconstructed_x, mu, log_var
```

Some cool math equations here. You can just use math like in latex e.g $x^2$ or $\alpha = \int_{\beta}^\gamma 1 \; dt$. For inline, use `$ ... $`, for block, use `\[ ... \]`.

\[
\begin{aligned}
\dot{x} &= \sigma(y-x) \\
\dot{y} &= \rho x - y - xz \\
\dot{z} &= -\beta z + xy
\end{aligned}
\]

## Showcase 2

Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat consequatur libero omnis dolore voluptatem. Sequi nesciunt veniam, ea laboriosam quas corporis quae nobis esse doloremque in aperiam excepturi dignissimos quis? Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi repudiandae vero aliquid molestias at consequatur tempore autem ullam illo provident?

<!-- This basically puts images in a grid. row-cols-md-X, where X means how many columns. md means until the screen is smaller than medium (ipad). Change X for 2,3,4,6,8,12 -->
<div class="image-grid text-center mb-2">
<div class="row row-cols-1 row-cols-sm-2 row-cols-md-4 g-2">
  <div class="col">
    <img class="img-fluid object-fit-contain"
      src="/assets/images/msc_projects/YY_my-title/hackathon-team.jpg"
      alt="Image 1">
  </div>
  <div class="col">
    <img class="img-fluid object-fit-contain"
      src="/assets/images/msc_projects/YY_my-title/dingo_manipulator.png"
      alt="Image 1">
  </div>
  <div class="col">
    <img class="img-fluid object-fit-contain"
      src="/assets/images/msc_projects/YY_my-title/hackathon-team.jpg"
      alt="Image 1">
  </div>
  <div class="col">
    <img class="img-fluid object-fit-contain"
      src="/assets/images/msc_projects/YY_my-title/hackathon-team.jpg"
      alt="Image 1">
  </div>
  <div class="col">
    <img class="img-fluid object-fit-contain"
      src="/assets/images/msc_projects/YY_my-title/dingo_manipulator.png"
      alt="Image 1">
  </div>
  <div class="col">
    <img class="img-fluid object-fit-contain"
      src="/assets/images/msc_projects/YY_my-title/hackathon-team.jpg"
      alt="Image 1">
  </div>
</div>
</div>

## Conclusions

Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat consequatur libero omnis dolore voluptatem. Sequi nesciunt veniam, ea laboriosam quas corporis quae nobis esse doloremque in aperiam excepturi dignissimos quis? Lorem ipsum dolor sit amet consectetur adipisicing elit. Sequi repudiandae vero aliquid molestias at consequatur tempore autem ullam illo provident?

Lorem ipsum dolor sit, amet consectetur adipisicing elit. Sit optio qui illo quo nam adipisci dolorum maiores molestias. Maxime hic nihil laboriosam harum, dignissimos ex minus, veritatis nobis porro aspernatur laborum facere ea voluptate ipsa. Minima adipisci quo tenetur quod.

<hr>
