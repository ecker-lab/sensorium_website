---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default

---

# SENSORIUM 2023

## The Problem

**Even today's most advanced models of visual cortex are not able to fully predict the brain's responses.**

Understanding how the brain processes visual input is a long standing goal in neuroscience. To solve this question in a quantitative, testable, and reproducible way, accurate predictive models of neural population responses to natural stimuli are crucial. However, even today's most advanced models of visual cortex are only able to account for a fraction of the observed neuronal activity. Furthermore, because there is an abundance of models and metrics, but no widely-used reference dataset, it is challenging to compare models on equal ground. This makes it difficult to determine the current state-of-the-art model.

<img src="../assets/images/sensorium_2023_schematic.png" alt="SENSORIUM 2023 schematic">

## The SENSORIUM 2023 Competition

**Benchmarking the predictive performance of your model on large-scale datasets.**

The SENSORIUM 2023 competition offers a publicly available, large-scale dataset consisting of the activity from over 38,000 neurons from the primary visual cortex of five different mice in response to around 1800 natural scene videos (around 10 seconds). The dataset also includes additional behavioral measurements such as running speed, pupil dilation and eye movements. The performance of predictive models can be automatically evaluated by submitting predicted neural responses to our website which will display the performance of all submissions in a leaderboard for easy comparison.

The SENSORIUM 2022 competition approached this issue for static stimulus (pictures) models. This year we are adding a time dimensional component and try to inspire community to establish a benchmark dataset and a model for dynamic stimulus (videos). See more about data in the whitepaper and data section.

**Currently, we offer two benchmark tracks**

<!-- Stimulus-only in our SENSORIUM track, and stimulus-and-behavior in our SENSORIUM+ track. Stimulus-only models are assessed on how well they predict neural activity solely considering the stimulus averaged over trials. Since the animal's behavior and its internal brain state influence the responses, we introduce the SENSORIUM+ track, where model performance is assessed based on how well they can predict individual trials given behavioral variables. -->
There is a main track and a bonus track. The focus of the main track is to predict the neuronal activity for dynamic stimuli, while the focus of the bonus is to generalize to out of domain (OOD) stimuli.

**Main Track**

We provide data from 5 mice, more than 38,000 neurons, around 1800 natural scene videos (around 10 seconds), and additionally behavioral activity (pupil center, pupil dilation, and running speed). The goal is to train a networks, which would predict the neuronal activity for the neurons. To see more details about data or metrics see the corresponding section.
*Please note that this year there is not separate track for behaviour. It is up for the team if they want to use behavioural data or not.*

**Bonus Track**

We think that from a biological perspective it is crucial to have not only good performing but also generalizable models. Hence, we establish a bonus track with five out of domain (OOD) stimuli to measure the models' generalizable capabilities. This track would have one winning team.

**Let's predict how the brain processes what we see!**

## Timeline
* May 22    Full website and starting kit release.
* June 01     Start of the competition and data release.
* Sept 22    Submission deadline.
* Sept 29    Validation of all submitted scores completed. Final test set scores released. Rank 1-3 in
                 both competition tracks are contacted to provide the code for their submission.
* Oct 13      Deadline for top-ranked entries to provide the code for their submission.
* Oct 23     Winners contacted to contribute to the competition summary write-up.


## Getting Started

