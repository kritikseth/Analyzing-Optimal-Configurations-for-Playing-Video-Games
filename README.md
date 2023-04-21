# Analyzing Optimal Configurations for Playing Video Games

## Introduction
First-person shooter (FPS) games have become increasingly popular in recent years due to the growth of the video game industry, technological advancements, and the rise of e-sports. With the increased accessibility of high-quality hardware and software, players can now play games with high frame rates and improved graphics. In this project, we aimed to understand the optimal conditions for playing video games by analyzing a dataset from OpenML.

View the final report here [DSGA1001_Capstone_report.pdf](report/DSGA1001_Capstone_report.pdf)

## Dataset
The dataset we used is a mix of laptop and desktop CPU/GPU specifications. An ideal dataset would have an extra column specifying if it is a laptop or a desktop. Additionally, if we had the price of each component, we could have analyzed the price for each specification of FPS. However, this information was not available, and we had to work with the given dataset.

Since the original dataset is too big to upload on GitHub, you can find the dataset on [Kaggle](https://www.kaggle.com/datasets/kritikseth/achieved-frames-per-second-fps-in-video-games).

## Methodology
We started by cleaning the dataset to ensure it was error-free and organized. Then, we conducted data exploration to identify trends and patterns in the data. During this process, we discovered a unique relationship between three variables: die size, process size, and transistors. This led us to explore Moore’s Law, a theory that states that the number of transistors on a microchip will double approximately every two years.

To test the validity of Moore’s Law, we performed a hypothesis test, with the null hypothesis being that Moore’s Law is still accurate today. After analyzing the data, we were unable to reject the null hypothesis and thus concluded that Moore’s Law remains true. Using this information, we were able to impute missing values for transistor counts using Moore’s Law.

With the final dataset complete, we then conducted predictive analyses to further understand the optimal conditions for video game playing. We also pursued the prediction of game settings that each configuration could be classified into. Our cleaned dataset also allowed us to cluster our dataset based solely on game features of resolution, settings, and FPS.

We performed regression trying to estimate FPS using PC specifications and classification on Game-Resolution to recomment optimal resolution a game should be played on, given PC specifications.

## Conclusion
Through this project, we gained valuable insights into the FPS gaming industry and the factors that contribute to successful gameplay. However, we must note that Die Size and Process Size are different for different SKUs in a company’s product lineup, even if all the SKUs were launched in the same year. This may be because any company might want to cut costs in its lower end products and hence may end up not providing the latest technology. We assume that this trend will continue in the future.

Overall, this project provides a starting point for further research into optimal conditions for playing video games, which could help game developers create better games and enhance the gaming experience for players.

## Mentor

This project was completed with the guidance of [Dr Pascal Wallisch](https://github.com/Pascallisch)

## Installation
```
pip install -r requirements.txt
```

### Clone this repository using the following command:
```
bash git clone https://github.com/kritikseth/Analyzing-Optimal-Configurations-for-Playing-Video-Games.git
```

## Usage
To use this project, navigate to the cloned directory and open the following file:
[OCPVG_final.ipynb](OCPVG_final.ipynb)

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
