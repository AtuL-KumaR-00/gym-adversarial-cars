# Adversarial Chase and Run Cars Gym 
<div align="center">
   <img src=https://img.shields.io/badge/version-0.0.1-red>
   <img src=https://img.shields.io/badge/license-MIT-brightgreen>
</div>

Adversarial Chase and Run Cars Gym is a **gym environment**, to test and develop algorithms related to **Multi Agent Systems**, especially those related to Multi-Agent Reinforcement Learning. This was done under the **Robotics Research Group (RoboReG)** to try and learn emergent behavior between agents competing against each other via Reinforcement learning and how it could generate new control strategies.

This gym environment consists of **2 mobile robots**, where the task of one of the robots is to chase the other one, while the other simply avoids the chaser. The environment also consists of **walls which define the operating area**, so that the robots remain confined in a particular area. Though this has been done in 2D-worlds, **analyzing emergent behaviour** in a physical world with **real physics and dynamics** is a relatively less explored area.

<p align="center">
   <img src="media/cars.gif">
</p>

The gym environment was built in the physics simulator **[PyBullet](https://pybullet.org/) - a python module for physics simulations of robots**, because of its easy usage and integration with RL frameworks like **Stable Baselines**. Work is currently being done on training the agents to compete via Multi Agent Reinforcement Learning.

The **mobile robots** that are being used in the environment were built and designed completely in **Blender**, and were exported as **URDFs**, so that they could be imported in all physics simulators.

<p align="center">
<img src="media/auto.png">
</p>

## Objective

One of the key challenges and active areas of research in **robotics and control systems** are **multi-agent systems**, especially those which involve collaboration or competition between individual systems. The **traditional control strategies** in these situations require a lot of control equations with **underlying mathematics** and **physical dynamics** of the system along with the communication protocols. This however, confines these systems to work in an already known fashion without display of any new behaviour. Through this project, we aim to visualize **new emergent behaviours** in competitive as well as mixed settings (competitive + collaborative) using **multi-agent reinforcement learning** as they provide a more robust and efficient way of developing a control system with the ability to perform new behaviours than traditional methods.

## Installation Guidelines

This gym environment can be installed by following these steps:

0. Although not compulsory, we strongly recommend creating a virtual environment specific to this project. This will help in package management and for decluttering your workspace. A simple way to create a virtual environment is as follows:

   ~~~bash
   python3 -m venv <Env_Name>
   ~~~

   Activation and deactivation of the virtual environment, will be done as specified [here](https://docs.python.org/3/library/venv.html). Scroll down to the table where the activation method for various operating systems is provided. Deactivation, in most cases, can be done by simply typing deactivate while being in in the virtual environment.

1. Once you activate your virtual environment, you will have to install the various dependencies of this project. We have simplified this process for you. Just follow the following steps:
   * Download/Clone this repository on to your local machine
   * Navigate to the root folder of this repository through your terminal.
   * Execute the following command in your terminal.

      ~~~bash
      pip install -e adversarial-gym
      ~~~
   * Now, the environment can be created by calling this function in the python file:
      ~~~
      env = gym.make("adversarial_cars-v0")
      ~~~

In case there are problems with the PyBullet installation, you can refer to this [guide](https://github.com/Robotics-Club-IIT-BHU/Robo-Summer-Camp-20/blob/master/Part1/Subpart%201/README.md).

## Contributions
Contributions are welcome! However, if it's going to be a major change, please create an issue first. Before starting to work on something, please comment on a specific issue and say you'd like to work on it.

## Made and maintained by ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
     <td align="center"><a href="http://terabyte17.github.io"><img src="https://avatars3.githubusercontent.com/u/60649571?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yash Sahijwani</b></sub></a><br /><a href="https://github.com/Robotics-Club-IIT-BHU/gym-adversarial-cars/commits?author=Terabyte17" title="Code">💻</a> <a href="#ideas-Terabyte17" title="Ideas, Planning, & Feedback">🤔</a></td>
     <td align="center"><a href="https://github.com/aksayushx"><img src="https://avatars2.githubusercontent.com/u/55887638?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ayush Kumar Shaw</b></sub></a><br /><a href="#ideas-aksayushx" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/Robotics-Club-IIT-BHU/gym-adversarial-cars/commits?author=aksayushx" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/Raghav-Soni"><img src="https://avatars1.githubusercontent.com/u/60649723?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Raghav-Soni</b></sub></a><br /><a href="https://github.com/Robotics-Club-IIT-BHU/gym-adversarial-cars/commits?author=Raghav-Soni" title="Code">💻</a> <a href="#ideas-Raghav-Soni" title="Ideas, Planning, & Feedback">🤔</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## Advisors and Mentors 🙌
<table>
   <td align="center">
      <a href="https://github.com/lok-i">
         <img src="https://avatars1.githubusercontent.com/u/54435909?s=460&u=29af076049dab351b2e43621e9a433919bf50fb1&v=43" width="100px;" alt=""/>
         <br />
         <sub>
            <b>Lokesh Krishna</b>
         </sub>
      </a>
      <br />
   </td>   
   <td align="center">
      <a href="https://github.com/NiranthS">
         <img src="https://avatars3.githubusercontent.com/u/44475481?s=400&v=4" width="100px;" alt=""/>
         <br />
         <sub>
            <b>Niranth Sai</b>
         </sub>
      </a>
      <br />
   </td>   
</table>
