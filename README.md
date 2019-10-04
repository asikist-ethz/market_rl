# Reinforcement Learning for Markets

## Quick Intro
This project contains sample code relevant to a possible topic for the project of Agent-Based Modeling and Social System Simulation at ETH Zürich, https://coss.ethz.ch/education/agentBased.html.

The code is not expected to be used as-is, but modifications and testing need to be done from each team, to modify it to their requirements and needs. 
In the case that you detect a bug or any other issue, please don't hesitate to report in the Issues section and/or mention it in the relevant slack channel:
https://abm-teams.slack.com/.

## Installation Info
The proposed implementation relies on usage of Python 3.6 or higher.
For the environment to work, the usage of conda or miniconda is suggested.
This helps to avoid messing up your pc's default python environment. 
Please find information about installing miniconda in:
https://docs.conda.io/en/latest/miniconda.html

Once conda is installed, please create and activate the following environment:

```
conda create -env abm_sss
conda activate abm_sss
# in older version of conda: 
# source activate abm_sss
```

Then it is suggested that you install with pip the following:
```
pip install jupyter
pip install pandas

# for plotting
pip install plotly
pip install holoviews
```

For reinforcement learning, the following libraries are suggested:
```
pip install tensorforce[tf]
#for gpu: 
#pip install tensorforce[tf_gpu]
pip install stable-baselines[mpi]
```

Sometimes the mpi installation may fail with pip, then you can use conda:
```
conda install mpi4py
#the retry with stable baselines
```
In general openai gym is used by the project. This either comes with the stable-baselines module or you can install it via:
```
pip install gym
```

Once everything is installed, please download or clone the project and use it locally, with your editor of choice, from the rl_markets_code folder.

## Examples
A notebook containing appropriate an appropritate example and explanations is found at rl_markets_code/example.ipynb.
At a later stage the github will be updated with reinforcement learning examples relevant to the lectures of 14.10 and 21.10. 
In the meantime you can start experiementing with the above. 

## Project Description
An overview of the project description is found in project_description.pdf.
Relevant papers and the description will be uploaded on the course website in the coming days.

## Further Extensions
Asynchronous versions of the multi-agent environment and single agent environments will be demonstrated in the course. 
Still, you are encouranged to try you own implementations based on the scope of your project untill then. 
