# The BoME dataset
### Overview
we created the __BoME__ (**Bo**dy **M**otor **E**lements) dataset, comprising 1,600 high-quality video clips of human movements. We consider different human movements within a single video as distinct clips. Each of these clips is annotated with precise, expert-provided movement labels. We used the AVA video dataset as the video source and applied the Laban Movement Analysis (LMA) system to describe the motor elements. LMA, which originated within the dance community in the early 20th century, has evolved into an internationally recognized framework for describing and comprehending human bodily motions. It characterizes human movements into five categories: __Body__, __Effort__, __Space__, __Shape__, and __Phrasing__,  and includes over a hundred detailed motor elements. To balance the tradeoff between the number of LMA elements and the cost of annotation, we selectively included eleven emotion-related LMA elements. This decision was guided by preliminary psychological research exploring the relationship between emotions and motor elements as described by LMA. We designed a systematic procedure for dataset collection and invited a Certified Movement Analyst (CMA), an expert in LMA, to annotate the presence of LMA elements in the human movement clips. Below shows some examples of the BoME dataset.

### Examples
<!-- ![examples](examples.png) -->
<div align="center">
<img src="examples.png" alt="examples" width="600">
</div>
Three sample frames are shown for each clip. Instances of interest are bounded by red boxes.The LMA motor elements annotated based on the movement of the person in the red box  are shown.
### Downloads
The annotations are here: [LMA_coding_cleaned_enlarge.csv](LMA_coding_cleaned_enlarge.csv) provides the whole annotations. We split the dataset into training and test set, namely [LMA_coding_cleaned_enlarge_train.csv](LMA_coding_cleaned_enlarge_train.csv) and [LMA_coding_cleaned_enlarge_val.csv](LMA_coding_cleaned_enlarge_val.csv).
### Paper
For more details of the dataset and corresponding experiments, please refer to our [paper](https://arxiv.org/abs/2304.02187).
### Code
We also provide the code to estimate LMA elements on BoME and the code to enhance Bodily Expressed Emotion Understanding (BEEU) with BoME. They are in the folders emotion_action and emotion_swin_video of the [OneDrive](https://pennstateoffice365-my.sharepoint.com/:f:/g/personal/czw390_psu_edu/EnKgLsQYlIhDmEqlYND8SuEBTCLaX7q-4ODMB_S9w0mxqA?e=6a6BHK). To run the LMA element estimation experiments, please refer to [README1.md](https://pennstateoffice365-my.sharepoint.com/:f:/g/personal/czw390_psu_edu/EswU_gNZ_phEmYNgxvlsLR0B9bfcGa-BoG2r0LVr69W8XA?e=NrBZ7S). To reproduce the BEEU experiments, please refer to [README2.md](https://pennstateoffice365-my.sharepoint.com/:f:/g/personal/czw390_psu_edu/EswU_gNZ_phEmYNgxvlsLR0B9bfcGa-BoG2r0LVr69W8XA?e=NrBZ7S).