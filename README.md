 <h1 align="center">
  <br>
  <a href="https://www.overleaf.com"><img src="https://user-images.githubusercontent.com/31168586/65396910-dbd1f300-dd81-11e9-9a98-8f4f329461e0.png" alt="Overleaf" width="400"></a>
</h1>

<h4 align="center">

CHALLENGE ROSI 2019 Competition Team</h4>

<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="https://github.com/overleaf/overleaf/wiki">Wiki</a> •
  <a href="#Instructions">Instructions</a> •
  <a href="#Team">Team</a> •
  <a href="#license">License</a>
</p>

<a href="https://www.overleaf.com"><img src="https://user-images.githubusercontent.com/31168586/65396913-e096a700-dd81-11e9-9b02-68e3119673cd.png" alt="Overleaf" ></a>

## Key Features

The team's main objective is to develop computational algorithms applied to autonomous robots, using techniques of artificial intelligence and computer vision. This code was desenvolver for the ROSI CHALLENGE simulation 2019.

## Instructions

##### 1. Copy the follow files in the script folder:
- [ ] *valeNeuralNetwork.ipynb*  # Description of strategy used in competition
- [ ] *rosi_joy.py* # Rosi node
- [ ] *model.h* # Trainned CNN model to avoid obstacles
- [ ] *modelLadder.h* # Trainned CNN model to go up the stairs
- [ ] *model.py* # To train a new CNN model

##### 2. Now, create the follow folders in the script folder:
- [ ] *rgb_data* # To save data for training a new CNN model
- [ ] *robotCommands* # To sabe the xls file with the motors traction commands
- [ ] *map* # To save the GPS tracking

##### 3. Replace your own paths in the Rosi node 
- [ ] model1 = load_model('/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/model.h5') 
- [ ] model2 = load_model('/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/modelLadder.h5') 
- [ ] path_to_imageName1 = '/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/'+imageName1+'/' 
- [ ] path_to_imageName2 = '/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/'+imageName2+'/' 
- [ ] path_to_folder = '/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/robotCommands/' 
- [ ] path_to_folder = '/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/map/' 
- [ ] plt.savefig('/home/raphaell/catkin_ws_ROSI/src/rosi_defy/script/map/map.png') 


##### 4. Open a bash terminal and tipe the follow commands:
- `$ roscore` # start a ROS master

###### 4.1 In a new bash tab:
- `$ vrep` # to open the vrep simulator

###### 4.2 In a new bash tab:
- `$ cd catkin_ws` # open your catkin workspace
- `$ source deve/setup.bash` # source the path
- `$ roslaunch rosi_defy rosi_joy.launch --screen` # start the Rosi node

##### 5. Install the dependences:
- `$ sudo apt install python-pip` # pip2 install
- `$ pip2 install "numpy<1.17" ` # Numpy version<1.17
- `$ pip2 install https://storage.googleapis.com/tensorflow/linux/cpu/tensorflow-1.14.0-cp27-none-linux_x86_64.whl` # Tensorflow version 1.14.0
- `$ pip2 install keras==2.2.5` # Keras version 2.2.5

##### 6. Load the vrep scene and start the simulation



## Team

Institutions: Federal Institute of Paraiba - IFPB - (Cajazeiras) and Federal Institute of Bahia - IFBA (Vitoria da Conquista).
* Raphaell Maciel de Sousa (team leader/IFPB)
* José Alberto Diaz Amado (IFBA)
* Gerberson Felix da Silva (IFPB)	
* Jean Carlos Palácio Santos (IFBA)
* Rafael Silva Nogueira Pacheco (IFBA)
* Michael Botelho Santana (IFBA)
* Sérgio Ricardo Ferreira Andrade Júnior (IFBA)
* Lucas dos Santos Ribeiro (IFBA)
* Félix Santana Brito (IFBA)



## License

Copyright (c) ForROS, 2019.
