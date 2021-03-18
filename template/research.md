## 卖菜爆气表

#### MEMBERS
<p style="font-family: 'gaoyuan'; font-size:1em; color: #A8A8A8"><b>
隼：  录屏 - 四模，代码，整合
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: indianred"><b>
当歌： 录屏 - 星弹泡 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #ec971f"><b>
东野： 描述
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #E2F129"><b>
㳸開： 录屏 - 星弹弦 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #34ce57"><b>
花戏： 描述 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #28a745"><b>
明哲： 录屏 - 弹弦 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #29D0F1"><b>
千弦： 录屏 - 星弹弦 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #8879DE"><b>
思豆： 排版、校对、整合 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #9F79DE"><b>
严： 录屏 - 星弹泡 
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #C979DE"><b>
有饼： 描述
</b></p>

<p style="font-family: 'gaoyuan'; font-size:1em; color: #F97CC0"><b>
真理： 录屏 - 泡弦
</b></p>

[comment]: <> (Motion planning is used in robotics for finding a sequence of valid configurations that moves the robot from the source to a destination.)

[comment]: <> (![Figure 1]&#40;imgs/Simulation.jpg "The simulation results of moving three exemplary objects. &#40;a&#41; The robot pile up three Domino blocks. &#40;b&#41; The robot stacks up two Coke cans. &#40;c&#41; The robot piles up three tissue boxes."&#41;)

[comment]: <> (**Fig.1**: The simulation results of moving three exemplary objects. &#40;a&#41; The robot pile up three Domino blocks. &#40;b&#41; The robot stacks up two Coke cans. &#40;c&#41; The robot piles up three tissue boxes.)

[comment]: <> (![Figure 2]&#40;imgs/RealExecution.jpg "The real-world executions of previous simulation results. &#40;a&#41; The robot moves three Domino blocks to the goal. &#40;b&#41;The robot piles up two Coke cans. &#40;c&#41; The robot moves three tissue boxes to the goal."&#41;)

[comment]: <> (**Fig.2**: The real-world executions of previous simulation results. &#40;a&#41; The robot moves three Domino blocks to the goal. &#40;b&#41;The robot piles up two Coke cans. &#40;c&#41; The robot moves three tissue boxes to the goal.)

[comment]: <> (>[This paper]&#40;https://arxiv.org/pdf/1909.00192.pdf "Combined Task and Motion Planning for a Dual-arm Robot to Use a Suction Cup Tool"&#41; proposes a combined task and motion planner for a dual-arm robot to use a suction cup tool. The planner consists of three sub-planners – A suction pose subplanner and two regrasp and motion sub-planners. The suction pose sub-planner finds all the available poses for a suction cup tool to suck on the object, using the models of the tool and the object. The regrasp and motion sub-planner builds the regrasp graph that represents all possible grasp sequences to reorient and move the suction cup tool from an initial pose to a goal pose. Two regrasp graphs are used to plan for a single suction cup and the complex of the suction cup and an object respectively. The output of the proposed planner is a sequence of robot motion that uses a suction cup tool to manipulate objects following human instructions. The planner is examined and analyzed by both simulation experiments and real-world executions using several real-world tasks. The results show that the planner is efficient, robust, and can generate sequential transit and transfer robot motion to finish complicated combined task and motion planning tasks in a few seconds.)

[comment]: <> (#### Assembly Planning)

[comment]: <> (Assembly planning is to automatically find the detailed sets of instructions for the robot to assembly the product.)

[comment]: <> (![Figure 3]&#40;imgs/ex2.png "&#40;a&#41; Four-block assembly involves unstable assembly. &#40;b&#41; Seven-block assembly assembles the blocks into a cube."&#41;)

[comment]: <> (**Fig.3**: &#40;a&#41; Four-block assembly involves unstable assembly. &#40;b&#41; Seven-block assembly assembles the blocks into a cube.)

[comment]: <> (![Figure 4]&#40;imgs/real.png "&#40;a.1&#41;  The  left  picture  is  the  initial  configuration  of  the  assembly.  The  right  picture  is  the  final  configuration  of  the  robot  and  the  final  poseof  the  assembly.  &#40;a.2&#41;  It  is  the  initial  and  final  configuration  of  the  second  experiment.  &#40;b&#41;  The  robot  assembles  the  three  components  according  to  thesequence, direction, grasp configurations, auxiliary grasp configuration and assembly direction generating by the proposed planner. The red arrows indicatethe assembly direction. The left group of images is the simulation result of the motion planner. The right group of images is the real-world execution. &#40;c&#41;The left is the simulation result. The right is the real-world execution of the second experiment."&#41;)

[comment]: <> (**Fig.4**: &#40;a.1&#41;  The  left  picture  is  the  initial  configuration  of  the  assembly.  The  right  picture  is  the  final  configuration  of  the  robot  and  the  final  poseof  the  assembly.  &#40;a.2&#41;  It  is  the  initial  and  final  configuration  of  the  second  experiment.  &#40;b&#41;  The  robot  assembles  the  three  components  according  to  thesequence, direction, grasp configurations, auxiliary grasp configuration and assembly direction generating by the proposed planner. The red arrows indicatethe assembly direction. The left group of images is the simulation result of the motion planner. The right group of images is the real-world execution. &#40;c&#41;The left is the simulation result. The right is the real-world execution of the second experiment.)



[comment]: <> (>[This paper]&#40;https://arxiv.org****/pdf/2003.00699.pdf "Planning to Build Soma Blocks Using a Dual-arm Robot"&#41; presents a planner that can automatically find an optimal assembly sequence for a dual-arm robot to assemble the soma blocks. The planner uses the mesh model of objects and the final state of the assembly to generate all possible assembly sequence and evaluate the optimal assembly sequence by considering the stability, graspability, assemblability, as well as the need for a second arm. Especially, the need for a second arm is considered when supports from worktables and other workpieces are not enough to produce a stable assembly. The planner will refer to an assisting grasp to additionally hold and support the unstable components so that the robot can further assemble new workpieces and finally reach a stable state. The output of the planner is the optimal assembly orders, candidate grasps, assembly directions, and the assisting grasps if any. The output of the planner can be used to guide a dualarm robot to perform the assembly task. The planner is verified in both simulations and real-world executions.)