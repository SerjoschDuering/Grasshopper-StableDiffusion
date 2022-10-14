
# !!! Outdated please use this [improved repro](https://github.com/SerjoschDuering/StableDiffusion-Grasshopper) !!!

## Grasshopper-StableDiffusion

A slightly modified version of **[InvokeAI: A Stable Diffusion Toolkit](https://github.com/invoke-ai/InvokeAI) /** [CompVis/stable-diffusion](https://github.com/CompVis/stable-diffusion) where the stable diffusion model can be connected to grasshopper (or anything else) through sockets. 
The preset mode is image2image translation where a prompt is combined with a guiding input image. In this case, the guiding image is taken from rhino's viewport.
Additionally, a simple humanUI interface is provided. Moreover, the script calling the stable diffusion model through a socket is wrapped in a hops definition to utilize its async functionality (while the image is computed, the viewport won't freeze). 

![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled.png)
![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/spcow.PNG)
## Prerequisites

A) **Stable Diffusion Model**

- Clone this [repro](https://github.com/invoke-ai/InvokeAI) and follow Installation instructions

B) **Grasshopper Plugins**

- install grasshopper [Hops](https://developer.rhino3d.com/guides/compute/hops-component/)
- [Human](https://www.food4rhino.com/en/app/human)
- [HumanUI](https://www.food4rhino.com/en/app/human-ui)

## Set-up

1. Fulfill Prerequisites
2. Download this repository
3. replace [dream.py](http://dream.py) file:
in your stable diffusion folder (prerequisites Step A), navigate to 
\scripts and replace the dream.py file with the dream.py file from this repro

1. Open Rhino 7+, launch grasshopper and open main.gh.
In the upper section of the humanUI window, set viewport name and file path to the stable diffusion model
2. open an **anaconda prompt**  and paste the commands to start the stable diffusion model (see image below)

![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled%201.png)

**Sample Images** 

Naturally, the model is not limited to a particular domain

![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled%202.png)

![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled%203.png)
