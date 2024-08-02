# Deep Q-Learning Hospital Navigation Agent

## Project Overview

This project implements a reinforcement learning agent using Deep Q-Learning to navigate a simulated hospital environment. The agent, representing a nurse assistant, must efficiently navigate a 5x5 grid to reach a medicine cabinet while avoiding collisions with doctors and nurses.

## Environment Description

- 5x5 grid representing a hospital floor
- Agent: Nurse assistant (🙂)
- Static objects: 5 Beds, 1 Medicine Cabinet, 1 Doctor, 1 Nurse
- Actions: Move Up, Down, Left, Right
- Rewards:
  - Reaching Medicine Cabinet: +10
  - Reaching a Bed: +1
  - Colliding with Doctor or Nurse: -5
  - Each step: -0.1 (to encourage efficiency)
- Termination Conditions:
  - Reaching the Medicine Cabinet (success)
  - Colliding with Doctor or Nurse (failure)
  - Max steps reached (100 steps)

## Project Structure

- `HospitalNavigation_env.py`: Custom Gym environment implementation
- `train.py`: Script to train the DQN agent
- `play.py`: Script to run simulations with the trained agent
- `hospital_navigation_weights.h5f`: Saved weights of the trained model
- `requirements.txt`: List of required Python packages

## Installation

1. Clone this repository:

```

git clone https://github.com/freedisch/DQN.git
cd DQN

```

2. Install the required packages:

```

pip install -r requirements.txt

```

## Usage

1. To train the agent:

```

python train.py

```

2. To run a simulation with the trained agent:

```

python play.py

```

## Video Demonstration

[Link to 5-minute video demonstration](https://youtu.be/gFM__0xhhmg)

## Technologies Used

- Python 3.8+
- OpenAI Gym
- Keras
- Keras-RL
- TensorFlow

## Author

Thibaut Batale

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