To ensure you have a swift and easy start participating in our competition we prepared a starting kit for you. The starting kit (link to Github [https://github.com/ecker-lab/sensorium_2023](https://github.com/ecker-lab/sensorium_2023)) includes a comprehensive 3-step manual with code examples for installing required software, downloading and inspecting the competition data, and training and submitting a model to the competition website.

* Code to download our complete corpus of data and how to load it for model-fitting.
* A visual guide to the properties of the dataset, to give neuroscientists as well as non-experts an overview of the scale and all properties of the data.
* Code to re-train the baselines, as well as checkpoints to load our provided baselines.
* Ready-to-use code to generate a submission entry, given only the model as an input.
* Furthermore, you can find details about the competition data and design in our whitepaper.

<!-- Our full dataset can be downloaded here: Download DataAvailable Now! -->

## Rules

* **No restrictions**              We do not place any restrictions on the approaches you can choose
                                        from, be it by inclusion of additional data, or by using pre-trained
                                        models.
* **Submission deadline**   To be eligible for consideration, submissions must be sent between 
                                        23:59 AOE (anywhere on earth) on June 1st, 2023, and 23:59 AOE on 
                                        September 22nd, 2023.
* **Valid email**                     Please ensure that your submission includes a valid email address
                                        during registration.
* **Winning**                         From each team we would take best-performing submission on the
                                        live test set and evaluate these submissions on the final test set.
                                        The top 3 submissions that outperform both ensembled baselines
                                        on the final test set by 23:59 AOE on September 22nd, 2023, will be
                                        considered for the winning positions. The participants responsible
                                        for these submissions will receive an email notification and will have 
                                        until 23:59 AOE on October 13th, 2023, to submit the code for their
                                        winning entry. In order to qualify, the code should be a self-
                                        contained Jupyter notebook that reproduces the submitted model 
                                        predictions.
* **Evaluation**                     The organizers will have time until 23:59 AOE on October 23rd,
                                        2023, to replicate the submission with the provided code. 
                                        If the replication fails, the organizers will reach out to the participant.
                                        In case of the unsuccessful validation, the team will be disqualified, 
                                        and the next highest-ranked submission will be considered.
* **One entry per day**        Each registered user or team is allowed to submit one entry
                                        per day per competition track.
* **Organizers**                     Members of the organizing labs are welcome to submit their
                                        work, but they will not be considered as winners.

## FAQ

**Q: What is this competition about?**  
We are looking for the best neural predictive model that can predict the activity of thousands of neurons in the primary visual cortex of mice in response to natural images.

**Q: Why are neural predictive models interesting?**  
Accurate models of neuronal activity can serve as phenomenological digital twins for the visual cortex, allowing computational neuroscientists to derive new hypotheses about biological vision “in silico”, enabling systems neuroscientists to test them “in vivo”. On top of that, these models are relevant to machine learning researchers who use them to bridge the gap between biological and machine vision.

**Q: Where will the results be presented?**  
We are happy to announce that we are part of the NeurIPS 2023 competition track! We’ll host a virtual workshop at NeurIPS in December 2023 to present the winners and overall results of this competition.

**Q: Are there plans for future data and competition releases?**  
We intend to start the competition this year at NeurIPS, but keep the website open for new challenges to make this website a valuable resource for data driven neural system identification models in mouse visual cortex and beyond.

## Previous competitions

Feel free to also check out our competition from 2022: [SENSORIUM 2022](https://sensorium2022.net/home). The submissions to both competition tracks are still open, and will continue to stay open, so that the state-of-the-art can be improved continuously.

## Organizers

| Polina Turishcheva *(University of Göttingen)* | Eric Y. Wang *(Baylor College of Medicine)* |
| Konstantin F. Willeke *(University of Tübingen)* | Paul G. Fahey *(Baylor College of Medicine)* |
| Laura Hansel *(University of Göttingen)* | Michaela Vystrčilová *(University of Göttingen)* |
| Zhiwei Ding *(Baylor College of Medicine)* | Kayla Ponder *(Baylor College of Medicine)* |
| Alexander Ecker *(University of Göttingen)* | Andreas S. Tolias *(Baylor College of Medicine)* |
| Fabian H. Sinz *(University of Göttingen)* ||

## Contact

Have more questions? Join our [slack workspace](https://join.slack.com/t/sensorium-competition/shared_invite/zt-1bep6o4np-tiO93ekNDdo63UZcRFaCrw)! Or contact us at [contact@sensorium2023.net](mailto:contact@sensorium2023.net).