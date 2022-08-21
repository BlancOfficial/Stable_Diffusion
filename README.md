# Unofficial Stable-Diffusion
by StabilityAI

Leaked stable diffusion weights collab, working on top off CompVis' GitHub Project,  bringing AIs to the People

[stability ai blogpost](https://stability-ai.webpkgcache.com/doc/-/s/stability.ai/beta-signup-form)

[offical github](https://github.com/CompVis/stable-diffusion)

Now With
(TechnoMancer) Added Image Prompt Utility,
(BlancDeOfficial) Added Google Drive integration, Random Seed, Friendlier User interface and made the 7GB download a one time affair,
(lukasaey) Added Random/ Custom Seed options

![Anarchy Reference](https://cdn.discordapp.com/attachments/806288700736405506/1010835283211714730/unknown.png)

---

NOTE: IF AN ERROR MESSAGE APPEARS SAYING Cannot connect to GPU backend, THERE ARE NO GPUs AVAILABLE; TRY AGAIN LATER

---

For information on the technical side of this AI's Image Generation Capabilities, see the [offical github](https://github.com/CompVis/stable-diffusion)

---

# Step By Step Guide for Dummies w/ images

![Run All](https://cdn.discordapp.com/attachments/806288700736405506/1010840674272280576/Screenshot_2022-08-21_at_10.05.52.png)

By Clicking The Run All Button, you also start the process in which google colab connects to a GPU runtime

---

![Lack of GPUs](https://cdn.discordapp.com/attachments/806288700736405506/1010843232239886377/Screenshot_2022-08-21_at_10.29.42.png)

If You get this error message, there are no free GPUs at the time and so it is recommended you Ctrl + R a million times, or more preferably you try again at another time

---

![Drive Integration](https://cdn.discordapp.com/attachments/806288700736405506/1010840674603651133/Screenshot_2022-08-21_at_10.10.36.png)

If It has successfully started running you will see this message within the first minute of running the colab, click Connect to Google Drive, sign in and click Accept
Google Drive Integration is vital for the colab to run as image output and model storage rely on drive

---

![Kill Switch](https://cdn.discordapp.com/attachments/806288700736405506/1010840675031449600/Screenshot_2022-08-21_at_10.13.59.png)

Once cell 1.5 Model Downlod Check has finished running, the colab is designed to crash, this is a feature not a bug
You will not need to rerun cells 1.1 to 1.5 again during this runtime

---

![Running after Breakpoint](https://cdn.discordapp.com/attachments/806288700736405506/1010840675455082496/Screenshot_2022-08-21_at_10.15.34.png)

To Continue with the AI generation process click on the cell that says cd/content/stable-diffusion/, then follow by pressing Ctrl +  F10.
Alternatively you could click on the cell click, then click the Runtime Tab on the top left, and then Run After

---

![Parameters](https://cdn.discordapp.com/attachments/806288700736405506/1010840675769663540/Screenshot_2022-08-21_at_10.16.56.png)

NOTE: AFTER CHANGING PARAMETERS, RERUN CELLS 3.1 TO 3.7
|Parameter            |Description                                                                                  |
| ------------------- | ------------------------------------------------------------------------------------------- |
|self.ddim_steps      | number of ddim sampling steps|

self.seed SEED         the seed (for reproducible sampling)

self.n_rows            rows in the grid (default: n_samples)

self.C                 latent channels

self.H                 image height, in pixel space

self.W                 image width, in pixel space

self.F                 downsampling factor

self.n_samples         how many samples to produce for each given prompt. A.k.a. batch size

self.n_iter            sample this often

self.scale             unconditional guidance scale: eps = eps(x, empty) + scale * (eps(x, cond) - eps(x, empty))

self.strength          The Weight of the Image prompt. NOTE: MAXES OUT AT 0.99 AND MUST ATLEAST BE 0.01

