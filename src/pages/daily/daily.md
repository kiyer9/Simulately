## 2024-10-23


### E-3DGS: Gaussian Splatting with Exposure and Motion Events

- **Authors**: Xiaoting Yin, Hao Shi, Yuhan Bao, Zhenshan Bing, Yiyi Liao, Kailun Yang, Kaiwei Wang

#### Abstract

Estimating Neural Radiance Fields (NeRFs) from images captured under optimal
conditions has been extensively explored in the vision community. However,
robotic applications often face challenges such as motion blur, insufficient
illumination, and high computational overhead, which adversely affect
downstream tasks like navigation, inspection, and scene visualization. To
address these challenges, we propose E-3DGS, a novel event-based approach that
partitions events into motion (from camera or object movement) and exposure
(from camera exposure), using the former to handle fast-motion scenes and using
the latter to reconstruct grayscale images for high-quality training and
optimization of event-based 3D Gaussian Splatting (3DGS). We introduce a novel
integration of 3DGS with exposure events for high-quality reconstruction of
explicit scene representations. Our versatile framework can operate on motion
events alone for 3D reconstruction, enhance quality using exposure events, or
adopt a hybrid mode that balances quality and effectiveness by optimizing with
initial exposure events followed by high-speed motion events. We also introduce
EME-3D, a real-world 3D dataset with exposure events, motion events, camera
calibration parameters, and sparse point clouds. Our method is faster and
delivers better reconstruction quality than event-based NeRF while being more
cost-effective than NeRF methods that combine event and RGB data by using a
single event sensor. By combining motion and exposure events, E-3DGS sets a new
benchmark for event-based 3D reconstruction with robust performance in
challenging conditions and lower hardware demands. The source code and dataset
will be available at https://github.com/MasterHow/E-3DGS.

[Website Link](https://github.com/MasterHow/E-3DGS.)

[Paper Link](
https://arxiv.org/abs/2410.16995
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-53.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Implicit Contact Diffuser: Sequential Contact Reasoning with Latent Point Cloud Diffusion

- **Authors**: Zixuan Huang, Yinong He, Yating Lin, Dmitry Berenson

#### Abstract

Long-horizon contact-rich manipulation has long been a challenging problem,
as it requires reasoning over both discrete contact modes and continuous object
motion. We introduce Implicit Contact Diffuser (ICD), a diffusion-based model
that generates a sequence of neural descriptors that specify a series of
contact relationships between the object and the environment. This sequence is
then used as guidance for an MPC method to accomplish a given task. The key
advantage of this approach is that the latent descriptors provide more
task-relevant guidance to MPC, helping to avoid local minima for contact-rich
manipulation tasks. Our experiments demonstrate that ICD outperforms baselines
on complex, long-horizon, contact-rich manipulation tasks, such as cable
routing and notebook folding. Additionally, our experiments also indicate that
\methodshort can generalize a target contact relationship to a different
environment. More visualizations can be found on our website
$\href{https://implicit-contact-diffuser.github.io/}{https://implicit-contact-diffuser.github.io}$

[Website Link](https://implicit-contact-diffuser.github.io/)

[Paper Link](
https://arxiv.org/abs/2410.16571
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-52.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### DiffusionSeeder: Seeding Motion Optimization with Diffusion for Rapid Motion Planning

- **Authors**: Huang Huang, Balakumar Sundaralingam, Arsalan Mousavian, Adithyavairavan Murali, Ken Goldberg, Dieter Fox

#### Abstract

Running optimization across many parallel seeds leveraging GPU compute have
relaxed the need for a good initialization, but this can fail if the problem is
highly non-convex as all seeds could get stuck in local minima. One such
setting is collision-free motion optimization for robot manipulation, where
optimization converges quickly on easy problems but struggle in obstacle dense
environments (e.g., a cluttered cabinet or table). In these situations,
graph-based planning algorithms are used to obtain seeds, resulting in
significant slowdowns. We propose DiffusionSeeder, a diffusion based approach
that generates trajectories to seed motion optimization for rapid robot motion
planning. DiffusionSeeder takes the initial depth image observation of the
scene and generates high quality, multi-modal trajectories that are then
fine-tuned with a few iterations of motion optimization. We integrate
DiffusionSeeder to generate the seed trajectories for cuRobo, a GPU-accelerated
motion optimization method, which results in 12x speed up on average, and 36x
speed up for more complicated problems, while achieving 10% higher success rate
in partially observed simulation environments. Our results show the
effectiveness of using diverse solutions from a learned diffusion model.
Physical experiments on a Franka robot demonstrate the sim2real transfer of
DiffusionSeeder to the real robot, with an average success rate of 86% and
planning time of 26ms, improving on cuRobo by 51% higher success rate while
also being 2.5x faster.

[Paper Link](
https://arxiv.org/abs/2410.16727
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-50.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### EnvBridge: Bridging Diverse Environments with Cross-Environment Knowledge Transfer for Embodied AI

- **Authors**: Tomoyuki Kagaya, Yuxuan Lou, Thong Jing Yuan, Subramanian Lakshmi, Jayashree Karlekar, Sugiri Pranata, Natsuki Murakami, Akira Kinose, Koki Oguri, Felix Wick, Yang You

#### Abstract

In recent years, Large Language Models (LLMs) have demonstrated high
reasoning capabilities, drawing attention for their applications as agents in
various decision-making processes. One notably promising application of LLM
agents is robotic manipulation. Recent research has shown that LLMs can
generate text planning or control code for robots, providing substantial
flexibility and interaction capabilities. However, these methods still face
challenges in terms of flexibility and applicability across different
environments, limiting their ability to adapt autonomously. Current approaches
typically fall into two categories: those relying on environment-specific
policy training, which restricts their transferability, and those generating
code actions based on fixed prompts, which leads to diminished performance when
confronted with new environments. These limitations significantly constrain the
generalizability of agents in robotic manipulation. To address these
limitations, we propose a novel method called EnvBridge. This approach involves
the retention and transfer of successful robot control codes from source
environments to target environments. EnvBridge enhances the agent's
adaptability and performance across diverse settings by leveraging insights
from multiple environments. Notably, our approach alleviates environmental
constraints, offering a more flexible and generalizable solution for robotic
manipulation tasks. We validated the effectiveness of our method using robotic
manipulation benchmarks: RLBench, MetaWorld, and CALVIN. Our experiments
demonstrate that LLM agents can successfully leverage diverse knowledge sources
to solve complex tasks. Consequently, our approach significantly enhances the
adaptability and robustness of robotic manipulation agents in planning across
diverse environments.

[Paper Link](
https://arxiv.org/abs/2410.16919
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-48.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GS-LIVM: Real-Time Photo-Realistic LiDAR-Inertial-Visual Mapping with Gaussian Splatting

- **Authors**: Yusen Xie, Zhenmin Huang, Jin Wu, Jun Ma

#### Abstract

In this paper, we introduce GS-LIVM, a real-time photo-realistic
LiDAR-Inertial-Visual mapping framework with Gaussian Splatting tailored for
outdoor scenes. Compared to existing methods based on Neural Radiance Fields
(NeRF) and 3D Gaussian Splatting (3DGS), our approach enables real-time
photo-realistic mapping while ensuring high-quality image rendering in
large-scale unbounded outdoor environments. In this work, Gaussian Process
Regression (GPR) is employed to mitigate the issues resulting from sparse and
unevenly distributed LiDAR observations. The voxel-based 3D Gaussians map
representation facilitates real-time dense mapping in large outdoor
environments with acceleration governed by custom CUDA kernels. Moreover, the
overall framework is designed in a covariance-centered manner, where the
estimated covariance is used to initialize the scale and rotation of 3D
Gaussians, as well as update the parameters of the GPR. We evaluate our
algorithm on several outdoor datasets, and the results demonstrate that our
method achieves state-of-the-art performance in terms of mapping efficiency and
rendering quality. The source code is available on GitHub.

[Paper Link](
https://arxiv.org/abs/2410.17084
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-47.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Learning Precise, Contact-Rich Manipulation through Uncalibrated Tactile Skins

- **Authors**: Venkatesh Pattabiraman, Yifeng Cao, Siddhant Haldar, Lerrel Pinto, Raunaq Bhirangi

#### Abstract

While visuomotor policy learning has advanced robotic manipulation, precisely
executing contact-rich tasks remains challenging due to the limitations of
vision in reasoning about physical interactions. To address this, recent work
has sought to integrate tactile sensing into policy learning. However, many
existing approaches rely on optical tactile sensors that are either restricted
to recognition tasks or require complex dimensionality reduction steps for
policy learning. In this work, we explore learning policies with magnetic skin
sensors, which are inherently low-dimensional, highly sensitive, and
inexpensive to integrate with robotic platforms. To leverage these sensors
effectively, we present the Visuo-Skin (ViSk) framework, a simple approach that
uses a transformer-based policy and treats skin sensor data as additional
tokens alongside visual information. Evaluated on four complex real-world tasks
involving credit card swiping, plug insertion, USB insertion, and bookshelf
retrieval, ViSk significantly outperforms both vision-only and optical tactile
sensing based policies. Further analysis reveals that combining tactile and
visual modalities enhances policy performance and spatial generalization,
achieving an average improvement of 27.5% across tasks.
https://visuoskin.github.io/

[Website Link](https://visuoskin.github.io/)

[Paper Link](
https://arxiv.org/abs/2410.17246
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-46.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-22


### EVA: An Embodied World Model for Future Video Anticipation

- **Authors**: Xiaowei Chi, Hengyuan Zhang, Chun-Kai Fan, Xingqun Qi, Rongyu Zhang, Anthony Chen, Chi-min Chan, Wei Xue, Wenhan Luo, Shanghang Zhang, Yike Guo

#### Abstract

World models integrate raw data from various modalities, such as images and
language to simulate comprehensive interactions in the world, thereby
displaying crucial roles in fields like mixed reality and robotics. Yet,
applying the world model for accurate video prediction is quite challenging due
to the complex and dynamic intentions of the various scenes in practice. In
this paper, inspired by the human rethinking process, we decompose the complex
video prediction into four meta-tasks that enable the world model to handle
this issue in a more fine-grained manner. Alongside these tasks, we introduce a
new benchmark named Embodied Video Anticipation Benchmark (EVA-Bench) to
provide a well-rounded evaluation. EVA-Bench focused on evaluating the video
prediction ability of human and robot actions, presenting significant
challenges for both the language model and the generation model. Targeting
embodied video prediction, we propose the Embodied Video Anticipator (EVA), a
unified framework aiming at video understanding and generation. EVA integrates
a video generation model with a visual language model, effectively combining
reasoning capabilities with high-quality generation. Moreover, to enhance the
generalization of our framework, we tailor-designed a multi-stage pretraining
paradigm that adaptatively ensembles LoRA to produce high-fidelity results.
Extensive experiments on EVA-Bench highlight the potential of EVA to
significantly improve performance in embodied scenes, paving the way for
large-scale pre-trained models in real-world prediction tasks.

[Paper Link](
https://arxiv.org/abs/2410.15461
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-45.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Diff-DAgger: Uncertainty Estimation with Diffusion Policy for Robotic Manipulation

- **Authors**: Sung-Wook Lee, Yen-Ling Kuo

#### Abstract

Recently, diffusion policy has shown impressive results in handling
multi-modal tasks in robotic manipulation. However, it has fundamental
limitations in out-of-distribution failures that persist due to compounding
errors and its limited capability to extrapolate. One way to address these
limitations is robot-gated DAgger, an interactive imitation learning with a
robot query system to actively seek expert help during policy rollout. While
robot-gated DAgger has high potential for learning at scale, existing methods
like Ensemble-DAgger struggle with highly expressive policies: They often
misinterpret policy disagreements as uncertainty at multi-modal decision
points. To address this problem, we introduce Diff-DAgger, an efficient
robot-gated DAgger algorithm that leverages the training objective of diffusion
policy. We evaluate Diff-DAgger across different robot tasks including
stacking, pushing, and plugging, and show that Diff-DAgger improves the task
failure prediction by 37%, the task completion rate by 14%, and reduces the
wall-clock time by up to 540%. We hope that this work opens up a path for
efficiently incorporating expressive yet data-hungry policies into interactive
robot learning settings.

[Paper Link](
https://arxiv.org/abs/2410.14868
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-43_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### A Novel Approach to Grasping Control of Soft Robotic Grippers based on Digital Twin

- **Authors**: Tianyi Xiang, Borui Li, Quan Zhang, Mark Leach, Eng Gee Lim

#### Abstract

This paper has proposed a Digital Twin (DT) framework for real-time motion
and pose control of soft robotic grippers. The developed DT is based on an
industrial robot workstation, integrated with our newly proposed approach for
soft gripper control, primarily based on computer vision, for setting the
driving pressure for desired gripper status in real-time. Knowing the gripper
motion, the gripper parameters (e.g. curvatures and bending angles, etc.) are
simulated by kinematics modelling in Unity 3D, which is based on four-piecewise
constant curvature kinematics. The mapping in between the driving pressure and
gripper parameters is achieved by implementing OpenCV based image processing
algorithms and data fitting. Results show that our DT-based approach can
achieve satisfactory performance in real-time control of soft gripper
manipulation, which can satisfy a wide range of industrial applications.

[Paper Link](
https://arxiv.org/abs/2410.14928
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-43.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Development of a Simple and Novel Digital Twin Framework for Industrial Robots in Intelligent robotics manufacturing

- **Authors**: Tianyi Xiang, Borui Li, Xin Pan, Quan Zhang

#### Abstract

This paper has proposed an easily replicable and novel approach for
developing a Digital Twin (DT) system for industrial robots in intelligent
manufacturing applications. Our framework enables effective communication via
Robot Web Service (RWS), while a real-time simulation is implemented in Unity
3D and Web-based Platform without any other 3rd party tools. The framework can
do real-time visualization and control of the entire work process, as well as
implement real-time path planning based on algorithms executed in MATLAB.
Results verify the high communication efficiency with a refresh rate of only
$17 ms$. Furthermore, our developed web-based platform and Graphical User
Interface (GUI) enable easy accessibility and user-friendliness in real-time
control.

[Paper Link](
https://arxiv.org/abs/2410.14934
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-42.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### MENTOR: Mixture-of-Experts Network with Task-Oriented Perturbation for Visual Reinforcement Learning

- **Authors**: Suning Huang, Zheyu Zhang, Tianhai Liang, Yihan Xu, Zhehao Kou, Chenhao Lu, Guowei Xu, Zhengrong Xue, Huazhe Xu

#### Abstract

Visual deep reinforcement learning (RL) enables robots to acquire skills from
visual input for unstructured tasks. However, current algorithms suffer from
low sample efficiency, limiting their practical applicability. In this work, we
present MENTOR, a method that improves both the architecture and optimization
of RL agents. Specifically, MENTOR replaces the standard multi-layer perceptron
(MLP) with a mixture-of-experts (MoE) backbone, enhancing the agent's ability
to handle complex tasks by leveraging modular expert learning to avoid gradient
conflicts. Furthermore, MENTOR introduces a task-oriented perturbation
mechanism, which heuristically samples perturbation candidates containing
task-relevant information, leading to more targeted and effective optimization.
MENTOR outperforms state-of-the-art methods across three simulation domains --
DeepMind Control Suite, Meta-World, and Adroit. Additionally, MENTOR achieves
an average of 83% success rate on three challenging real-world robotic
manipulation tasks including peg insertion, cable routing, and tabletop golf,
which significantly surpasses the success rate of 32% from the current
strongest model-free visual RL algorithm. These results underscore the
importance of sample efficiency in advancing visual RL for real-world robotics.
Experimental videos are available at
https://suninghuang19.github.io/mentor_page.

[Website Link](https://suninghuang19.github.io/mentor_page.)

[Paper Link](
https://arxiv.org/abs/2410.14972
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-41.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GRS: Generating Robotic Simulation Tasks from Real-World Images

- **Authors**: Alex Zook, Fan-Yun Sun, Josef Spjut, Valts Blukis, Stan Birchfield, Jonathan Tremblay

#### Abstract

We introduce GRS (Generating Robotic Simulation tasks), a novel system to
address the challenge of real-to-sim in robotics, computer vision, and AR/VR.
GRS enables the creation of digital twin simulations from single real-world
RGB-D observations, complete with diverse, solvable tasks for virtual agent
training. We use state-of-the-art vision-language models (VLMs) to achieve a
comprehensive real-to-sim pipeline. GRS operates in three stages: 1) scene
comprehension using SAM2 for object segmentation and VLMs for object
description, 2) matching identified objects with simulation-ready assets, and
3) generating contextually appropriate robotic tasks. Our approach ensures
simulations align with task specifications by generating test suites designed
to verify adherence to the task specification. We introduce a router that
iteratively refines the simulation and test code to ensure the simulation is
solvable by a robot policy while remaining aligned to the task specification.
Our experiments demonstrate the system's efficacy in accurately identifying
object correspondence, which allows us to generate task environments that
closely match input environments, and enhance automated simulation task
generation through our novel router mechanism.

[Paper Link](
https://arxiv.org/abs/2410.15536
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-38.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### MSGField: A Unified Scene Representation Integrating Motion, Semantics, and Geometry for Robotic Manipulation

- **Authors**: Yu Sheng, Runfeng Lin, Lidian Wang, Quecheng Qiu, YanYong Zhang, Yu Zhang, Bei Hua, Jianmin Ji

#### Abstract

Combining accurate geometry with rich semantics has been proven to be highly
effective for language-guided robotic manipulation. Existing methods for
dynamic scenes either fail to update in real-time or rely on additional depth
sensors for simple scene editing, limiting their applicability in real-world.
In this paper, we introduce MSGField, a representation that uses a collection
of 2D Gaussians for high-quality reconstruction, further enhanced with
attributes to encode semantic and motion information. Specially, we represent
the motion field compactly by decomposing each primitive's motion into a
combination of a limited set of motion bases. Leveraging the differentiable
real-time rendering of Gaussian splatting, we can quickly optimize object
motion, even for complex non-rigid motions, with image supervision from only
two camera views. Additionally, we designed a pipeline that utilizes object
priors to efficiently obtain well-defined semantics. In our challenging
dataset, which includes flexible and extremely small objects, our method
achieve a success rate of 79.2% in static and 63.3% in dynamic environments for
language-guided manipulation. For specified object grasping, we achieve a
success rate of 90%, on par with point cloud-based methods. Code and dataset
will be released at:https://shengyu724.github.io/MSGField.github.io.

[Website Link](https://shengyu724.github.io/MSGField.github.io.)

[Paper Link](
https://arxiv.org/abs/2410.15730
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-35.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Diffusion Transformer Policy

- **Authors**: Zhi Hou, Tianyi Zhang, Yuwen Xiong, Hengjun Pu, Chengyang Zhao, Ronglei Tong, Yu Qiao, Jifeng Dai, Yuntao Chen

#### Abstract

Recent large visual-language action models pretrained on diverse robot
datasets have demonstrated the potential for generalizing to new environments
with a few in-domain data. However, those approaches usually predict
discretized or continuous actions by a small action head, which limits the
ability in handling diverse action spaces. In contrast, we model the continuous
action with a large multi-modal diffusion transformer, dubbed as Diffusion
Transformer Policy, in which we directly denoise action chunks by a large
transformer model rather than a small action head. By leveraging the scaling
capability of transformers, the proposed approach can effectively model
continuous end-effector actions across large diverse robot datasets, and
achieve better generalization performance. Extensive experiments demonstrate
Diffusion Transformer Policy pretrained on diverse robot data can generalize to
different embodiments, including simulation environments like Maniskill2 and
Calvin, as well as the real-world Franka arm. Specifically, without bells and
whistles, the proposed approach achieves state-of-the-art performance with only
a single third-view camera stream in the Calvin novel task setting (ABC->D),
improving the average number of tasks completed in a row of 5 to 3.6, and the
pretraining stage significantly facilitates the success sequence length on the
Calvin by over 1.2. The code will be publicly available.

[Paper Link](
https://arxiv.org/abs/2410.15959
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-23_18-32.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-21


### Graph Optimality-Aware Stochastic LiDAR Bundle Adjustment with Progressive Spatial Smoothing

- **Authors**: Jianping Li, Thien-Minh Nguyen, Muqing Cao, Shenghai Yuan, Tzu-Yi Hung, Lihua Xie

#### Abstract

Large-scale LiDAR Bundle Adjustment (LBA) for refining sensor orientation and
point cloud accuracy simultaneously is a fundamental task in photogrammetry and
robotics, particularly as low-cost 3D sensors are increasingly used for 3D
mapping in complex scenes. Unlike pose-graph-based methods that rely solely on
pairwise relationships between LiDAR frames, LBA leverages raw LiDAR
correspondences to achieve more precise results, especially when initial pose
estimates are unreliable for low-cost sensors. However, existing LBA methods
face challenges such as simplistic planar correspondences, extensive
observations, and dense normal matrices in the least-squares problem, which
limit robustness, efficiency, and scalability. To address these issues, we
propose a Graph Optimality-aware Stochastic Optimization scheme with
Progressive Spatial Smoothing, namely PSS-GOSO, to achieve \textit{robust},
\textit{efficient}, and \textit{scalable} LBA. The Progressive Spatial
Smoothing (PSS) module extracts \textit{robust} LiDAR feature association
exploiting the prior structure information obtained by the polynomial smooth
kernel. The Graph Optimality-aware Stochastic Optimization (GOSO) module first
sparsifies the graph according to optimality for an \textit{efficient}
optimization. GOSO then utilizes stochastic clustering and graph
marginalization to solve the large-scale state estimation problem for a
\textit{scalable} LBA. We validate PSS-GOSO across diverse scenes captured by
various platforms, demonstrating its superior performance compared to existing
methods.

[Paper Link](
https://arxiv.org/abs/2410.14565
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-54.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-18


### ALOHA Unleashed: A Simple Recipe for Robot Dexterity

- **Authors**: Tony Z. Zhao, Jonathan Tompson, Danny Driess, Pete Florence, Kamyar Ghasemipour, Chelsea Finn, Ayzaan Wahid

#### Abstract

Recent work has shown promising results for learning end-to-end robot
policies using imitation learning. In this work we address the question of how
far can we push imitation learning for challenging dexterous manipulation
tasks. We show that a simple recipe of large scale data collection on the ALOHA
2 platform, combined with expressive models such as Diffusion Policies, can be
effective in learning challenging bimanual manipulation tasks involving
deformable objects and complex contact rich dynamics. We demonstrate our recipe
on 5 challenging real-world and 3 simulated tasks and demonstrate improved
performance over state-of-the-art baselines. The project website and videos can
be found at aloha-unleashed.github.io.

[Paper Link](
https://arxiv.org/abs/2410.13126
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-48_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Interactive Navigation with Adaptive Non-prehensile Mobile Manipulation

- **Authors**: Cunxi Dai, Xiaohan Liu, Koushil Sreenath, Zhongyu Li, Ralph Hollis

#### Abstract

This paper introduces a framework for interactive navigation through adaptive
non-prehensile mobile manipulation. A key challenge in this process is handling
objects with unknown dynamics, which are difficult to infer from visual
observation. To address this, we propose an adaptive dynamics model for common
movable indoor objects via learned SE(2) dynamics representations. This model
is integrated into Model Predictive Path Integral (MPPI) control to guide the
robot's interactions. Additionally, the learned dynamics help inform
decision-making when navigating around objects that cannot be manipulated.Our
approach is validated in both simulation and real-world scenarios,
demonstrating its ability to accurately represent object dynamics and
effectively manipulate various objects. We further highlight its success in the
Navigation Among Movable Objects (NAMO) task by deploying the proposed
framework on a dynamically balancing mobile robot, Shmoobot. Project website:
https://cmushmoobot.github.io/AdaptivePushing/.

[Website Link](https://cmushmoobot.github.io/AdaptivePushing/.)

[Paper Link](
https://arxiv.org/abs/2410.13418
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-48.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### State Estimation Transformers for Agile Legged Locomotion

- **Authors**: Chen Yu, Yichu Yang, Tianlin Liu, Yangwei You, Mingliang Zhou, Diyun Xiang

#### Abstract

We propose a state estimation method that can accurately predict the robot's
privileged states to push the limits of quadruped robots in executing advanced
skills such as jumping in the wild. In particular, we present the State
Estimation Transformers (SET), an architecture that casts the state estimation
problem as conditional sequence modeling. SET outputs the robot states that are
hard to obtain directly in the real world, such as the body height and
velocities, by leveraging a causally masked Transformer. By conditioning an
autoregressive model on the robot's past states, our SET model can predict
these privileged observations accurately even in highly dynamic locomotions. We
evaluate our methods on three tasks -- running jumping, running backflipping,
and running sideslipping -- on a low-cost quadruped robot, Cyberdog2. Results
show that SET can outperform other methods in estimation accuracy and
transferability in the simulation as well as success rates of jumping and
triggering a recovery controller in the real world, suggesting the superiority
of such a Transformer-based explicit state estimator in highly dynamic
locomotion tasks.

[Paper Link](
https://arxiv.org/abs/2410.13496
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-47.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Preference Aligned Diffusion Planner for Quadrupedal Locomotion Control

- **Authors**: Xinyi Yuan, Zhiwei Shang, Zifan Wang, Chenkai Wang, Zhao Shan, Zhenchao Qi, Meixin Zhu, Chenjia Bai, Xuelong Li

#### Abstract

Diffusion models demonstrate superior performance in capturing complex
distributions from large-scale datasets, providing a promising solution for
quadrupedal locomotion control. However, offline policy is sensitive to
Out-of-Distribution (OOD) states due to the limited state coverage in the
datasets. In this work, we propose a two-stage learning framework combining
offline learning and online preference alignment for legged locomotion control.
Through the offline stage, the diffusion planner learns the joint distribution
of state-action sequences from expert datasets without using reward labels.
Subsequently, we perform the online interaction in the simulation environment
based on the trained offline planer, which significantly addresses the OOD
issues and improves the robustness. Specifically, we propose a novel weak
preference labeling method without the ground-truth reward or human
preferences. The proposed method exhibits superior stability and velocity
tracking accuracy in pacing, trotting, and bounding gait under both slow- and
high-speed scenarios and can perform zero-shot transfer to the real Unitree Go1
robots. The project website for this paper is at
https://shangjaven.github.io/preference-aligned-diffusion-legged/.

[Website Link](https://shangjaven.github.io/preference-aligned-diffusion-legged/.)

[Paper Link](
https://arxiv.org/abs/2410.13586
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-46.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Jailbreaking LLM-Controlled Robots

- **Authors**: Alexander Robey, Zachary Ravichandran, Vijay Kumar, Hamed Hassani, George J. Pappas

#### Abstract

The recent introduction of large language models (LLMs) has revolutionized
the field of robotics by enabling contextual reasoning and intuitive
human-robot interaction in domains as varied as manipulation, locomotion, and
self-driving vehicles. When viewed as a stand-alone technology, LLMs are known
to be vulnerable to jailbreaking attacks, wherein malicious prompters elicit
harmful text by bypassing LLM safety guardrails. To assess the risks of
deploying LLMs in robotics, in this paper, we introduce RoboPAIR, the first
algorithm designed to jailbreak LLM-controlled robots. Unlike existing, textual
attacks on LLM chatbots, RoboPAIR elicits harmful physical actions from
LLM-controlled robots, a phenomenon we experimentally demonstrate in three
scenarios: (i) a white-box setting, wherein the attacker has full access to the
NVIDIA Dolphins self-driving LLM, (ii) a gray-box setting, wherein the attacker
has partial access to a Clearpath Robotics Jackal UGV robot equipped with a
GPT-4o planner, and (iii) a black-box setting, wherein the attacker has only
query access to the GPT-3.5-integrated Unitree Robotics Go2 robot dog. In each
scenario and across three new datasets of harmful robotic actions, we
demonstrate that RoboPAIR, as well as several static baselines, finds
jailbreaks quickly and effectively, often achieving 100% attack success rates.
Our results reveal, for the first time, that the risks of jailbroken LLMs
extend far beyond text generation, given the distinct possibility that
jailbroken robots could cause physical damage in the real world. Indeed, our
results on the Unitree Go2 represent the first successful jailbreak of a
deployed commercial robotic system. Addressing this emerging vulnerability is
critical for ensuring the safe deployment of LLMs in robotics. Additional media
is available at: https://robopair.org

[Website Link](https://robopair.org)

[Paper Link](
https://arxiv.org/abs/2410.13691
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-45.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Differentiable Robot Rendering

- **Authors**: Ruoshi Liu, Alper Canberk, Shuran Song, Carl Vondrick

#### Abstract

Vision foundation models trained on massive amounts of visual data have shown
unprecedented reasoning and planning skills in open-world settings. A key
challenge in applying them to robotic tasks is the modality gap between visual
data and action data. We introduce differentiable robot rendering, a method
allowing the visual appearance of a robot body to be directly differentiable
with respect to its control parameters. Our model integrates a kinematics-aware
deformable model and Gaussians Splatting and is compatible with any robot form
factors and degrees of freedom. We demonstrate its capability and usage in
applications including reconstruction of robot poses from images and
controlling robots through vision language models. Quantitative and qualitative
results show that our differentiable rendering model provides effective
gradients for robotic control directly from pixels, setting the foundation for
the future applications of vision foundation models in robotics.

[Paper Link](
https://arxiv.org/abs/2410.13851
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-44.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-17


### Dynamic Open-Vocabulary 3D Scene Graphs for Long-term Language-Guided Mobile Manipulation

- **Authors**: Zhijie Yan, Shufei Li, Zuoxu Wang, Lixiu Wu, Han Wang, Jun Zhu, Lijiang Chen, Jihong Liu

#### Abstract

Enabling mobile robots to perform long-term tasks in dynamic real-world
environments is a formidable challenge, especially when the environment changes
frequently due to human-robot interactions or the robot's own actions.
Traditional methods typically assume static scenes, which limits their
applicability in the continuously changing real world. To overcome these
limitations, we present DovSG, a novel mobile manipulation framework that
leverages dynamic open-vocabulary 3D scene graphs and a language-guided task
planning module for long-term task execution. DovSG takes RGB-D sequences as
input and utilizes vision-language models (VLMs) for object detection to obtain
high-level object semantic features. Based on the segmented objects, a
structured 3D scene graph is generated for low-level spatial relationships.
Furthermore, an efficient mechanism for locally updating the scene graph,
allows the robot to adjust parts of the graph dynamically during interactions
without the need for full scene reconstruction. This mechanism is particularly
valuable in dynamic environments, enabling the robot to continually adapt to
scene changes and effectively support the execution of long-term tasks. We
validated our system in real-world environments with varying degrees of manual
modifications, demonstrating its effectiveness and superior performance in
long-term tasks. Our project page is available at:
https://BJHYZJ.github.io/DoviSG.

[Website Link](https://BJHYZJ.github.io/DoviSG.)

[Paper Link](
https://arxiv.org/abs/2410.11989
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-42.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### In-Context Learning Enables Robot Action Prediction in LLMs

- **Authors**: Yida Yin, Zekai Wang, Yuvan Sharma, Dantong Niu, Trevor Darrell, Roei Herzig

#### Abstract

Recently, Large Language Models (LLMs) have achieved remarkable success using
in-context learning (ICL) in the language domain. However, leveraging the ICL
capabilities within LLMs to directly predict robot actions remains largely
unexplored. In this paper, we introduce RoboPrompt, a framework that enables
off-the-shelf text-only LLMs to directly predict robot actions through ICL
without training. Our approach first heuristically identifies keyframes that
capture important moments from an episode. Next, we extract end-effector
actions from these keyframes as well as the estimated initial object poses, and
both are converted into textual descriptions. Finally, we construct a
structured template to form ICL demonstrations from these textual descriptions
and a task instruction. This enables an LLM to directly predict robot actions
at test time. Through extensive experiments and analysis, RoboPrompt shows
stronger performance over zero-shot and ICL baselines in simulated and
real-world settings.

[Paper Link](
https://arxiv.org/abs/2410.12782
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-35.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Harmon: Whole-Body Motion Generation of Humanoid Robots from Language Descriptions

- **Authors**: Zhenyu Jiang, Yuqi Xie, Jinhan Li, Ye Yuan, Yifeng Zhu, Yuke Zhu

#### Abstract

Humanoid robots, with their human-like embodiment, have the potential to
integrate seamlessly into human environments. Critical to their coexistence and
cooperation with humans is the ability to understand natural language
communications and exhibit human-like behaviors. This work focuses on
generating diverse whole-body motions for humanoid robots from language
descriptions. We leverage human motion priors from extensive human motion
datasets to initialize humanoid motions and employ the commonsense reasoning
capabilities of Vision Language Models (VLMs) to edit and refine these motions.
Our approach demonstrates the capability to produce natural, expressive, and
text-aligned humanoid motions, validated through both simulated and real-world
experiments. More videos can be found at
https://ut-austin-rpl.github.io/Harmon/.

[Website Link](https://ut-austin-rpl.github.io/Harmon/.)

[Paper Link](
https://arxiv.org/abs/2410.12773
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-34.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-16


### Visual Manipulation with Legs

- **Authors**: Xialin He, Chengjing Yuan, Wenxuan Zhou, Ruihan Yang, David Held, Xiaolong Wang

#### Abstract

Animals use limbs for both locomotion and manipulation. We aim to equip
quadruped robots with similar versatility. This work introduces a system that
enables quadruped robots to interact with objects using their legs, inspired by
non-prehensile manipulation. The system has two main components: a visual
manipulation policy module and a loco-manipulator module. The visual
manipulation policy, trained with reinforcement learning (RL) using point cloud
observations and object-centric actions, decides how the leg should interact
with the object. The loco-manipulator controller manages leg movements and body
pose adjustments, based on impedance control and Model Predictive Control
(MPC). Besides manipulating objects with a single leg, the system can select
from the left or right leg based on critic maps and move objects to distant
goals through base adjustment. Experiments evaluate the system on object pose
alignment tasks in both simulation and the real world, demonstrating more
versatile object manipulation skills with legs than previous work. Videos can
be found at https://legged-manipulation.github.io/

[Website Link](https://legged-manipulation.github.io/)

[Paper Link](
https://arxiv.org/abs/2410.11345
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-33.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GSORB-SLAM: Gaussian Splatting SLAM benefits from ORB features and Transmittance information

- **Authors**: Wancai Zheng, Xinyi Yu, Jintao Rong, Linlin Ou, Yan Wei, Libo Zhou

#### Abstract

The emergence of 3D Gaussian Splatting (3DGS) has recently sparked a renewed
wave of dense visual SLAM research. However, current methods face challenges
such as sensitivity to artifacts and noise, sub-optimal selection of training
viewpoints, and a lack of light global optimization. In this paper, we propose
a dense SLAM system that tightly couples 3DGS with ORB features. We design a
joint optimization approach for robust tracking and effectively reducing the
impact of noise and artifacts. This involves combining novel geometric
observations, derived from accumulated transmittance, with ORB features
extracted from pixel data. Furthermore, to improve mapping quality, we propose
an adaptive Gaussian expansion and regularization method that enables Gaussian
primitives to represent the scene compactly. This is coupled with a viewpoint
selection strategy based on the hybrid graph to mitigate over-fitting effects
and enhance convergence quality. Finally, our approach achieves compact and
high-quality scene representations and accurate localization. GSORB-SLAM has
been evaluated on different datasets, demonstrating outstanding performance.
The code will be available.

[Paper Link](
https://arxiv.org/abs/2410.11356
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-32.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### PAVLM: Advancing Point Cloud based Affordance Understanding Via Vision-Language Model

- **Authors**: Shang-Ching Liu, Van Nhiem Tran, Wenkai Chen, Wei-Lun Cheng, Yen-Lin Huang, I-Bin Liao, Yung-Hui Li, Jianwei Zhang

#### Abstract

Affordance understanding, the task of identifying actionable regions on 3D
objects, plays a vital role in allowing robotic systems to engage with and
operate within the physical world. Although Visual Language Models (VLMs) have
excelled in high-level reasoning and long-horizon planning for robotic
manipulation, they still fall short in grasping the nuanced physical properties
required for effective human-robot interaction. In this paper, we introduce
PAVLM (Point cloud Affordance Vision-Language Model), an innovative framework
that utilizes the extensive multimodal knowledge embedded in pre-trained
language models to enhance 3D affordance understanding of point cloud. PAVLM
integrates a geometric-guided propagation module with hidden embeddings from
large language models (LLMs) to enrich visual semantics. On the language side,
we prompt Llama-3.1 models to generate refined context-aware text, augmenting
the instructional input with deeper semantic cues. Experimental results on the
3D-AffordanceNet benchmark demonstrate that PAVLM outperforms baseline methods
for both full and partial point clouds, particularly excelling in its
generalization to novel open-world affordance tasks of 3D objects. For more
information, visit our project site: pavlm-source.github.io.

[Paper Link](
https://arxiv.org/abs/2410.11564
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-30.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### SDS -- See it, Do it, Sorted: Quadruped Skill Synthesis from Single Video Demonstration

- **Authors**: Jeffrey Li, Maria Stamatopoulou, Dimitrios Kanoulas

#### Abstract

In this paper, we present SDS (``See it. Do it. Sorted.''), a novel pipeline
for intuitive quadrupedal skill learning from a single demonstration video.
Leveraging the Visual capabilities of GPT-4o, SDS processes input videos
through our novel chain-of-thought promoting technique (SUS) and generates
executable reward functions (RFs) that drive the imitation of locomotion
skills, through learning a Proximal Policy Optimization (PPO)-based
Reinforcement Learning (RL) policy, using environment information from the
NVIDIA IsaacGym simulator. SDS autonomously evaluates the RFs by monitoring the
individual reward components and supplying training footage and fitness metrics
back into GPT-4o, which is then prompted to evolve the RFs to achieve higher
task fitness at each iteration. We validate our method on the Unitree Go1
robot, demonstrating its ability to execute variable skills such as trotting,
bounding, pacing and hopping, achieving high imitation fidelity and locomotion
stability. SDS shows improvements over SOTA methods in task adaptability,
reduced dependence on domain-specific knowledge, and bypassing the need for
labor-intensive reward engineering and large-scale training datasets.
Additional information and the open-sourced code can be found in:
https://rpl-cs-ucl.github.io/SDSweb

[Website Link](https://rpl-cs-ucl.github.io/SDSweb)

[Paper Link](
https://arxiv.org/abs/2410.11571
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-29_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### DeformPAM: Data-Efficient Learning for Long-horizon Deformable Object Manipulation via Preference-based Action Alignment

- **Authors**: Wendi Chen, Han Xue, Fangyuan Zhou, Yuan Fang, Cewu Lu

#### Abstract

In recent years, imitation learning has made progress in the field of robotic
manipulation. However, it still faces challenges when dealing with complex
long-horizon deformable object tasks, such as high-dimensional state spaces,
complex dynamics, and multimodal action distributions. Traditional imitation
learning methods often require a large amount of data and encounter
distributional shifts and accumulative errors in these tasks. To address these
issues, we propose a data-efficient general learning framework (DeformPAM)
based on preference learning and reward-guided action selection. DeformPAM
decomposes long-horizon tasks into multiple action primitives, utilizes 3D
point cloud inputs and diffusion models to model action distributions, and
trains an implicit reward model using human preference data. During the
inference phase, the reward model scores multiple candidate actions, selecting
the optimal action for execution, thereby reducing the occurrence of anomalous
actions and improving task completion quality. Experiments conducted on three
challenging real-world long-horizon deformable object manipulation tasks
demonstrate the effectiveness of this method. Results show that DeformPAM
improves both task completion quality and efficiency compared to baseline
methods even with limited data. Code and data will be available at
https://deform-pam.robotflow.ai.

[Website Link](https://deform-pam.robotflow.ai.)

[Paper Link](
https://arxiv.org/abs/2410.11584
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-29.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Robust Manipulation Primitive Learning via Domain Contraction

- **Authors**: Teng Xue, Amirreza Razmjoo, Suhan Shetty, Sylvain Calinon

#### Abstract

Contact-rich manipulation plays an important role in human daily activities,
but uncertain parameters pose significant challenges for robots to achieve
comparable performance through planning and control. To address this issue,
domain adaptation and domain randomization have been proposed for robust policy
learning. However, they either lose the generalization ability across diverse
instances or perform conservatively due to neglecting instance-specific
information. In this paper, we propose a bi-level approach to learn robust
manipulation primitives, including parameter-augmented policy learning using
multiple models, and parameter-conditioned policy retrieval through domain
contraction. This approach unifies domain randomization and domain adaptation,
providing optimal behaviors while keeping generalization ability. We validate
the proposed method on three contact-rich manipulation primitives: hitting,
pushing, and reorientation. The experimental results showcase the superior
performance of our approach in generating robust policies for instances with
diverse physical parameters.

[Paper Link](
https://arxiv.org/abs/2410.11600
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-28.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Latent Action Pretraining from Videos

- **Authors**: Seonghyeon Ye, Joel Jang, Byeongguk Jeon, Sejune Joo, Jianwei Yang, Baolin Peng, Ajay Mandlekar, Reuben Tan, Yu-Wei Chao, Bill Yuchen Lin, Lars Liden, Kimin Lee, Jianfeng Gao, Luke Zettlemoyer, Dieter Fox, Minjoon Seo

#### Abstract

We introduce Latent Action Pretraining for general Action models (LAPA), an
unsupervised method for pretraining Vision-Language-Action (VLA) models without
ground-truth robot action labels. Existing Vision-Language-Action models
require action labels typically collected by human teleoperators during
pretraining, which significantly limits possible data sources and scale. In
this work, we propose a method to learn from internet-scale videos that do not
have robot action labels. We first train an action quantization model
leveraging VQ-VAE-based objective to learn discrete latent actions between
image frames, then pretrain a latent VLA model to predict these latent actions
from observations and task descriptions, and finally finetune the VLA on
small-scale robot manipulation data to map from latent to robot actions.
Experimental results demonstrate that our method significantly outperforms
existing techniques that train robot manipulation policies from large-scale
videos. Furthermore, it outperforms the state-of-the-art VLA model trained with
robotic action labels on real-world manipulation tasks that require language
conditioning, generalization to unseen objects, and semantic generalization to
unseen instructions. Training only on human manipulation videos also shows
positive transfer, opening up the potential for leveraging web-scale data for
robotics foundation model.

[Paper Link](
https://arxiv.org/abs/2410.11758
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-27.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### OKAMI: Teaching Humanoid Robots Manipulation Skills through Single Video Imitation

- **Authors**: Jinhan Li, Yifeng Zhu, Yuqi Xie, Zhenyu Jiang, Mingyo Seo, Georgios Pavlakos, Yuke Zhu

#### Abstract

We study the problem of teaching humanoid robots manipulation skills by
imitating from single video demonstrations. We introduce OKAMI, a method that
generates a manipulation plan from a single RGB-D video and derives a policy
for execution. At the heart of our approach is object-aware retargeting, which
enables the humanoid robot to mimic the human motions in an RGB-D video while
adjusting to different object locations during deployment. OKAMI uses
open-world vision models to identify task-relevant objects and retarget the
body motions and hand poses separately. Our experiments show that OKAMI
achieves strong generalizations across varying visual and spatial conditions,
outperforming the state-of-the-art baseline on open-world imitation from
observation. Furthermore, OKAMI rollout trajectories are leveraged to train
closed-loop visuomotor policies, which achieve an average success rate of 79.2%
without the need for labor-intensive teleoperation. More videos can be found on
our website https://ut-austin-rpl.github.io/OKAMI/.

[Website Link](https://ut-austin-rpl.github.io/OKAMI/.)

[Paper Link](
https://arxiv.org/abs/2410.11792
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-26.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Learning Smooth Humanoid Locomotion through Lipschitz-Constrained Policies

- **Authors**: Zixuan Chen, Xialin He, Yen-Jen Wang, Qiayuan Liao, Yanjie Ze, Zhongyu Li, S. Shankar Sastry, Jiajun Wu, Koushil Sreenath, Saurabh Gupta, Xue Bin Peng

#### Abstract

Reinforcement learning combined with sim-to-real transfer offers a general
framework for developing locomotion controllers for legged robots. To
facilitate successful deployment in the real world, smoothing techniques, such
as low-pass filters and smoothness rewards, are often employed to develop
policies with smooth behaviors. However, because these techniques are
non-differentiable and usually require tedious tuning of a large set of
hyperparameters, they tend to require extensive manual tuning for each robotic
platform. To address this challenge and establish a general technique for
enforcing smooth behaviors, we propose a simple and effective method that
imposes a Lipschitz constraint on a learned policy, which we refer to as
Lipschitz-Constrained Policies (LCP). We show that the Lipschitz constraint can
be implemented in the form of a gradient penalty, which provides a
differentiable objective that can be easily incorporated with automatic
differentiation frameworks. We demonstrate that LCP effectively replaces the
need for smoothing rewards or low-pass filters and can be easily integrated
into training frameworks for many distinct humanoid robots. We extensively
evaluate LCP in both simulation and real-world humanoid robots, producing
smooth and robust locomotion controllers. All simulation and deployment code,
along with complete checkpoints, is available on our project page:
https://lipschitz-constrained-policy.github.io.

[Website Link](https://lipschitz-constrained-policy.github.io.)

[Paper Link](
https://arxiv.org/abs/2410.11825
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-25.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-15


### Traversability-Aware Legged Navigation by Learning from Real-World Visual Data

- **Authors**: Hongbo Zhang, Zhongyu Li, Xuanqi Zeng, Laura Smith, Kyle Stachowicz, Dhruv Shah, Linzhu Yue, Zhitao Song, Weipeng Xia, Sergey Levine, Koushil Sreenath, Yun-hui Liu

#### Abstract

The enhanced mobility brought by legged locomotion empowers quadrupedal
robots to navigate through complex and unstructured environments. However,
optimizing agile locomotion while accounting for the varying energy costs of
traversing different terrains remains an open challenge. Most previous work
focuses on planning trajectories with traversability cost estimation based on
human-labeled environmental features. However, this human-centric approach is
insufficient because it does not account for the varying capabilities of the
robot locomotion controllers over challenging terrains. To address this, we
develop a novel traversability estimator in a robot-centric manner, based on
the value function of the robot's locomotion controller. This estimator is
integrated into a new learning-based RGBD navigation framework. The framework
develops a planner that guides the robot in avoiding obstacles and
hard-to-traverse terrains while reaching its goals. The training of the
navigation planner is directly performed in the real world using a sample
efficient reinforcement learning method. Through extensive benchmarking, we
demonstrate that the proposed framework achieves the best performance in
accurate traversability cost estimation and efficient learning from multi-modal
data (the robot's color and depth vision, and proprioceptive feedback) for
real-world training. Using the proposed method, a quadrupedal robot learns to
perform traversability-aware navigation through trial and error in various
real-world environments with challenging terrains that are difficult to
classify using depth vision alone.

[Paper Link](
https://arxiv.org/abs/2410.10621
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-21.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Generalizable Humanoid Manipulation with Improved 3D Diffusion Policies

- **Authors**: Yanjie Ze, Zixuan Chen, Wenhao Wang, Tianyi Chen, Xialin He, Ying Yuan, Xue Bin Peng, Jiajun Wu

#### Abstract

Humanoid robots capable of autonomous operation in diverse environments have
long been a goal for roboticists. However, autonomous manipulation by humanoid
robots has largely been restricted to one specific scene, primarily due to the
difficulty of acquiring generalizable skills. Recent advances in 3D visuomotor
policies, such as the 3D Diffusion Policy (DP3), have shown promise in
extending these capabilities to wilder environments. However, 3D visuomotor
policies often rely on camera calibration and point-cloud segmentation, which
present challenges for deployment on mobile robots like humanoids. In this
work, we introduce the Improved 3D Diffusion Policy (iDP3), a novel 3D
visuomotor policy that eliminates these constraints by leveraging egocentric 3D
visual representations. We demonstrate that iDP3 enables a full-sized humanoid
robot to autonomously perform skills in diverse real-world scenarios, using
only data collected in the lab. Videos are available at:
https://humanoid-manipulation.github.io

[Website Link](https://humanoid-manipulation.github.io)

[Paper Link](
https://arxiv.org/abs/2410.10803
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-19.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-14


### FusionSense: Bridging Common Sense, Vision, and Touch for Robust Sparse-View Reconstruction

- **Authors**: Irving Fang, Kairui Shi, Xujin He, Siqi Tan, Yifan Wang, Hanwen Zhao, Hung-Jui Huang, Wenzhen Yuan, Chen Feng, Jing Zhang

#### Abstract

Humans effortlessly integrate common-sense knowledge with sensory input from
vision and touch to understand their surroundings. Emulating this capability,
we introduce FusionSense, a novel 3D reconstruction framework that enables
robots to fuse priors from foundation models with highly sparse observations
from vision and tactile sensors. FusionSense addresses three key challenges:
(i) How can robots efficiently acquire robust global shape information about
the surrounding scene and objects? (ii) How can robots strategically select
touch points on the object using geometric and common-sense priors? (iii) How
can partial observations such as tactile signals improve the overall
representation of the object? Our framework employs 3D Gaussian Splatting as a
core representation and incorporates a hierarchical optimization strategy
involving global structure construction, object visual hull pruning and local
geometric constraints. This advancement results in fast and robust perception
in environments with traditionally challenging objects that are transparent,
reflective, or dark, enabling more downstream manipulation or navigation tasks.
Experiments on real-world data suggest that our framework outperforms
previously state-of-the-art sparse-view methods. All code and data are
open-sourced on the project website.

[Paper Link](
https://arxiv.org/abs/2410.08282
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-18.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Guiding Collision-Free Humanoid Multi-Contact Locomotion using Convex Kinematic Relaxations and Dynamic Optimization

- **Authors**: Carlos Gonzalez, Luis Sentis

#### Abstract

Humanoid robots rely on multi-contact planners to navigate a diverse set of
environments, including those that are unstructured and highly constrained. To
synthesize stable multi-contact plans within a reasonable time frame, most
planners assume statically stable motions or rely on reduced order models.
However, these approaches can also render the problem infeasible in the
presence of large obstacles or when operating near kinematic and dynamic
limits. To that end, we propose a new multi-contact framework that leverages
recent advancements in relaxing collision-free path planning into a convex
optimization problem, extending it to be applicable to humanoid multi-contact
navigation. Our approach generates near-feasible trajectories used as guides in
a dynamic trajectory optimizer, altogether addressing the aforementioned
limitations. We evaluate our computational approach showcasing three
different-sized humanoid robots traversing a high-raised naval knee-knocker
door using our proposed framework in simulation. Our approach can generate
motion plans within a few seconds consisting of several multi-contact states,
including dynamic feasibility in joint space.

[Paper Link](
https://arxiv.org/abs/2410.08335
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-17.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Aerial Vision-and-Language Navigation via Semantic-Topo-Metric Representation Guided LLM Reasoning

- **Authors**: Yunpeng Gao, Zhigang Wang, Linglin Jing, Dong Wang, Xuelong Li, Bin Zhao

#### Abstract

Aerial Vision-and-Language Navigation (VLN) is a novel task enabling Unmanned
Aerial Vehicles (UAVs) to navigate in outdoor environments through natural
language instructions and visual cues. It remains challenging due to the
complex spatial relationships in outdoor aerial scenes. In this paper, we
propose an end-to-end zero-shot framework for aerial VLN tasks, where the large
language model (LLM) is introduced as our agent for action prediction.
Specifically, we develop a novel Semantic-Topo-Metric Representation (STMR) to
enhance the spatial reasoning ability of LLMs. This is achieved by extracting
and projecting instruction-related semantic masks of landmarks into a top-down
map that contains the location information of surrounding landmarks. Further,
this map is transformed into a matrix representation with distance metrics as
the text prompt to the LLM, for action prediction according to the instruction.
Experiments conducted in real and simulation environments have successfully
proved the effectiveness and robustness of our method, achieving 15.9% and
12.5% improvements (absolute) in Oracle Success Rate (OSR) on AerialVLN-S
dataset.

[Paper Link](
https://arxiv.org/abs/2410.08500
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-16.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### SegGrasp: Zero-Shot Task-Oriented Grasping via Semantic and Geometric Guided Segmentation

- **Authors**: Haosheng Li, Weixin Mao, Weipeng Deng, Chenyu Meng, Rui Zhang, Fan Jia, Tiancai Wang, Haoqiang Fan, Hongan Wang, Xiaoming Deng

#### Abstract

Task-oriented grasping, which involves grasping specific parts of objects
based on their functions, is crucial for developing advanced robotic systems
capable of performing complex tasks in dynamic environments. In this paper, we
propose a training-free framework that incorporates both semantic and geometric
priors for zero-shot task-oriented grasp generation. The proposed framework,
SegGrasp, first leverages the vision-language models like GLIP for coarse
segmentation. It then uses detailed geometric information from convex
decomposition to improve segmentation quality through a fusion policy named
GeoFusion. An effective grasp pose can be generated by a grasping network with
improved segmentation. We conducted the experiments on both segmentation
benchmark and real-world robot grasping. The experimental results show that
SegGrasp surpasses the baseline by more than 15\% in grasp and segmentation
performance.

[Paper Link](
https://arxiv.org/abs/2410.08901
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-14.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-11


### SPA: 3D Spatial-Awareness Enables Effective Embodied Representation

- **Authors**: Haoyi Zhu, Honghui Yang, Yating Wang, Jiange Yang, Limin Wang, Tong He

#### Abstract

In this paper, we introduce SPA, a novel representation learning framework
that emphasizes the importance of 3D spatial awareness in embodied AI. Our
approach leverages differentiable neural rendering on multi-view images to
endow a vanilla Vision Transformer (ViT) with intrinsic spatial understanding.
We present the most comprehensive evaluation of embodied representation
learning to date, covering 268 tasks across 8 simulators with diverse policies
in both single-task and language-conditioned multi-task scenarios. The results
are compelling: SPA consistently outperforms more than 10 state-of-the-art
representation methods, including those specifically designed for embodied AI,
vision-centric tasks, and multi-modal applications, while using less training
data. Furthermore, we conduct a series of real-world experiments to confirm its
effectiveness in practical scenarios. These results highlight the critical role
of 3D spatial awareness for embodied representation learning. Our strongest
model takes more than 6000 GPU hours to train and we are committed to
open-sourcing all code and model weights to foster future research in embodied
representation learning. Project Page: https://haoyizhu.github.io/spa/.

[Website Link](https://haoyizhu.github.io/spa/.)

[Paper Link](
https://arxiv.org/abs/2410.08208
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-10.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation

- **Authors**: Songming Liu, Lingxuan Wu, Bangguo Li, Hengkai Tan, Huayu Chen, Zhengyi Wang, Ke Xu, Hang Su, Jun Zhu

#### Abstract

Bimanual manipulation is essential in robotics, yet developing foundation
models is extremely challenging due to the inherent complexity of coordinating
two robot arms (leading to multi-modal action distributions) and the scarcity
of training data. In this paper, we present the Robotics Diffusion Transformer
(RDT), a pioneering diffusion foundation model for bimanual manipulation. RDT
builds on diffusion models to effectively represent multi-modality, with
innovative designs of a scalable Transformer to deal with the heterogeneity of
multi-modal inputs and to capture the nonlinearity and high frequency of
robotic data. To address data scarcity, we further introduce a Physically
Interpretable Unified Action Space, which can unify the action representations
of various robots while preserving the physical meanings of original actions,
facilitating learning transferrable physical knowledge. With these designs, we
managed to pre-train RDT on the largest collection of multi-robot datasets to
date and scaled it up to 1.2B parameters, which is the largest diffusion-based
foundation model for robotic manipulation. We finally fine-tuned RDT on a
self-created multi-task bimanual dataset with over 6K+ episodes to refine its
manipulation capabilities. Experiments on real robots demonstrate that RDT
significantly outperforms existing methods. It exhibits zero-shot
generalization to unseen objects and scenes, understands and follows language
instructions, learns new skills with just 1~5 demonstrations, and effectively
handles complex, dexterous tasks. We refer to
https://rdt-robotics.github.io/rdt-robotics/ for the code and videos.

[Website Link](https://rdt-robotics.github.io/rdt-robotics/)

[Paper Link](
https://arxiv.org/abs/2410.07864
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-06.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Dynamic Object Catching with Quadruped Robot Front Legs

- **Authors**: André Schakkal, Guillaume Bellegarda, Auke Ijspeert

#### Abstract

This paper presents a framework for dynamic object catching using a quadruped
robot's front legs while it stands on its rear legs. The system integrates
computer vision, trajectory prediction, and leg control to enable the quadruped
to visually detect, track, and successfully catch a thrown object using an
onboard camera. Leveraging a fine-tuned YOLOv8 model for object detection and a
regression-based trajectory prediction module, the quadruped adapts its front
leg positions iteratively to anticipate and intercept the object. The catching
maneuver involves identifying the optimal catching position, controlling the
front legs with Cartesian PD control, and closing the legs together at the
right moment. We propose and validate three different methods for selecting the
optimal catching position: 1) intersecting the predicted trajectory with a
vertical plane, 2) selecting the point on the predicted trajectory with the
minimal distance to the center of the robot's legs in their nominal position,
and 3) selecting the point on the predicted trajectory with the highest
likelihood on a Gaussian Mixture Model (GMM) modelling the robot's reachable
space. Experimental results demonstrate robust catching capabilities across
various scenarios, with the GMM method achieving the best performance, leading
to an 80% catching success rate. A video demonstration of the system in action
can be found at https://youtu.be/sm7RdxRfIYg .

[Website Link](https://youtu.be/sm7RdxRfIYg)

[Paper Link](
https://arxiv.org/abs/2410.08065
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-05.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-10


### Embodied Agent Interface: Benchmarking LLMs for Embodied Decision Making

- **Authors**: Manling Li, Shiyu Zhao, Qineng Wang, Kangrui Wang, Yu Zhou, Sanjana Srivastava, Cem Gokmen, Tony Lee, Li Erran Li, Ruohan Zhang, Weiyu Liu, Percy Liang, Li Fei-Fei, Jiayuan Mao, Jiajun Wu

#### Abstract

We aim to evaluate Large Language Models (LLMs) for embodied decision making.
While a significant body of work has been leveraging LLMs for decision making
in embodied environments, we still lack a systematic understanding of their
performance because they are usually applied in different domains, for
different purposes, and built based on different inputs and outputs.
Furthermore, existing evaluations tend to rely solely on a final success rate,
making it difficult to pinpoint what ability is missing in LLMs and where the
problem lies, which in turn blocks embodied agents from leveraging LLMs
effectively and selectively. To address these limitations, we propose a
generalized interface (Embodied Agent Interface) that supports the
formalization of various types of tasks and input-output specifications of
LLM-based modules. Specifically, it allows us to unify 1) a broad set of
embodied decision-making tasks involving both state and temporally extended
goals, 2) four commonly-used LLM-based modules for decision making: goal
interpretation, subgoal decomposition, action sequencing, and transition
modeling, and 3) a collection of fine-grained metrics which break down
evaluation into various types of errors, such as hallucination errors,
affordance errors, various types of planning errors, etc. Overall, our
benchmark offers a comprehensive assessment of LLMs' performance for different
subtasks, pinpointing the strengths and weaknesses in LLM-powered embodied AI
systems, and providing insights for effective and selective use of LLMs in
embodied decision making.

[Paper Link](
https://arxiv.org/abs/2410.07166
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-02.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Whole-Body Dynamic Throwing with Legged Manipulators

- **Authors**: Humphrey Munn, Brendan Tidd, David Howard, Marcus Gallagher

#### Abstract

Most robotic behaviours focus on either manipulation or locomotion, where
tasks that require the integration of both, such as full-body throwing, remain
under-explored. Throwing with a robot involves complex coordination between
object manipulation and legged locomotion, which is crucial for advanced
real-world interactions. This work investigates the challenge of full-body
throwing in robotic systems and highlights the advantages of utilising the
robot's entire body. We propose a deep reinforcement learning (RL) approach
that leverages the robot's body to enhance throwing performance through a
strategically designed curriculum to avoid local optima and sparse but
informative reward functions to improve policy flexibility. The robot's body
learns to generate additional momentum and fine-tune the projectile release
velocity. Our full-body method achieves on average 47% greater throwing
distance and 34% greater throwing accuracy than the arm alone, across two robot
morphologies - an armed quadruped and a humanoid. We also extend our method to
optimise robot stability during throws. The learned policy effectively
generalises throwing to targets at any 3D point in space within a specified
range, which has not previously been achieved and does so with human-level
throwing accuracy. We successfully transferred this approach from simulation to
a real robot using sim2real techniques, demonstrating its practical viability.

[Paper Link](
https://arxiv.org/abs/2410.05681
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-22_00-01.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### OrionNav: Online Planning for Robot Autonomy with Context-Aware LLM and Open-Vocabulary Semantic Scene Graphs

- **Authors**: Venkata Naren Devarakonda, Raktim Gautam Goswami, Ali Umut Kaypak, Naman Patel, Rooholla Khorrambakht, Prashanth Krishnamurthy, Farshad Khorrami

#### Abstract

Enabling robots to autonomously navigate unknown, complex, dynamic
environments and perform diverse tasks remains a fundamental challenge in
developing robust autonomous physical agents. They must effectively perceive
their surroundings while leveraging world knowledge for decision-making. While
recent approaches utilize vision-language and large language models for scene
understanding and planning, they often rely on offline processing, external
computing, or restrictive environmental assumptions. We present a novel
framework for efficient and scalable real-time, onboard autonomous navigation
that integrates multi-level abstraction in both perception and planning in
unknown large-scale environments that change over time. Our system fuses data
from multiple onboard sensors for localization and mapping and integrates it
with open-vocabulary semantics to generate hierarchical scene graphs. An
LLM-based planner leverages these graphs to generate high-level task execution
strategies, which guide low-level controllers in safely accomplishing goals.
Our framework's real-time operation enables continuous updates to scene graphs
and plans, allowing swift responses to environmental changes and on-the-fly
error correction. This is a key advantage over static or rule-based planning
systems. We demonstrate our system's efficacy on a quadruped robot navigating
large-scale, dynamic environments, showcasing its adaptability and robustness
in diverse scenarios.

[Paper Link](
https://arxiv.org/abs/2410.06239
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-59.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-21


### LocoVR: Multiuser Indoor Locomotion Dataset in Virtual Reality

- **Authors**: Kojiro Takeyama, Yimeng Liu, Misha Sra

#### Abstract

Understanding human locomotion is crucial for AI agents such as robots,
particularly in complex indoor home environments. Modeling human trajectories
in these spaces requires insight into how individuals maneuver around physical
obstacles and manage social navigation dynamics. These dynamics include subtle
behaviors influenced by proxemics - the social use of space, such as stepping
aside to allow others to pass or choosing longer routes to avoid collisions.
Previous research has developed datasets of human motion in indoor scenes, but
these are often limited in scale and lack the nuanced social navigation
dynamics common in home environments. To address this, we present LocoVR, a
dataset of 7000+ two-person trajectories captured in virtual reality from over
130 different indoor home environments. LocoVR provides full body pose data and
precise spatial information, along with rich examples of socially-motivated
movement behaviors. For example, the dataset captures instances of individuals
navigating around each other in narrow spaces, adjusting paths to respect
personal boundaries in living areas, and coordinating movements in high-traffic
zones like entryways and kitchens. Our evaluation shows that LocoVR
significantly enhances model performance in three practical indoor tasks
utilizing human trajectories, and demonstrates predicting socially-aware
navigation patterns in home environments.

[Paper Link](
https://arxiv.org/abs/2410.06437
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-58.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Real-to-Sim Grasp: Rethinking the Gap between Simulation and Real World in Grasp Detection

- **Authors**: Jia-Feng Cai, Zibo Chen, Xiao-Ming Wu, Jian-Jian Jiang, Yi-Lin Wei, Wei-Shi Zheng

#### Abstract

For 6-DoF grasp detection, simulated data is expandable to train more
powerful model, but it faces the challenge of the large gap between simulation
and real world. Previous works bridge this gap with a sim-to-real way. However,
this way explicitly or implicitly forces the simulated data to adapt to the
noisy real data when training grasp detectors, where the positional drift and
structural distortion within the camera noise will harm the grasp learning. In
this work, we propose a Real-to-Sim framework for 6-DoF Grasp detection, named
R2SGrasp, with the key insight of bridging this gap in a real-to-sim way, which
directly bypasses the camera noise in grasp detector training through an
inference-time real-to-sim adaption. To achieve this real-to-sim adaptation,
our R2SGrasp designs the Real-to-Sim Data Repairer (R2SRepairer) to mitigate
the camera noise of real depth maps in data-level, and the Real-to-Sim Feature
Enhancer (R2SEnhancer) to enhance real features with precise simulated
geometric primitives in feature-level. To endow our framework with the
generalization ability, we construct a large-scale simulated dataset
cost-efficiently to train our grasp detector, which includes 64,000 RGB-D
images with 14.4 million grasp annotations. Sufficient experiments show that
R2SGrasp is powerful and our real-to-sim perspective is effective. The
real-world experiments further show great generalization ability of R2SGrasp.
Project page is available on https://isee-laboratory.github.io/R2SGrasp.

[Website Link](https://isee-laboratory.github.io/R2SGrasp.)

[Paper Link](
https://arxiv.org/abs/2410.06521
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-57.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### M3Bench: Benchmarking Whole-body Motion Generation for Mobile Manipulation in 3D Scenes

- **Authors**: Zeyu Zhang, Sixu Yan, Muzhi Han, Zaijin Wang, Xinggang Wang, Song-Chun Zhu, Hangxin Liu

#### Abstract

We propose M^3Bench, a new benchmark of whole-body motion generation for
mobile manipulation tasks. Given a 3D scene context, M^3Bench requires an
embodied agent to understand its configuration, environmental constraints and
task objectives, then generate coordinated whole-body motion trajectories for
object rearrangement tasks. M^3Bench features 30k object rearrangement tasks
across 119 diverse scenes, providing expert demonstrations generated by our
newly developed M^3BenchMaker. This automatic data generation tool produces
coordinated whole-body motion trajectories from high-level task instructions,
requiring only basic scene and robot information. Our benchmark incorporates
various task splits to assess generalization across different dimensions and
leverages realistic physics simulation for trajectory evaluation. Through
extensive experimental analyses, we reveal that state-of-the-art models still
struggle with coordinated base-arm motion while adhering to environment-context
and task-specific constraints, highlighting the need to develop new models that
address this gap. Through M^3Bench, we aim to facilitate future robotics
research towards more adaptive and capable mobile manipulation in diverse,
real-world environments.

[Paper Link](
https://arxiv.org/abs/2410.06678
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-56.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### VIRT: Vision Instructed Transformer for Robotic Manipulation

- **Authors**: Zhuoling Li, Liangliang Ren, Jinrong Yang, Yong Zhao, Xiaoyang Wu, Zhenhua Xu, Xiang Bai, Hengshuang Zhao

#### Abstract

Robotic manipulation, owing to its multi-modal nature, often faces
significant training ambiguity, necessitating explicit instructions to clearly
delineate the manipulation details in tasks. In this work, we highlight that
vision instruction is naturally more comprehensible to recent robotic policies
than the commonly adopted text instruction, as these policies are born with
some vision understanding ability like human infants. Building on this premise
and drawing inspiration from cognitive science, we introduce the robotic
imagery paradigm, which realizes large-scale robotic data pre-training without
text annotations. Additionally, we propose the robotic gaze strategy that
emulates the human eye gaze mechanism, thereby guiding subsequent actions and
focusing the attention of the policy on the manipulated object. Leveraging
these innovations, we develop VIRT, a fully Transformer-based policy. We design
comprehensive tasks using both a physical robot and simulated environments to
assess the efficacy of VIRT. The results indicate that VIRT can complete very
competitive tasks like ``opening the lid of a tightly sealed bottle'', and the
proposed techniques boost the success rates of the baseline policy on diverse
challenging tasks from nearly 0% to more than 65%.

[Paper Link](
https://arxiv.org/abs/2410.07169
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-53.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-08


### ETHcavation: A Dataset and Pipeline for Panoptic Scene Understanding and Object Tracking in Dynamic Construction Environments

- **Authors**: Lorenzo Terenzi, Julian Nubert, Pol Eyschen, Pascal Roth, Simin Fei, Edo Jelavic, Marco Hutter

#### Abstract

Construction sites are challenging environments for autonomous systems due to
their unstructured nature and the presence of dynamic actors, such as workers
and machinery. This work presents a comprehensive panoptic scene understanding
solution designed to handle the complexities of such environments by
integrating 2D panoptic segmentation with 3D LiDAR mapping. Our system
generates detailed environmental representations in real-time by combining
semantic and geometric data, supported by Kalman Filter-based tracking for
dynamic object detection. We introduce a fine-tuning method that adapts large
pre-trained panoptic segmentation models for construction site applications
using a limited number of domain-specific samples. For this use case, we
release a first-of-its-kind dataset of 502 hand-labeled sample images with
panoptic annotations from construction sites. In addition, we propose a dynamic
panoptic mapping technique that enhances scene understanding in unstructured
environments. As a case study, we demonstrate the system's application for
autonomous navigation, utilizing real-time RRT* for reactive path planning in
dynamic scenarios. The dataset
(https://leggedrobotics.github.io/panoptic-scene-understanding.github.io/) and
code (https://github.com/leggedrobotics/rsl_panoptic_mapping) for training and
deployment are publicly available to support future research.

[Website Link](https://leggedrobotics.github.io/panoptic-scene-understanding.github.io/))

[Paper Link](
https://arxiv.org/abs/2410.04250
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-49.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GARField: Addressing the visual Sim-to-Real gap in garment manipulation with mesh-attached radiance fields

- **Authors**: Donatien Delehelle, Darwin G. Caldwell, Fei Chen

#### Abstract

While humans intuitively manipulate garments and other textiles items swiftly
and accurately, it is a significant challenge for robots. A factor crucial to
the human performance is the ability to imagine, a priori, the intended result
of the manipulation intents and hence develop predictions on the garment pose.
This allows us to plan from highly obstructed states, adapt our plans as we
collect more information and react swiftly to unforeseen circumstances. Robots,
on the other hand, struggle to establish such intuitions and form tight links
between plans and observations. This can be attributed in part to the high cost
of obtaining densely labelled data for textile manipulation, both in quality
and quantity. The problem of data collection is a long standing issue in
data-based approaches to garment manipulation. Currently, the generation of
high quality and labelled garment manipulation data is mainly attempted through
advanced data capture procedures that create simplified state estimations from
real-world observations. In this work, however, we propose to generate
real-world observations from given object states. To achieve this, we present
GARField (Garment Attached Radiance Field) a differentiable rendering
architecture allowing data generation from simulated states stored as triangle
meshes. Code will be available on https://ddonatien.github.io/garfield-website/

[Website Link](https://ddonatien.github.io/garfield-website/)

[Paper Link](
https://arxiv.org/abs/2410.05038
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-47.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### PhotoReg: Photometrically Registering 3D Gaussian Splatting Models

- **Authors**: Ziwen Yuan, Tianyi Zhang, Matthew Johnson-Roberson, Weiming Zhi

#### Abstract

Building accurate representations of the environment is critical for
intelligent robots to make decisions during deployment. Advances in
photorealistic environment models have enabled robots to develop
hyper-realistic reconstructions, which can be used to generate images that are
intuitive for human inspection. In particular, the recently introduced
\ac{3DGS}, which describes the scene with up to millions of primitive
ellipsoids, can be rendered in real time. \ac{3DGS} has rapidly gained
prominence. However, a critical unsolved problem persists: how can we fuse
multiple \ac{3DGS} into a single coherent model? Solving this problem will
enable robot teams to jointly build \ac{3DGS} models of their surroundings. A
key insight of this work is to leverage the {duality} between photorealistic
reconstructions, which render realistic 2D images from 3D structure, and
\emph{3D foundation models}, which predict 3D structure from image pairs. To
this end, we develop PhotoReg, a framework to register multiple photorealistic
\ac{3DGS} models with 3D foundation models. As \ac{3DGS} models are generally
built from monocular camera images, they have \emph{arbitrary scale}. To
resolve this, PhotoReg actively enforces scale consistency among the different
\ac{3DGS} models by considering depth estimates within these models. Then, the
alignment is iteratively refined with fine-grained photometric losses to
produce high-quality fused \ac{3DGS} models. We rigorously evaluate PhotoReg on
both standard benchmark datasets and our custom-collected datasets, including
with two quadruped robots. The code is released at
\url{ziweny11.github.io/photoreg}.

[Paper Link](
https://arxiv.org/abs/2410.05044
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-46_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### HE-Nav: A High-Performance and Efficient Navigation System for Aerial-Ground Robots in Cluttered Environments

- **Authors**: Junming Wang, Zekai Sun, Xiuxian Guan, Tianxiang Shen, Dong Huang, Zongyuan Zhang, Tianyang Duan, Fangming Liu, Heming Cui

#### Abstract

Existing AGR navigation systems have advanced in lightly occluded scenarios
(e.g., buildings) by employing 3D semantic scene completion networks for voxel
occupancy prediction and constructing Euclidean Signed Distance Field (ESDF)
maps for collision-free path planning. However, these systems exhibit
suboptimal performance and efficiency in cluttered environments with severe
occlusions (e.g., dense forests or tall walls), due to limitations arising from
perception networks' low prediction accuracy and path planners' high
computational overhead. In this paper, we present HE-Nav, the first
high-performance and efficient navigation system tailored for AGRs operating in
cluttered environments. The perception module utilizes a lightweight semantic
scene completion network (LBSCNet), guided by a bird's eye view (BEV) feature
fusion and enhanced by an exquisitely designed SCB-Fusion module and attention
mechanism. This enables real-time and efficient obstacle prediction in
cluttered areas, generating a complete local map. Building upon this completed
map, our novel AG-Planner employs the energy-efficient kinodynamic A* search
algorithm to guarantee planning is energy-saving. Subsequent trajectory
optimization processes yield safe, smooth, dynamically feasible and ESDF-free
aerial-ground hybrid paths. Extensive experiments demonstrate that HE-Nav
achieved 7x energy savings in real-world situations while maintaining planning
success rates of 98% in simulation scenarios. Code and video are available on
our project page: https://jmwang0117.github.io/HE-Nav/.

[Website Link](https://jmwang0117.github.io/HE-Nav/.)

[Paper Link](
https://arxiv.org/abs/2410.05079
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-46.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Towards a Modern and Lightweight Rendering Engine for Dynamic Robotic Simulations

- **Authors**: Christopher John Allison, Haoying Zhou, Adnan Munawar, Peter Kazanzides, Juan Antonio Barragan

#### Abstract

Interactive dynamic simulators are an accelerator for developing novel
robotic control algorithms and complex systems involving humans and robots. In
user training and synthetic data generation applications, a high-fidelity
visualization of the simulation is essential. Visual fidelity is dependent on
the quality of the computer graphics algorithms used to render the simulated
scene. Furthermore, the rendering algorithms must be implemented on the
graphics processing unit (GPU) to achieve real-time performance, requiring the
use of a graphics application programming interface (API). This paper presents
a performance-focused and lightweight rendering engine supporting the Vulkan
graphics API. The engine is designed to modernize the legacy rendering pipeline
of Asynchronous Multi-Body Framework (AMBF), a dynamic simulation framework
used extensively for interactive robotics simulation development. This new
rendering engine implements graphical features such as physically based
rendering (PBR), anti-aliasing, and ray-traced shadows, significantly improving
the image quality of AMBF. Computational experiments show that the engine can
render a simulated scene with over seven million triangles while maintaining
GPU computation times within two milliseconds.

[Paper Link](
https://arxiv.org/abs/2410.05095
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-45.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Proprioceptive State Estimation for Quadruped Robots using Invariant Kalman Filtering and Scale-Variant Robust Cost Functions

- **Authors**: Hilton Marques Souza Santana, João Carlos Virgolino Soares, Ylenia Nisticò, Marco Antonio Meggiolaro, Claudio Semini

#### Abstract

Accurate state estimation is crucial for legged robot locomotion, as it
provides the necessary information to allow control and navigation. However, it
is also challenging, especially in scenarios with uneven and slippery terrain.
This paper presents a new Invariant Extended Kalman filter for legged robot
state estimation using only proprioceptive sensors. We formulate the
methodology by combining recent advances in state estimation theory with the
use of robust cost functions in the measurement update. We tested our
methodology on quadruped robots through experiments and public datasets,
showing that we can obtain a pose drift up to 40% lower in trajectories
covering a distance of over 450m, in comparison with a state-of-the-art
Invariant Extended Kalman filter.

[Paper Link](
https://arxiv.org/abs/2410.05256
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-44.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-07


### MO-DDN: A Coarse-to-Fine Attribute-based Exploration Agent for Multi-object Demand-driven Navigation

- **Authors**: Hongcheng Wang, Peiqi Liu, Wenzhe Cai, Mingdong Wu, Zhengyu Qian, Hao Dong

#### Abstract

The process of satisfying daily demands is a fundamental aspect of humans'
daily lives. With the advancement of embodied AI, robots are increasingly
capable of satisfying human demands. Demand-driven navigation (DDN) is a task
in which an agent must locate an object to satisfy a specified demand
instruction, such as ``I am thirsty.'' The previous study typically assumes
that each demand instruction requires only one object to be fulfilled and does
not consider individual preferences. However, the realistic human demand may
involve multiple objects. In this paper, we introduce the Multi-object
Demand-driven Navigation (MO-DDN) benchmark, which addresses these nuanced
aspects, including multi-object search and personal preferences, thus making
the MO-DDN task more reflective of real-life scenarios compared to DDN.
Building upon previous work, we employ the concept of ``attribute'' to tackle
this new task. However, instead of solely relying on attribute features in an
end-to-end manner like DDN, we propose a modular method that involves
constructing a coarse-to-fine attribute-based exploration agent (C2FAgent). Our
experimental results illustrate that this coarse-to-fine exploration strategy
capitalizes on the advantages of attributes at various decision-making levels,
resulting in superior performance compared to baseline methods. Code and video
can be found at https://sites.google.com/view/moddn.

[Website Link](https://sites.google.com/view/moddn.)

[Paper Link](
https://arxiv.org/abs/2410.03488
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-38.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GenSim2: Scaling Robot Data Generation with Multi-modal and Reasoning LLMs

- **Authors**: Pu Hua, Minghuan Liu, Annabella Macaluso, Yunfeng Lin, Weinan Zhang, Huazhe Xu, Lirui Wang

#### Abstract

Robotic simulation today remains challenging to scale up due to the human
efforts required to create diverse simulation tasks and scenes.
Simulation-trained policies also face scalability issues as many sim-to-real
methods focus on a single task. To address these challenges, this work proposes
GenSim2, a scalable framework that leverages coding LLMs with multi-modal and
reasoning capabilities for complex and realistic simulation task creation,
including long-horizon tasks with articulated objects. To automatically
generate demonstration data for these tasks at scale, we propose planning and
RL solvers that generalize within object categories. The pipeline can generate
data for up to 100 articulated tasks with 200 objects and reduce the required
human efforts. To utilize such data, we propose an effective multi-task
language-conditioned policy architecture, dubbed proprioceptive point-cloud
transformer (PPT), that learns from the generated demonstrations and exhibits
strong sim-to-real zero-shot transfer. Combining the proposed pipeline and the
policy architecture, we show a promising usage of GenSim2 that the generated
data can be used for zero-shot transfer or co-train with real-world collected
data, which enhances the policy performance by 20% compared with training
exclusively on limited real data.

[Paper Link](
https://arxiv.org/abs/2410.03645
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-37_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Learning Humanoid Locomotion over Challenging Terrain

- **Authors**: Ilija Radosavovic, Sarthak Kamat, Trevor Darrell, Jitendra Malik

#### Abstract

Humanoid robots can, in principle, use their legs to go almost anywhere.
Developing controllers capable of traversing diverse terrains, however, remains
a considerable challenge. Classical controllers are hard to generalize broadly
while the learning-based methods have primarily focused on gentle terrains.
Here, we present a learning-based approach for blind humanoid locomotion
capable of traversing challenging natural and man-made terrain. Our method uses
a transformer model to predict the next action based on the history of
proprioceptive observations and actions. The model is first pre-trained on a
dataset of flat-ground trajectories with sequence modeling, and then fine-tuned
on uneven terrain using reinforcement learning. We evaluate our model on a real
humanoid robot across a variety of terrains, including rough, deformable, and
sloped surfaces. The model demonstrates robust performance, in-context
adaptation, and emergent terrain representations. In real-world case studies,
our humanoid robot successfully traversed over 4 miles of hiking trails in
Berkeley and climbed some of the steepest streets in San Francisco.

[Paper Link](
https://arxiv.org/abs/2410.03654
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-37.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-04


### DivScene: Benchmarking LVLMs for Object Navigation with Diverse Scenes and Objects

- **Authors**: Zhaowei Wang, Hongming Zhang, Tianqing Fang, Ye Tian, Yue Yang, Kaixin Ma, Xiaoman Pan, Yangqiu Song, Dong Yu

#### Abstract

Object navigation in unknown environments is crucial for deploying embodied
agents in real-world applications. While we have witnessed huge progress due to
large-scale scene datasets, faster simulators, and stronger models, previous
studies mainly focus on limited scene types and target objects. In this paper,
we study a new task of navigating to diverse target objects in a large number
of scene types. To benchmark the problem, we present a large-scale scene
dataset, DivScene, which contains 4,614 scenes across 81 different types. With
the dataset, we build an end-to-end embodied agent, NatVLM, by fine-tuning a
Large Vision Language Model (LVLM) through imitation learning. The LVLM is
trained to take previous observations from the environment and generate the
next actions. We also introduce CoT explanation traces of the action prediction
for better performance when tuning LVLMs. Our extensive experiments find that
we can build a performant LVLM-based agent through imitation learning on the
shortest paths constructed by a BFS planner without any human supervision. Our
agent achieves a success rate that surpasses GPT-4o by over 20%. Meanwhile, we
carry out various analyses showing the generalization ability of our agent. Our
code and data are available at https://github.com/zhaowei-wang-nlp/DivScene.

[Website Link](https://github.com/zhaowei-wang-nlp/DivScene.)

[Paper Link](
https://arxiv.org/abs/2410.02730
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-35.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Learning Diverse Bimanual Dexterous Manipulation Skills from Human Demonstrations

- **Authors**: Bohan Zhou, Haoqi Yuan, Yuhui Fu, Zongqing Lu

#### Abstract

Bimanual dexterous manipulation is a critical yet underexplored area in
robotics. Its high-dimensional action space and inherent task complexity
present significant challenges for policy learning, and the limited task
diversity in existing benchmarks hinders general-purpose skill development.
Existing approaches largely depend on reinforcement learning, often constrained
by intricately designed reward functions tailored to a narrow set of tasks. In
this work, we present a novel approach for efficiently learning diverse
bimanual dexterous skills from abundant human demonstrations. Specifically, we
introduce BiDexHD, a framework that unifies task construction from existing
bimanual datasets and employs teacher-student policy learning to address all
tasks. The teacher learns state-based policies using a general two-stage reward
function across tasks with shared behaviors, while the student distills the
learned multi-task policies into a vision-based policy. With BiDexHD, scalable
learning of numerous bimanual dexterous skills from auto-constructed tasks
becomes feasible, offering promising advances toward universal bimanual
dexterous manipulation. Our empirical evaluation on the TACO dataset, spanning
141 tasks across six categories, demonstrates a task fulfillment rate of 74.59%
on trained tasks and 51.07% on unseen tasks, showcasing the effectiveness and
competitive zero-shot generalization capabilities of BiDexHD. For videos and
more information, visit our project page https://sites.google.com/view/bidexhd.

[Website Link](https://sites.google.com/view/bidexhd.)

[Paper Link](
https://arxiv.org/abs/2410.02477
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-34.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Cross-Embodiment Dexterous Grasping with Reinforcement Learning

- **Authors**: Haoqi Yuan, Bohan Zhou, Yuhui Fu, Zongqing Lu

#### Abstract

Dexterous hands exhibit significant potential for complex real-world grasping
tasks. While recent studies have primarily focused on learning policies for
specific robotic hands, the development of a universal policy that controls
diverse dexterous hands remains largely unexplored. In this work, we study the
learning of cross-embodiment dexterous grasping policies using reinforcement
learning (RL). Inspired by the capability of human hands to control various
dexterous hands through teleoperation, we propose a universal action space
based on the human hand's eigengrasps. The policy outputs eigengrasp actions
that are then converted into specific joint actions for each robot hand through
a retargeting mapping. We simplify the robot hand's proprioception to include
only the positions of fingertips and the palm, offering a unified observation
space across different robot hands. Our approach demonstrates an 80% success
rate in grasping objects from the YCB dataset across four distinct embodiments
using a single vision-based policy. Additionally, our policy exhibits zero-shot
generalization to two previously unseen embodiments and significant improvement
in efficient finetuning. For further details and videos, visit our project page
https://sites.google.com/view/crossdex.

[Website Link](https://sites.google.com/view/crossdex.)

[Paper Link](
https://arxiv.org/abs/2410.02479
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-32.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-03


### Divide et Impera: Learning impedance families for peg-in-hole assembly

- **Authors**: Johannes Lachner, Federico Tessari, A. Michael West Jr., Moses C. Nah, Neville Hogan

#### Abstract

This paper addresses robotic peg-in-hole assembly using the framework of
Elementary Dynamic Actions (EDA). Inspired by motor primitives in neuromotor
control research, the method leverages three primitives: submovements,
oscillations, and mechanical impedances (e.g., stiffness and damping), combined
via a Norton equivalent network model. By focusing on impedance
parameterization, we explore the adaptability of EDA in contact-rich tasks.
Experimental results, conducted on a real robot setup with four different peg
types, demonstrated a range of successful impedance parameters, challenging
conventional methods that seek optimal parameters. We analyze our data in a
lower-dimensional solution space. Clustering analysis shows the possibility to
identify different individual strategies for each single peg, as well as common
strategies across all pegs. A neural network model, trained on the experimental
data, accurately predicted successful impedance parameters across all pegs. The
practical utility of this work is enhanced by a success-predictor model and the
public availability of all code and CAD files. These findings highlight the
flexibility and robustness of EDA; show multiple equally-successful strategies
for contact-rich manipulation; and offer valuable insights and tools for
robotic assembly programming.

[Paper Link](
https://arxiv.org/abs/2410.01054
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-28.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RoTip: A Finger-Shaped Tactile Sensor with Active Rotation

- **Authors**: Xuyang Zhang, Jiaqi Jiang, Shan Luo

#### Abstract

In recent years, advancements in optical tactile sensor technology have
primarily centred on enhancing sensing precision and expanding the range of
sensing modalities. To meet the requirements for more skilful manipulation,
there should be a movement towards making tactile sensors more dynamic. In this
paper, we introduce RoTip, a novel vision-based tactile sensor that is uniquely
designed with an independently controlled joint and the capability to sense
contact over its entire surface. The rotational capability of the sensor is
particularly crucial for manipulating everyday objects, especially thin and
flexible ones, as it enables the sensor to mobilize while in contact with the
object's surface. The manipulation experiments demonstrate the ability of our
proposed RoTip to manipulate rigid and flexible objects, and the full-finger
tactile feedback and active rotation capabilities have the potential to explore
more complex and precise manipulation tasks.

[Paper Link](
https://arxiv.org/abs/2410.01085
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-27.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### D(R, O) Grasp: A Unified Representation of Robot and Object Interaction for Cross-Embodiment Dexterous Grasping

- **Authors**: Zhenyu Wei, Zhixuan Xu, Jingxiang Guo, Yiwen Hou, Chongkai Gao, Zhehao Cai, Jiayu Luo, Lin Shao

#### Abstract

Dexterous grasping is a fundamental yet challenging skill in robotic
manipulation, requiring precise interaction between robotic hands and objects.
In this paper, we present D(R,O) Grasp, a novel framework that models the
interaction between the robotic hand in its grasping pose and the object,
enabling broad generalization across various robot hands and object geometries.
Our model takes the robot hand's description and object point cloud as inputs
and efficiently predicts kinematically valid and stable grasps, demonstrating
strong adaptability to diverse robot embodiments and object geometries.
Extensive experiments conducted in both simulated and real-world environments
validate the effectiveness of our approach, with significant improvements in
success rate, grasp diversity, and inference speed across multiple robotic
hands. Our method achieves an average success rate of 87.53% in simulation in
less than one second, tested across three different dexterous robotic hands. In
real-world experiments using the LeapHand, the method also demonstrates an
average success rate of 89%. D(R,O) Grasp provides a robust solution for
dexterous grasping in complex and varied environments. The code, appendix, and
videos are available on our project website at
https://nus-lins-lab.github.io/drograspweb/.

[Website Link](https://nus-lins-lab.github.io/drograspweb/.)

[Paper Link](
https://arxiv.org/abs/2410.01702
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-20.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-02


### Helpful DoggyBot: Open-World Object Fetching using Legged Robots and Vision-Language Models

- **Authors**: Qi Wu, Zipeng Fu, Xuxin Cheng, Xiaolong Wang, Chelsea Finn

#### Abstract

Learning-based methods have achieved strong performance for quadrupedal
locomotion. However, several challenges prevent quadrupeds from learning
helpful indoor skills that require interaction with environments and humans:
lack of end-effectors for manipulation, limited semantic understanding using
only simulation data, and low traversability and reachability in indoor
environments. We present a system for quadrupedal mobile manipulation in indoor
environments. It uses a front-mounted gripper for object manipulation, a
low-level controller trained in simulation using egocentric depth for agile
skills like climbing and whole-body tilting, and pre-trained vision-language
models (VLMs) with a third-person fisheye and an egocentric RGB camera for
semantic understanding and command generation. We evaluate our system in two
unseen environments without any real-world data collection or training. Our
system can zero-shot generalize to these environments and complete tasks, like
following user's commands to fetch a randomly placed stuff toy after climbing
over a queen-sized bed, with a 60% success rate. Project website:
https://helpful-doggybot.github.io/

[Website Link](https://helpful-doggybot.github.io/)

[Paper Link](
https://arxiv.org/abs/2410.00231
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-16.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### ManiSkill3: GPU Parallelized Robotics Simulation and Rendering for Generalizable Embodied AI

- **Authors**: Stone Tao, Fanbo Xiang, Arth Shukla, Yuzhe Qin, Xander Hinrichsen, Xiaodi Yuan, Chen Bao, Xinsong Lin, Yulin Liu, Tse-kai Chan, Yuan Gao, Xuanlin Li, Tongzhou Mu, Nan Xiao, Arnav Gurha, Zhiao Huang, Roberto Calandra, Rui Chen, Shan Luo, Hao Su

#### Abstract

Simulation has enabled unprecedented compute-scalable approaches to robot
learning. However, many existing simulation frameworks typically support a
narrow range of scenes/tasks and lack features critical for scaling
generalizable robotics and sim2real. We introduce and open source ManiSkill3,
the fastest state-visual GPU parallelized robotics simulator with contact-rich
physics targeting generalizable manipulation. ManiSkill3 supports GPU
parallelization of many aspects including simulation+rendering, heterogeneous
simulation, pointclouds/voxels visual input, and more. Simulation with
rendering on ManiSkill3 can run 10-1000x faster with 2-3x less GPU memory usage
than other platforms, achieving up to 30,000+ FPS in benchmarked environments
due to minimal python/pytorch overhead in the system, simulation on the GPU,
and the use of the SAPIEN parallel rendering system. Tasks that used to take
hours to train can now take minutes. We further provide the most comprehensive
range of GPU parallelized environments/tasks spanning 12 distinct domains
including but not limited to mobile manipulation for tasks such as drawing,
humanoids, and dextrous manipulation in realistic scenes designed by artists or
real-world digital twins. In addition, millions of demonstration frames are
provided from motion planning, RL, and teleoperation. ManiSkill3 also provides
a comprehensive set of baselines that span popular RL and
learning-from-demonstrations algorithms.

[Paper Link](
https://arxiv.org/abs/2410.00425
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-14_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RobotGraffiti: An AR tool for semi-automated construction of workcell models to optimize robot deployment

- **Authors**: Krzysztof Zieliński, Ryan Penning, Bruce Blumberg, Christian Schlette, Mikkel Baun Kjærgaard

#### Abstract

Improving robot deployment is a central step towards speeding up robot-based
automation in manufacturing. A main challenge in robot deployment is how to
best place the robot within the workcell. To tackle this challenge, we combine
two knowledge sources: robotic knowledge of the system and workcell context
awareness of the user, and intersect them with an Augmented Reality interface.
RobotGraffiti is a unique tool that empowers the user in robot deployment
tasks. One simply takes a 3D scan of the workcell with their mobile device,
adds contextual data points that otherwise would be difficult to infer from the
system, and receives a robot base position that satisfies the automation task.
The proposed approach is an alternative to expensive and time-consuming digital
twins, with a fast and easy-to-use tool that focuses on selected workcell
features needed to run the placement optimization algorithm. The main
contributions of this paper are the novel user interface for robot base
placement data collection and a study comparing the traditional offline
simulation with our proposed method. We showcase the method with a robot base
placement solution and obtain up to 16 times reduction in time.

[Paper Link](
https://arxiv.org/abs/2410.00484
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-14.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Obstacle-Avoidant Leader Following with a Quadruped Robot

- **Authors**: Carmen Scheidemann, Lennart Werner, Victor Reijgwart, Andrei Cramariuc, Joris Chomarat, Jia-Ruei Chiu, Roland Siegwart, Marco Hutter

#### Abstract

Personal mobile robotic assistants are expected to find wide applications in
industry and healthcare. For example, people with limited mobility can benefit
from robots helping with daily tasks, or construction workers can have robots
perform precision monitoring tasks on-site. However, manually steering a robot
while in motion requires significant concentration from the operator,
especially in tight or crowded spaces. This reduces walking speed, and the
constant need for vigilance increases fatigue and, thus, the risk of accidents.
This work presents a virtual leash with which a robot can naturally follow an
operator. We use a sensor fusion based on a custom-built RF transponder, RGB
cameras, and a LiDAR. In addition, we customize a local avoidance planner for
legged platforms, which enables us to navigate dynamic and narrow environments.
We successfully validate on the ANYmal platform the robustness and performance
of our entire pipeline in real-world experiments.

[Paper Link](
https://arxiv.org/abs/2410.00572
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-11.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-01


### KineDepth: Utilizing Robot Kinematics for Online Metric Depth Estimation

- **Authors**: Soofiyan Atar, Yuheng Zhi, Florian Richter, Michael Yip

#### Abstract

Depth perception is essential for a robot's spatial and geometric
understanding of its environment, with many tasks traditionally relying on
hardware-based depth sensors like RGB-D or stereo cameras. However, these
sensors face practical limitations, including issues with transparent and
reflective objects, high costs, calibration complexity, spatial and energy
constraints, and increased failure rates in compound systems. While monocular
depth estimation methods offer a cost-effective and simpler alternative, their
adoption in robotics is limited due to their output of relative rather than
metric depth, which is crucial for robotics applications. In this paper, we
propose a method that utilizes a single calibrated camera, enabling the robot
to act as a ``measuring stick" to convert relative depth estimates into metric
depth in real-time as tasks are performed. Our approach employs an LSTM-based
metric depth regressor, trained online and refined through probabilistic
filtering, to accurately restore the metric depth across the monocular depth
map, particularly in areas proximal to the robot's motion. Experiments with
real robots demonstrate that our method significantly outperforms current
state-of-the-art monocular metric depth estimation techniques, achieving a
22.1% reduction in depth error and a 52% increase in success rate for a
downstream task.

[Paper Link](
https://arxiv.org/abs/2409.19490
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-06.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### OptiGrasp: Optimized Grasp Pose Detection Using RGB Images for Warehouse Picking Robots

- **Authors**: Soofiyan Atar, Yi Li, Markus Grotz, Michael Wolf, Dieter Fox, Joshua Smith

#### Abstract

In warehouse environments, robots require robust picking capabilities to
manage a wide variety of objects. Effective deployment demands minimal
hardware, strong generalization to new products, and resilience in diverse
settings. Current methods often rely on depth sensors for structural
information, which suffer from high costs, complex setups, and technical
limitations. Inspired by recent advancements in computer vision, we propose an
innovative approach that leverages foundation models to enhance suction
grasping using only RGB images. Trained solely on a synthetic dataset, our
method generalizes its grasp prediction capabilities to real-world robots and a
diverse range of novel objects not included in the training set. Our network
achieves an 82.3\% success rate in real-world applications. The project website
with code and data will be available at http://optigrasp.github.io.

[Website Link](http://optigrasp.github.io.)

[Paper Link](
https://arxiv.org/abs/2409.19494
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-04.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Fast-UMI: A Scalable and Hardware-Independent Universal Manipulation Interface

- **Authors**: Ziniu Wu, Tianyu Wang, Zhaxizhuoma, Chuyue Guan, Zhongjie Jia, Shuai Liang, Haoming Song, Delin Qu, Dong Wang, Zhigang Wang, Nieqing Cao, Yan Ding, Bin Zhao, Xuelong Li

#### Abstract

Collecting real-world manipulation trajectory data involving robotic arms is
essential for developing general-purpose action policies in robotic
manipulation, yet such data remains scarce. Existing methods face limitations
such as high costs, labor intensity, hardware dependencies, and complex setup
requirements involving SLAM algorithms. In this work, we introduce Fast-UMI, an
interface-mediated manipulation system comprising two key components: a
handheld device operated by humans for data collection and a robot-mounted
device used during policy inference. Our approach employs a decoupled design
compatible with a wide range of grippers while maintaining consistent
observation perspectives, allowing models trained on handheld-collected data to
be directly applied to real robots. By directly obtaining the end-effector pose
using existing commercial hardware products, we eliminate the need for complex
SLAM deployment and calibration, streamlining data processing. Fast-UMI
provides supporting software tools for efficient robot learning data collection
and conversion, facilitating rapid, plug-and-play functionality. This system
offers an efficient and user-friendly tool for robotic learning data
acquisition.

[Paper Link](
https://arxiv.org/abs/2409.19499
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-03_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RoboNurse-VLA: Robotic Scrub Nurse System based on Vision-Language-Action Model

- **Authors**: Shunlei Li, Jin Wang, Rui Dai, Wanyu Ma, Wing Yin Ng, Yingbai Hu, Zheng Li

#### Abstract

In modern healthcare, the demand for autonomous robotic assistants has grown
significantly, particularly in the operating room, where surgical tasks require
precision and reliability. Robotic scrub nurses have emerged as a promising
solution to improve efficiency and reduce human error during surgery. However,
challenges remain in terms of accurately grasping and handing over surgical
instruments, especially when dealing with complex or difficult objects in
dynamic environments. In this work, we introduce a novel robotic scrub nurse
system, RoboNurse-VLA, built on a Vision-Language-Action (VLA) model by
integrating the Segment Anything Model 2 (SAM 2) and the Llama 2 language
model.
  The proposed RoboNurse-VLA system enables highly precise grasping and
handover of surgical instruments in real-time based on voice commands from the
surgeon. Leveraging state-of-the-art vision and language models, the system can
address key challenges for object detection, pose optimization, and the
handling of complex and difficult-to-grasp instruments. Through extensive
evaluations, RoboNurse-VLA demonstrates superior performance compared to
existing models, achieving high success rates in surgical instrument handovers,
even with unseen tools and challenging items. This work presents a significant
step forward in autonomous surgical assistance, showcasing the potential of
integrating VLA models for real-world medical applications. More details can be
found at https://robonurse-vla.github.io.

[Website Link](https://robonurse-vla.github.io.)

[Paper Link](
https://arxiv.org/abs/2409.19590
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-03.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Obstacle-Aware Quadrupedal Locomotion With Resilient Multi-Modal Reinforcement Learning

- **Authors**: I Made Aswin Nahrendra, Byeongho Yu, Minho Oh, Dongkyu Lee, Seunghyun Lee, Hyeonwoo Lee, Hyungtae Lim, Hyun Myung

#### Abstract

Quadrupedal robots hold promising potential for applications in navigating
cluttered environments with resilience akin to their animal counterparts.
However, their floating base configuration makes them vulnerable to real-world
uncertainties, yielding substantial challenges in their locomotion control.
Deep reinforcement learning has become one of the plausible alternatives for
realizing a robust locomotion controller. However, the approaches that rely
solely on proprioception sacrifice collision-free locomotion because they
require front-feet contact to detect the presence of stairs to adapt the
locomotion gait. Meanwhile, incorporating exteroception necessitates a
precisely modeled map observed by exteroceptive sensors over a period of time.
Therefore, this work proposes a novel method to fuse proprioception and
exteroception featuring a resilient multi-modal reinforcement learning. The
proposed method yields a controller that showcases agile locomotion performance
on a quadrupedal robot over a myriad of real-world courses, including rough
terrains, steep slopes, and high-rise stairs, while retaining its robustness
against out-of-distribution situations.

[Paper Link](
https://arxiv.org/abs/2409.19709
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-01.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### The Duke Humanoid: Design and Control For Energy Efficient Bipedal Locomotion Using Passive Dynamics

- **Authors**: Boxi Xia, Bokuan Li, Jacob Lee, Michael Scutari, Boyuan Chen

#### Abstract

We present the Duke Humanoid, an open-source 10-degrees-of-freedom humanoid,
as an extensible platform for locomotion research. The design mimics human
physiology, with minimized leg distances and symmetrical body alignment in the
frontal plane to maintain static balance with straight knees. We develop a
reinforcement learning policy that can be deployed zero-shot on the hardware
for velocity-tracking walking tasks. Additionally, to enhance energy efficiency
in locomotion, we propose an end-to-end reinforcement learning algorithm that
encourages the robot to leverage passive dynamics. Our experiment results show
that our passive policy reduces the cost of transport by up to $50\%$ in
simulation and $31\%$ in real-world testing. Our website is
http://generalroboticslab.com/DukeHumanoidv1/ .

[Website Link](http://generalroboticslab.com/DukeHumanoidv1/)

[Paper Link](
https://arxiv.org/abs/2409.19795
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_23-00.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Playful DoggyBot: Learning Agile and Precise Quadrupedal Locomotion

- **Authors**: Xin Duan, Ziwen Zhuang, Hang Zhao, Soeren Schwertfeger

#### Abstract

Quadrupedal animals have the ability to perform agile while accurate tasks: a
trained dog can chase and catch a flying frisbee before it touches the ground;
a cat alone at home can jump and grab the door handle accurately. However,
agility and precision are usually a trade-off in robotics problems. Recent
works in quadruped robots either focus on agile but not-so-accurate tasks, such
as locomotion in challenging terrain, or accurate but not-so-fast tasks, such
as using an additional manipulator to interact with objects. In this work, we
aim at an accurate and agile task, catching a small object hanging above the
robot. We mount a passive gripper in front of the robot chassis, so that the
robot has to jump and catch the object with extreme precision. Our experiment
shows that our system is able to jump and successfully catch the ball at 1.05m
high in simulation and 0.8m high in the real world, while the robot is 0.3m
high when standing.

[Paper Link](
https://arxiv.org/abs/2409.19920
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_22-47.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GravMAD: Grounded Spatial Value Maps Guided Action Diffusion for Generalized 3D Manipulation

- **Authors**: Yangtao Chen, Zixuan Chen, Junhui Yin, Jing Huo, Pinzhuo Tian, Jieqi Shi, Yang Gao

#### Abstract

Robots' ability to follow language instructions and execute diverse 3D tasks
is vital in robot learning. Traditional imitation learning-based methods
perform well on seen tasks but struggle with novel, unseen ones due to
variability. Recent approaches leverage large foundation models to assist in
understanding novel tasks, thereby mitigating this issue. However, these
methods lack a task-specific learning process, which is essential for an
accurate understanding of 3D environments, often leading to execution failures.
In this paper, we introduce GravMAD, a sub-goal-driven, language-conditioned
action diffusion framework that combines the strengths of imitation learning
and foundation models. Our approach breaks tasks into sub-goals based on
language instructions, allowing auxiliary guidance during both training and
inference. During training, we introduce Sub-goal Keypose Discovery to identify
key sub-goals from demonstrations. Inference differs from training, as there
are no demonstrations available, so we use pre-trained foundation models to
bridge the gap and identify sub-goals for the current task. In both phases,
GravMaps are generated from sub-goals, providing flexible 3D spatial guidance
compared to fixed 3D positions. Empirical evaluations on RLBench show that
GravMAD significantly outperforms state-of-the-art methods, with a 28.63%
improvement on novel tasks and a 13.36% gain on tasks encountered during
training. These results demonstrate GravMAD's strong multi-task learning and
generalization in 3D manipulation. Video demonstrations are available at:
https://gravmad.github.io.

[Website Link](https://gravmad.github.io.)

[Paper Link](
https://arxiv.org/abs/2409.20154
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_22-41.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Opt2Skill: Imitating Dynamically-feasible Whole-Body Trajectories for Versatile Humanoid Loco-Manipulation

- **Authors**: Fukang Liu, Zhaoyuan Gu, Yilin Cai, Ziyi Zhou, Shijie Zhao, Hyunyoung Jung, Sehoon Ha, Yue Chen, Danfei Xu, Ye Zhao

#### Abstract

Humanoid robots are designed to perform diverse loco-manipulation tasks.
However, they face challenges due to their high-dimensional and unstable
dynamics, as well as the complex contact-rich nature of the tasks. Model-based
optimal control methods offer precise and systematic control but are limited by
high computational complexity and accurate contact sensing. On the other hand,
reinforcement learning (RL) provides robustness and handles high-dimensional
spaces but suffers from inefficient learning, unnatural motion, and sim-to-real
gaps. To address these challenges, we introduce Opt2Skill, an end-to-end
pipeline that combines model-based trajectory optimization with RL to achieve
robust whole-body loco-manipulation. We generate reference motions for the
Digit humanoid robot using differential dynamic programming (DDP) and train RL
policies to track these trajectories. Our results demonstrate that Opt2Skill
outperforms pure RL methods in both training efficiency and task performance,
with optimal trajectories that account for torque limits enhancing trajectory
tracking. We successfully transfer our approach to real-world applications.

[Paper Link](
https://arxiv.org/abs/2409.20514
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_22-38.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### UniAff: A Unified Representation of Affordances for Tool Usage and Articulation with Vision-Language Models

- **Authors**: Qiaojun Yu, Siyuan Huang, Xibin Yuan, Zhengkai Jiang, Ce Hao, Xin Li, Haonan Chang, Junbo Wang, Liu Liu, Hongsheng Li, Peng Gao, Cewu Lu

#### Abstract

Previous studies on robotic manipulation are based on a limited understanding
of the underlying 3D motion constraints and affordances. To address these
challenges, we propose a comprehensive paradigm, termed UniAff, that integrates
3D object-centric manipulation and task understanding in a unified formulation.
Specifically, we constructed a dataset labeled with manipulation-related key
attributes, comprising 900 articulated objects from 19 categories and 600 tools
from 12 categories. Furthermore, we leverage MLLMs to infer object-centric
representations for manipulation tasks, including affordance recognition and
reasoning about 3D motion constraints. Comprehensive experiments in both
simulation and real-world settings indicate that UniAff significantly improves
the generalization of robotic manipulation for tools and articulated objects.
We hope that UniAff will serve as a general baseline for unified robotic
manipulation tasks in the future. Images, videos, dataset, and code are
published on the project website at:https://sites.google.com/view/uni-aff/home

[Website Link](https://sites.google.com/view/uni-aff/home)

[Paper Link](
https://arxiv.org/abs/2409.20551
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_22-36.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Continuously Improving Mobile Manipulation with Autonomous Real-World RL

- **Authors**: Russell Mendonca, Emmanuel Panov, Bernadette Bucher, Jiuguang Wang, Deepak Pathak

#### Abstract

We present a fully autonomous real-world RL framework for mobile manipulation
that can learn policies without extensive instrumentation or human supervision.
This is enabled by 1) task-relevant autonomy, which guides exploration towards
object interactions and prevents stagnation near goal states, 2) efficient
policy learning by leveraging basic task knowledge in behavior priors, and 3)
formulating generic rewards that combine human-interpretable semantic
information with low-level, fine-grained observations. We demonstrate that our
approach allows Spot robots to continually improve their performance on a set
of four challenging mobile manipulation tasks, obtaining an average success
rate of 80% across tasks, a 3-4 improvement over existing approaches. Videos
can be found at https://continual-mobile-manip.github.io/

[Website Link](https://continual-mobile-manip.github.io/)

[Paper Link](
https://arxiv.org/abs/2409.20568
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_22-22.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-30


### VLEIBot: A New 45-mg Swimming Microrobot Driven by a Bioinspired Anguilliform Propulsor

- **Authors**: Elijah K. Blankenship, Conor K. Trygstad, Francisco M. F. R. Gonçalves, Néstor O. Pérez-Arancibia

#### Abstract

This paper presents the VLEIBot^* (Very Little Eel-Inspired roBot), a
45-mg/23-mm^3 microrobotic swimmer that is propelled by a bioinspired
anguilliform propulsor. The propulsor is excited by a single 6-mg
high-work-density (HWD) microactuator and undulates periodically due to wave
propagation phenomena generated by fluid-structure interaction (FSI) during
swimming. The microactuator is composed of a carbon-fiber beam, which functions
as a leaf spring, and shape-memory alloy (SMA) wires, which deform cyclically
when excited periodically using Joule heating. The VLEIBot can swim at speeds
as high as 15.1mm * s^{-1} (0.33 Bl * s^{-1}}) when driven with a
heuristically-optimized propulsor. To improve maneuverability, we evolved the
VLEIBot design into the 90-mg/47-mm^3 VLEIBot^+, which is driven by two
propulsors and fully controllable in the two-dimensional (2D) space. The
VLEIBot^+ can swim at speeds as high as 16.1mm * s^{-1} (0.35 Bl * s^{-1}),
when driven with heuristically-optimized propulsors, and achieves turning rates
as high as 0.28 rad * s^{-1}, when tracking path references. The measured
root-mean-square (RMS) values of the tracking errors are as low as 4 mm.

[Paper Link](
https://arxiv.org/abs/2403.07073
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_00-18.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-27


### Active Vision Might Be All You Need: Exploring Active Vision in Bimanual Robotic Manipulation

- **Authors**: Ian Chuang, Andrew Lee, Dechen Gao, Iman Soltani

#### Abstract

Imitation learning has demonstrated significant potential in performing
high-precision manipulation tasks using visual feedback from cameras. However,
it is common practice in imitation learning for cameras to be fixed in place,
resulting in issues like occlusion and limited field of view. Furthermore,
cameras are often placed in broad, general locations, without an effective
viewpoint specific to the robot's task. In this work, we investigate the
utility of active vision (AV) for imitation learning and manipulation, in
which, in addition to the manipulation policy, the robot learns an AV policy
from human demonstrations to dynamically change the robot's camera viewpoint to
obtain better information about its environment and the given task. We
introduce AV-ALOHA, a new bimanual teleoperation robot system with AV, an
extension of the ALOHA 2 robot system, incorporating an additional 7-DoF robot
arm that only carries a stereo camera and is solely tasked with finding the
best viewpoint. This camera streams stereo video to an operator wearing a
virtual reality (VR) headset, allowing the operator to control the camera pose
using head and body movements. The system provides an immersive teleoperation
experience, with bimanual first-person control, enabling the operator to
dynamically explore and search the scene and simultaneously interact with the
environment. We conduct imitation learning experiments of our system both in
real-world and in simulation, across a variety of tasks that emphasize
viewpoint planning. Our results demonstrate the effectiveness of human-guided
AV for imitation learning, showing significant improvements over fixed cameras
in tasks with limited visibility. Project website:
https://soltanilara.github.io/av-aloha/

[Website Link](https://soltanilara.github.io/av-aloha/)

[Paper Link](
https://arxiv.org/abs/2409.17435
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_00-12.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Robust Ladder Climbing with a Quadrupedal Robot

- **Authors**: Dylan Vogel, Robert Baines, Joseph Church, Julian Lotzer, Karl Werner, Marco Hutter

#### Abstract

Quadruped robots are proliferating in industrial environments where they
carry sensor suites and serve as autonomous inspection platforms. Despite the
advantages of legged robots over their wheeled counterparts on rough and uneven
terrain, they are still yet to be able to reliably negotiate ubiquitous
features of industrial infrastructure: ladders. Inability to traverse ladders
prevents quadrupeds from inspecting dangerous locations, puts humans in harm's
way, and reduces industrial site productivity. In this paper, we learn
quadrupedal ladder climbing via a reinforcement learning-based control policy
and a complementary hooked end-effector. We evaluate the robustness in
simulation across different ladder inclinations, rung geometries, and
inter-rung spacings. On hardware, we demonstrate zero-shot transfer with an
overall 90% success rate at ladder angles ranging from 70{\deg} to 90{\deg},
consistent climbing performance during unmodeled perturbations, and climbing
speeds 232x faster than the state of the art. This work expands the scope of
industrial quadruped robot applications beyond inspection on nominal terrains
to challenging infrastructural features in the environment, highlighting
synergies between robot morphology and control policy when performing complex
skills. More information can be found at the project website:
https://sites.google.com/leggedrobotics.com/climbingladders.

[Website Link](https://sites.google.com/leggedrobotics.com/climbingladders.)

[Paper Link](
https://arxiv.org/abs/2409.17731
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_00-10.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### LoopSR: Looping Sim-and-Real for Lifelong Policy Adaptation of Legged Robots

- **Authors**: Peilin Wu, Weiji Xie, Jiahang Cao, Hang Lai, Weinan Zhang

#### Abstract

Reinforcement Learning (RL) has shown its remarkable and generalizable
capability in legged locomotion through sim-to-real transfer. However, while
adaptive methods like domain randomization are expected to make policy more
robust to diverse environments, such comprehensiveness potentially detracts
from the policy's performance in any specific environment according to the No
Free Lunch theorem, leading to a suboptimal solution once deployed in the real
world. To address this issue, we propose a lifelong policy adaptation framework
named LoopSR, which utilizes a transformer-based encoder to project real-world
trajectories into a latent space, and accordingly reconstruct the real-world
environments back in simulation for further improvement. Autoencoder
architecture and contrastive learning methods are adopted to better extract the
characteristics of real-world dynamics. The simulation parameters for continual
training are derived by combining predicted parameters from the decoder with
retrieved parameters from the simulation trajectory dataset. By leveraging the
continual training, LoopSR achieves superior data efficiency compared with
strong baselines, with only a limited amount of data to yield eminent
performance in both sim-to-sim and sim-to-real experiments.

[Paper Link](
https://arxiv.org/abs/2409.17992
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_00-09.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-25


### Tag Map: A Text-Based Map for Spatial Reasoning and Navigation with Large Language Models

- **Authors**: Mike Zhang, Kaixian Qu, Vaishakh Patil, Cesar Cadena, Marco Hutter

#### Abstract

Large Language Models (LLM) have emerged as a tool for robots to generate
task plans using common sense reasoning. For the LLM to generate actionable
plans, scene context must be provided, often through a map. Recent works have
shifted from explicit maps with fixed semantic classes to implicit open
vocabulary maps based on queryable embeddings capable of representing any
semantic class. However, embeddings cannot directly report the scene context as
they are implicit, requiring further processing for LLM integration. To address
this, we propose an explicit text-based map that can represent thousands of
semantic classes while easily integrating with LLMs due to their text-based
nature by building upon large-scale image recognition models. We study how
entities in our map can be localized and show through evaluations that our
text-based map localizations perform comparably to those from open vocabulary
maps while using two to four orders of magnitude less memory. Real-robot
experiments demonstrate the grounding of an LLM with the text-based map to
solve user tasks.

[Paper Link](
https://arxiv.org/abs/2409.15451
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_00-04.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Autotuning Bipedal Locomotion MPC with GRFM-Net for Efficient Sim-to-Real Transfer

- **Authors**: Qianzhong Chen, Junheng Li, Sheng Cheng, Naira Hovakimyan, Quan Nguyen

#### Abstract

Bipedal locomotion control is essential for humanoid robots to navigate
complex, human-centric environments. While optimization-based control designs
are popular for integrating sophisticated models of humanoid robots, they often
require labor-intensive manual tuning. In this work, we address the challenges
of parameter selection in bipedal locomotion control using DiffTune, a
model-based autotuning method that leverages differential programming for
efficient parameter learning. A major difficulty lies in balancing model
fidelity with differentiability. We address this difficulty using a
low-fidelity model for differentiability, enhanced by a Ground Reaction
Force-and-Moment Network (GRFM-Net) to capture discrepancies between MPC
commands and actual control effects. We validate the parameters learned by
DiffTune with GRFM-Net in hardware experiments, which demonstrates the
parameters' optimality in a multi-objective setting compared with baseline
parameters, reducing the total loss by up to 40.5$\%$ compared with the
expert-tuned parameters. The results confirm the GRFM-Net's effectiveness in
mitigating the sim-to-real gap, improving the transferability of
simulation-learned parameters to real hardware.

[Paper Link](
https://arxiv.org/abs/2409.15710
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-21_00-00.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-10-20


### A Learning Framework for Diverse Legged Robot Locomotion Using Barrier-Based Style Rewards

- **Authors**: Gijeong Kim, Yong-Hoon Lee, Hae-Won Park

#### Abstract

This work introduces a model-free reinforcement learning framework that
enables various modes of motion (quadruped, tripod, or biped) and diverse tasks
for legged robot locomotion. We employ a motion-style reward based on a relaxed
logarithmic barrier function as a soft constraint, to bias the learning process
toward the desired motion style, such as gait, foot clearance, joint position,
or body height. The predefined gait cycle is encoded in a flexible manner,
facilitating gait adjustments throughout the learning process. Extensive
experiments demonstrate that KAIST HOUND, a 45 kg robotic system, can achieve
biped, tripod, and quadruped locomotion using the proposed framework;
quadrupedal capabilities include traversing uneven terrain, galloping at 4.67
m/s, and overcoming obstacles up to 58 cm (67 cm for HOUND2); bipedal
capabilities include running at 3.6 m/s, carrying a 7.5 kg object, and
ascending stairs-all performed without exteroceptive input.

[Paper Link](
https://arxiv.org/abs/2409.15780
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-59.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### AnyCar to Anywhere: Learning Universal Dynamics Model for Agile and Adaptive Mobility

- **Authors**: Wenli Xiao, Haoru Xue, Tony Tao, Dvij Kalaria, John M. Dolan, Guanya Shi

#### Abstract

Recent works in the robot learning community have successfully introduced
generalist models capable of controlling various robot embodiments across a
wide range of tasks, such as navigation and locomotion. However, achieving
agile control, which pushes the limits of robotic performance, still relies on
specialist models that require extensive parameter tuning. To leverage
generalist-model adaptability and flexibility while achieving specialist-level
agility, we propose AnyCar, a transformer-based generalist dynamics model
designed for agile control of various wheeled robots. To collect training data,
we unify multiple simulators and leverage different physics backends to
simulate vehicles with diverse sizes, scales, and physical properties across
various terrains. With robust training and real-world fine-tuning, our model
enables precise adaptation to different vehicles, even in the wild and under
large state estimation errors. In real-world experiments, AnyCar shows both
few-shot and zero-shot generalization across a wide range of vehicles and
environments, where our model, combined with a sampling-based MPC, outperforms
specialist models by up to 54%. These results represent a key step toward
building a foundation model for agile wheeled robot control. We will also
open-source our framework to support further research.

[Paper Link](
https://arxiv.org/abs/2409.15783
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-58.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Whole-body end-effector pose tracking

- **Authors**: Tifanny Portela, Andrei Cramariuc, Mayank Mittal, Marco Hutter

#### Abstract

Combining manipulation with the mobility of legged robots is essential for a
wide range of robotic applications. However, integrating an arm with a mobile
base significantly increases the system's complexity, making precise
end-effector control challenging. Existing model-based approaches are often
constrained by their modeling assumptions, leading to limited robustness.
Meanwhile, recent Reinforcement Learning (RL) implementations restrict the
arm's workspace to be in front of the robot or track only the position to
obtain decent tracking accuracy. In this work, we address these limitations by
introducing a whole-body RL formulation for end-effector pose tracking in a
large workspace on rough, unstructured terrains. Our proposed method involves a
terrain-aware sampling strategy for the robot's initial configuration and
end-effector pose commands, as well as a game-based curriculum to extend the
robot's operating range. We validate our approach on the ANYmal quadrupedal
robot with a six DoF robotic arm. Through our experiments, we show that the
learned controller achieves precise command tracking over a large workspace and
adapts across varying terrains such as stairs and slopes. On deployment, it
achieves a pose-tracking error of 2.64 cm and 3.64 degrees, outperforming
existing competitive baselines.

[Paper Link](
https://arxiv.org/abs/2409.16048
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-53.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Gen2Act: Human Video Generation in Novel Scenarios enables Generalizable Robot Manipulation

- **Authors**: Homanga Bharadhwaj, Debidatta Dwibedi, Abhinav Gupta, Shubham Tulsiani, Carl Doersch, Ted Xiao, Dhruv Shah, Fei Xia, Dorsa Sadigh, Sean Kirmani

#### Abstract

How can robot manipulation policies generalize to novel tasks involving
unseen object types and new motions? In this paper, we provide a solution in
terms of predicting motion information from web data through human video
generation and conditioning a robot policy on the generated video. Instead of
attempting to scale robot data collection which is expensive, we show how we
can leverage video generation models trained on easily available web data, for
enabling generalization. Our approach Gen2Act casts language-conditioned
manipulation as zero-shot human video generation followed by execution with a
single policy conditioned on the generated video. To train the policy, we use
an order of magnitude less robot interaction data compared to what the video
prediction model was trained on. Gen2Act doesn't require fine-tuning the video
model at all and we directly use a pre-trained model for generating human
videos. Our results on diverse real-world scenarios show how Gen2Act enables
manipulating unseen object types and performing novel motions for tasks not
present in the robot data. Videos are at https://homangab.github.io/gen2act/

[Website Link](https://homangab.github.io/gen2act/)

[Paper Link](
https://arxiv.org/abs/2409.16283
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-51.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Articulated Object Manipulation using Online Axis Estimation with SAM2-Based Tracking

- **Authors**: Xi Wang, Tianxing Chen, Qiaojun Yu, Tianling Xu, Zanxin Chen, Yiting Fu, Cewu Lu, Yao Mu, Ping Luo

#### Abstract

Articulated object manipulation requires precise object interaction, where
the object's axis must be carefully considered. Previous research employed
interactive perception for manipulating articulated objects, but typically,
open-loop approaches often suffer from overlooking the interaction dynamics. To
address this limitation, we present a closed-loop pipeline integrating
interactive perception with online axis estimation from segmented 3D point
clouds. Our method leverages any interactive perception technique as a
foundation for interactive perception, inducing slight object movement to
generate point cloud frames of the evolving dynamic scene. These point clouds
are then segmented using Segment Anything Model 2 (SAM2), after which the
moving part of the object is masked for accurate motion online axis estimation,
guiding subsequent robotic actions. Our approach significantly enhances the
precision and efficiency of manipulation tasks involving articulated objects.
Experiments in simulated environments demonstrate that our method outperforms
baseline approaches, especially in tasks that demand precise axis-based
control. Project Page:
https://hytidel.github.io/video-tracking-for-axis-estimation/.

[Website Link](https://hytidel.github.io/video-tracking-for-axis-estimation/.)

[Paper Link](
https://arxiv.org/abs/2409.16287
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-50.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-24


### MaskedMimic: Unified Physics-Based Character Control Through Masked Motion Inpainting

- **Authors**: Chen Tessler, Yunrong Guo, Ofir Nabati, Gal Chechik, Xue Bin Peng

#### Abstract

Crafting a single, versatile physics-based controller that can breathe life
into interactive characters across a wide spectrum of scenarios represents an
exciting frontier in character animation. An ideal controller should support
diverse control modalities, such as sparse target keyframes, text instructions,
and scene information. While previous works have proposed physically simulated,
scene-aware control models, these systems have predominantly focused on
developing controllers that each specializes in a narrow set of tasks and
control modalities. This work presents MaskedMimic, a novel approach that
formulates physics-based character control as a general motion inpainting
problem. Our key insight is to train a single unified model to synthesize
motions from partial (masked) motion descriptions, such as masked keyframes,
objects, text descriptions, or any combination thereof. This is achieved by
leveraging motion tracking data and designing a scalable training method that
can effectively utilize diverse motion descriptions to produce coherent
animations. Through this process, our approach learns a physics-based
controller that provides an intuitive control interface without requiring
tedious reward engineering for all behaviors of interest. The resulting
controller supports a wide range of control modalities and enables seamless
transitions between disparate tasks. By unifying character control through
motion inpainting, MaskedMimic creates versatile virtual characters. These
characters can dynamically adapt to complex scenes and compose diverse motions
on demand, enabling more interactive and immersive experiences.

[Paper Link](
https://arxiv.org/abs/2409.14393
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-47.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### ScissorBot: Learning Generalizable Scissor Skill for Paper Cutting via Simulation, Imitation, and Sim2Real

- **Authors**: Jiangran Lyu, Yuxing Chen, Tao Du, Feng Zhu, Huiquan Liu, Yizhou Wang, He Wang

#### Abstract

This paper tackles the challenging robotic task of generalizable paper
cutting using scissors. In this task, scissors attached to a robot arm are
driven to accurately cut curves drawn on the paper, which is hung with the top
edge fixed. Due to the frequent paper-scissor contact and consequent fracture,
the paper features continual deformation and changing topology, which is
diffult for accurate modeling. To ensure effective execution, we customize an
action primitive sequence for imitation learning to constrain its action space,
thus alleviating potential compounding errors. Finally, by integrating
sim-to-real techniques to bridge the gap between simulation and reality, our
policy can be effectively deployed on the real robot. Experimental results
demonstrate that our method surpasses all baselines in both simulation and
real-world benchmarks and achieves performance comparable to human operation
with a single hand under the same conditions.

[Paper Link](
https://arxiv.org/abs/2409.13966
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-35.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### D3RoMa: Disparity Diffusion-based Depth Sensing for Material-Agnostic Robotic Manipulation

- **Authors**: Songlin Wei, Haoran Geng, Jiayi Chen, Congyue Deng, Wenbo Cui, Chengyang Zhao, Xiaomeng Fang, Leonidas Guibas, He Wang

#### Abstract

Depth sensing is an important problem for 3D vision-based robotics. Yet, a
real-world active stereo or ToF depth camera often produces noisy and
incomplete depth which bottlenecks robot performances. In this work, we propose
D3RoMa, a learning-based depth estimation framework on stereo image pairs that
predicts clean and accurate depth in diverse indoor scenes, even in the most
challenging scenarios with translucent or specular surfaces where classical
depth sensing completely fails. Key to our method is that we unify depth
estimation and restoration into an image-to-image translation problem by
predicting the disparity map with a denoising diffusion probabilistic model. At
inference time, we further incorporated a left-right consistency constraint as
classifier guidance to the diffusion process. Our framework combines recently
advanced learning-based approaches and geometric constraints from traditional
stereo vision. For model training, we create a large scene-level synthetic
dataset with diverse transparent and specular objects to compensate for
existing tabletop datasets. The trained model can be directly applied to
real-world in-the-wild scenes and achieve state-of-the-art performance in
multiple public depth estimation benchmarks. Further experiments in real
environments show that accurate depth prediction significantly improves robotic
manipulation in various scenarios.

[Paper Link](
https://arxiv.org/abs/2409.14365
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-32.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-23


### Towards Robust Automation of Surgical Systems via Digital Twin-based Scene Representations from Foundation Models

- **Authors**: Hao Ding, Lalithkumar Seenivasan, Hongchao Shu, Grayson Byrd, Han Zhang, Pu Xiao, Juan Antonio Barragan, Russell H. Taylor, Peter Kazanzides, Mathias Unberath

#### Abstract

Large language model-based (LLM) agents are emerging as a powerful enabler of
robust embodied intelligence due to their capability of planning complex action
sequences. Sound planning ability is necessary for robust automation in many
task domains, but especially in surgical automation. These agents rely on a
highly detailed natural language representation of the scene. Thus, to leverage
the emergent capabilities of LLM agents for surgical task planning, developing
similarly powerful and robust perception algorithms is necessary to derive a
detailed scene representation of the environment from visual input. Previous
research has focused primarily on enabling LLM-based task planning while
adopting simple yet severely limited perception solutions to meet the needs for
bench-top experiments but lack the critical flexibility to scale to less
constrained settings. In this work, we propose an alternate perception approach
-- a digital twin-based machine perception approach that capitalizes on the
convincing performance and out-of-the-box generalization of recent vision
foundation models. Integrating our digital twin-based scene representation and
LLM agent for planning with the dVRK platform, we develop an embodied
intelligence system and evaluate its robustness in performing peg transfer and
gauze retrieval tasks. Our approach shows strong task performance and
generalizability to varied environment settings. Despite convincing
performance, this work is merely a first step towards the integration of
digital twin-based scene representations. Future studies are necessary for the
realization of a comprehensive digital twin framework to improve the
interpretability and generalizability of embodied intelligence in surgery.

[Paper Link](
https://arxiv.org/abs/2409.13107
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-20.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### SoloParkour: Constrained Reinforcement Learning for Visual Locomotion from Privileged Experience

- **Authors**: Elliot Chane-Sane, Joseph Amigo, Thomas Flayols, Ludovic Righetti, Nicolas Mansard

#### Abstract

Parkour poses a significant challenge for legged robots, requiring navigation
through complex environments with agility and precision based on limited
sensory inputs. In this work, we introduce a novel method for training
end-to-end visual policies, from depth pixels to robot control commands, to
achieve agile and safe quadruped locomotion. We formulate robot parkour as a
constrained reinforcement learning (RL) problem designed to maximize the
emergence of agile skills within the robot's physical limits while ensuring
safety. We first train a policy without vision using privileged information
about the robot's surroundings. We then generate experience from this
privileged policy to warm-start a sample efficient off-policy RL algorithm from
depth images. This allows the robot to adapt behaviors from this privileged
experience to visual locomotion while circumventing the high computational
costs of RL directly from pixels. We demonstrate the effectiveness of our
method on a real Solo-12 robot, showcasing its capability to perform a variety
of parkour skills such as walking, climbing, leaping, and crawling.

[Paper Link](
https://arxiv.org/abs/2409.13678
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-13.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-20


### Extended Reality System for Robotic Learning from Human Demonstration

- **Authors**: Isaac Ngui, Courtney McBeth, Grace He, André Corrêa Santos, Luciano Soares, Marco Morales, Nancy M. Amato

#### Abstract

Many real-world tasks are intuitive for a human to perform, but difficult to
encode algorithmically when utilizing a robot to perform the tasks. In these
scenarios, robotic systems can benefit from expert demonstrations to learn how
to perform each task. In many settings, it may be difficult or unsafe to use a
physical robot to provide these demonstrations, for example, considering
cooking tasks such as slicing with a knife. Extended reality provides a natural
setting for demonstrating robotic trajectories while bypassing safety concerns
and providing a broader range of interaction modalities. We propose the Robot
Action Demonstration in Extended Reality (RADER) system, a generic extended
reality interface for learning from demonstration. We additionally present its
application to an existing state-of-the-art learning from demonstration
approach and show comparable results between demonstrations given on a physical
robot and those given using our extended reality system.

[Paper Link](
https://arxiv.org/abs/2409.12862
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_23-06.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-19


### Generalized Robot Learning Framework

- **Authors**: Jiahuan Yan, Zhouyang Hong, Yu Zhao, Yu Tian, Yunxin Liu, Travis Davies, Luhui Hu

#### Abstract

Imitation based robot learning has recently gained significant attention in
the robotics field due to its theoretical potential for transferability and
generalizability. However, it remains notoriously costly, both in terms of
hardware and data collection, and deploying it in real-world environments
demands meticulous setup of robots and precise experimental conditions. In this
paper, we present a low-cost robot learning framework that is both easily
reproducible and transferable to various robots and environments. We
demonstrate that deployable imitation learning can be successfully applied even
to industrial-grade robots, not just expensive collaborative robotic arms.
Furthermore, our results show that multi-task robot learning is achievable with
simple network architectures and fewer demonstrations than previously thought
necessary. As the current evaluating method is almost subjective when it comes
to real-world manipulation tasks, we propose Voting Positive Rate (VPR) - a
novel evaluation strategy that provides a more objective assessment of
performance. We conduct an extensive comparison of success rates across various
self-designed tasks to validate our approach. To foster collaboration and
support the robot learning community, we have open-sourced all relevant
datasets and model checkpoints, available at huggingface.co/ZhiChengAI.

[Paper Link](
https://arxiv.org/abs/2409.12061
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_22-52.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### An Efficient Projection-Based Next-best-view Planning Framework for Reconstruction of Unknown Objects

- **Authors**: Zhizhou Jia, Shaohui Zhang, Qun Hao

#### Abstract

Efficiently and completely capturing the three-dimensional data of an object
is a fundamental problem in industrial and robotic applications. The task of
next-best-view (NBV) planning is to infer the pose of the next viewpoint based
on the current data, and gradually realize the complete three-dimensional
reconstruction. Many existing algorithms, however, suffer a large computational
burden due to the use of ray-casting. To address this, this paper proposes a
projection-based NBV planning framework. It can select the next best view at an
extremely fast speed while ensuring the complete scanning of the object.
Specifically, this framework refits different types of voxel clusters into
ellipsoids based on the voxel structure.Then, the next best view is selected
from the candidate views using a projection-based viewpoint quality evaluation
function in conjunction with a global partitioning strategy. This process
replaces the ray-casting in voxel structures, significantly improving the
computational efficiency. Comparative experiments with other algorithms in a
simulation environment show that the framework proposed in this paper can
achieve 10 times efficiency improvement on the basis of capturing roughly the
same coverage. The real-world experimental results also prove the efficiency
and feasibility of the framework.

[Paper Link](
https://arxiv.org/abs/2409.12096
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_13-12.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### DynaMo: In-Domain Dynamics Pretraining for Visuo-Motor Control

- **Authors**: Zichen Jeff Cui, Hengkai Pan, Aadhithya Iyer, Siddhant Haldar, Lerrel Pinto

#### Abstract

Imitation learning has proven to be a powerful tool for training complex
visuomotor policies. However, current methods often require hundreds to
thousands of expert demonstrations to handle high-dimensional visual
observations. A key reason for this poor data efficiency is that visual
representations are predominantly either pretrained on out-of-domain data or
trained directly through a behavior cloning objective. In this work, we present
DynaMo, a new in-domain, self-supervised method for learning visual
representations. Given a set of expert demonstrations, we jointly learn a
latent inverse dynamics model and a forward dynamics model over a sequence of
image embeddings, predicting the next frame in latent space, without
augmentations, contrastive sampling, or access to ground truth actions.
Importantly, DynaMo does not require any out-of-domain data such as Internet
datasets or cross-embodied datasets. On a suite of six simulated and real
environments, we show that representations learned with DynaMo significantly
improve downstream imitation learning performance over prior self-supervised
learning objectives, and pretrained representations. Gains from using DynaMo
hold across policy classes such as Behavior Transformer, Diffusion Policy, MLP,
and nearest neighbors. Finally, we ablate over key components of DynaMo and
measure its impact on downstream policy performance. Robot videos are best
viewed at https://dynamo-ssl.github.io

[Website Link](https://dynamo-ssl.github.io)

[Paper Link](
https://arxiv.org/abs/2409.12192
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_13-09.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-18


### Agile Continuous Jumping in Discontinuous Terrains

- **Authors**: Yuxiang Yang, Guanya Shi, Changyi Lin, Xiangyun Meng, Rosario Scalise, Mateo Guaman Castro, Wenhao Yu, Tingnan Zhang, Ding Zhao, Jie Tan, Byron Boots

#### Abstract

We focus on agile, continuous, and terrain-adaptive jumping of quadrupedal
robots in discontinuous terrains such as stairs and stepping stones. Unlike
single-step jumping, continuous jumping requires accurately executing highly
dynamic motions over long horizons, which is challenging for existing
approaches. To accomplish this task, we design a hierarchical learning and
control framework, which consists of a learned heightmap predictor for robust
terrain perception, a reinforcement-learning-based centroidal-level motion
policy for versatile and terrain-adaptive planning, and a low-level model-based
leg controller for accurate motion tracking. In addition, we minimize the
sim-to-real gap by accurately modeling the hardware characteristics. Our
framework enables a Unitree Go1 robot to perform agile and continuous jumps on
human-sized stairs and sparse stepping stones, for the first time to the best
of our knowledge. In particular, the robot can cross two stair steps in each
jump and completes a 3.5m long, 2.8m high, 14-step staircase in 4.5 seconds.
Moreover, the same policy outperforms baselines in various other parkour tasks,
such as jumping over single horizontal or vertical discontinuities. Experiment
videos can be found at https://yxyang.github.io/jumping_cod/

[Website Link](https://yxyang.github.io/jumping_cod/)

[Paper Link](
https://arxiv.org/abs/2409.10923
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_11-11.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### MoDex: Planning High-Dimensional Dexterous Control via Learning Neural Hand Models

- **Authors**: Tong Wu, Shoujie Li, Chuqiao Lyu, Kit-Wa Sou, Wang-Sing Chan, Wenbo Ding

#### Abstract

Controlling hands in the high-dimensional action space has been a
longstanding challenge, yet humans naturally perform dexterous tasks with ease.
In this paper, we draw inspiration from the human embodied cognition and
reconsider dexterous hands as learnable systems. Specifically, we introduce
MoDex, a framework which employs a neural hand model to capture the dynamical
characteristics of hand movements. Based on the model, a bidirectional planning
method is developed, which demonstrates efficiency in both training and
inference. The method is further integrated with a large language model to
generate various gestures such as ``Scissorshand" and ``Rock\&Roll." Moreover,
we show that decomposing the system dynamics into a pretrained hand model and
an external model improves data efficiency, as supported by both theoretical
analysis and empirical experiments. Additional visualization results are
available at https://tongwu19.github.io/MoDex.

[Website Link](https://tongwu19.github.io/MoDex.)

[Paper Link](
https://arxiv.org/abs/2409.10983
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_11-06.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### TacDiffusion: Force-domain Diffusion Policy for Precise Tactile Manipulation

- **Authors**: Yansong Wu, Zongxie Chen, Fan Wu, Lingyun Chen, Liding Zhang, Zhenshan Bing, Abdalla Swikir, Alois Knoll, Sami Haddadin

#### Abstract

Assembly is a crucial skill for robots in both modern manufacturing and
service robotics. However, mastering transferable insertion skills that can
handle a variety of high-precision assembly tasks remains a significant
challenge. This paper presents a novel framework that utilizes diffusion models
to generate 6D wrench for high-precision tactile robotic insertion tasks. It
learns from demonstrations performed on a single task and achieves a zero-shot
transfer success rate of 95.7% across various novel high-precision tasks. Our
method effectively inherits the self-adaptability demonstrated by our previous
work. In this framework, we address the frequency misalignment between the
diffusion policy and the real-time control loop with a dynamic system-based
filter, significantly improving the task success rate by 9.15%. Furthermore, we
provide a practical guideline regarding the trade-off between diffusion models'
inference ability and speed.

[Paper Link](
https://arxiv.org/abs/2409.11047
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_10-58.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Use the Force, Bot! -- Force-Aware ProDMP with Event-Based Replanning

- **Authors**: Paul Werner Lödige, Maximilian Xiling Li, Rudolf Lioutikov

#### Abstract

Movement Primitives (MPs) are a well-established method for representing and
generating modular robot trajectories. This work presents FA-ProDMP, a new
approach which introduces force awareness to Probabilistic Dynamic Movement
Primitives (ProDMP). FA-ProDMP adapts the trajectory during runtime to account
for measured and desired forces. It offers smooth trajectories and captures
position and force correlations over multiple trajectories, e.g. a set of human
demonstrations. FA-ProDMP supports multiple axes of force and is thus agnostic
to cartesian or joint space control. This makes FA-ProDMP a valuable tool for
learning contact rich manipulation tasks such as polishing, cutting or
industrial assembly from demonstration. In order to reliably evaluate
FA-ProDMP, this work additionally introduces a modular, 3D printed task suite
called POEMPEL, inspired by the popular Lego Technic pins. POEMPEL mimics
industrial peg-in-hole assembly tasks with force requirements. It offers
multiple parameters of adjustment, such as position, orientation and plug
stiffness level, thus varying the direction and amount of required forces. Our
experiments show that FA-ProDMP outperforms other MP formulations on the
POEMPEL setup and a electrical power plug insertion task, due to its replanning
capabilities based on the measured forces. These findings highlight how
FA-ProDMP enhances the performance of robotic systems in contact-rich
manipulation tasks.

[Paper Link](
https://arxiv.org/abs/2409.11144
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-20_10-56.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-17


### Learning to enhance multi-legged robot on rugged landscapes

- **Authors**: Juntao He, Baxi Chong, Zhaochen Xu, Sehoon Ha, Daniel I. Goldman

#### Abstract

Navigating rugged landscapes poses significant challenges for legged
locomotion. Multi-legged robots (those with 6 and greater) offer a promising
solution for such terrains, largely due to their inherent high static
stability, resulting from a low center of mass and wide base of support. Such
systems require minimal effort to maintain balance. Recent studies have shown
that a linear controller, which modulates the vertical body undulation of a
multi-legged robot in response to shifts in terrain roughness, can ensure
reliable mobility on challenging terrains. However, the potential of a
learning-based control framework that adjusts multiple parameters to address
terrain heterogeneity remains underexplored. We posit that the development of
an experimentally validated physics-based simulator for this robot can rapidly
advance capabilities by allowing wide parameter space exploration. Here we
develop a MuJoCo-based simulator tailored to this robotic platform and use the
simulation to develop a reinforcement learning-based control framework that
dynamically adjusts horizontal and vertical body undulation, and limb stepping
in real-time. Our approach improves robot performance in simulation, laboratory
experiments, and outdoor tests. Notably, our real-world experiments reveal that
the learning-based controller achieves a 30\% to 50\% increase in speed
compared to a linear controller, which only modulates vertical body waves. We
hypothesize that the superior performance of the learning-based controller
arises from its ability to adjust multiple parameters simultaneously, including
limb stepping, horizontal body wave, and vertical body wave.

[Paper Link](
https://arxiv.org/abs/2409.09473
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-46.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Robots with Attitude: Singularity-Free Quaternion-Based Model-Predictive Control for Agile Legged Robots

- **Authors**: Zixin Zhang, John Z. Zhang, Shuo Yang, Zachary Manchester

#### Abstract

We present a model-predictive control (MPC) framework for legged robots that
avoids the singularities associated with common three-parameter attitude
representations like Euler angles during large-angle rotations. Our method
parameterizes the robot's attitude with singularity-free unit quaternions and
makes modifications to the iterative linear-quadratic regulator (iLQR)
algorithm to deal with the resulting geometry. The derivation of our algorithm
requires only elementary calculus and linear algebra, deliberately avoiding the
abstraction and notation of Lie groups. We demonstrate the performance and
computational efficiency of quaternion MPC in several experiments on quadruped
and humanoid robots.

[Paper Link](
https://arxiv.org/abs/2409.09940
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-43.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### SplatSim: Zero-Shot Sim2Real Transfer of RGB Manipulation Policies Using Gaussian Splatting

- **Authors**: Mohammad Nomaan Qureshi, Sparsh Garg, Francisco Yandun, David Held, George Kantor, Abhisesh Silwal

#### Abstract

Sim2Real transfer, particularly for manipulation policies relying on RGB
images, remains a critical challenge in robotics due to the significant domain
shift between synthetic and real-world visual data. In this paper, we propose
SplatSim, a novel framework that leverages Gaussian Splatting as the primary
rendering primitive to reduce the Sim2Real gap for RGB-based manipulation
policies. By replacing traditional mesh representations with Gaussian Splats in
simulators, SplatSim produces highly photorealistic synthetic data while
maintaining the scalability and cost-efficiency of simulation. We demonstrate
the effectiveness of our framework by training manipulation policies within
SplatSim and deploying them in the real world in a zero-shot manner, achieving
an average success rate of 86.25%, compared to 97.5% for policies trained on
real-world data. Videos can be found on our project page:
https://splatsim.github.io

[Website Link](https://splatsim.github.io)

[Paper Link](
https://arxiv.org/abs/2409.10161
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-40.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Know your limits! Optimize the robot's behavior through self-awareness

- **Authors**: Esteve Valls Mascaro, Dongheui Lee

#### Abstract

As humanoid robots transition from labs to real-world environments, it is
essential to democratize robot control for non-expert users. Recent human-robot
imitation algorithms focus on following a reference human motion with high
precision, but they are susceptible to the quality of the reference motion and
require the human operator to simplify its movements to match the robot's
capabilities. Instead, we consider that the robot should understand and adapt
the reference motion to its own abilities, facilitating the operator's task.
For that, we introduce a deep-learning model that anticipates the robot's
performance when imitating a given reference. Then, our system can generate
multiple references given a high-level task command, assign a score to each of
them, and select the best reference to achieve the desired robot behavior. Our
Self-AWare model (SAW) ranks potential robot behaviors based on various
criteria, such as fall likelihood, adherence to the reference motion, and
smoothness. We integrate advanced motion generation, robot control, and SAW in
one unique system, ensuring optimal robot behavior for any task command. For
instance, SAW can anticipate falls with 99.29% accuracy. For more information
check our project page: https://evm7.github.io/Self-AWare

[Website Link](https://evm7.github.io/Self-AWare)

[Paper Link](
https://arxiv.org/abs/2409.10308
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-37.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Catch It! Learning to Catch in Flight with Mobile Dexterous Hands

- **Authors**: Yuanhang Zhang, Tianhai Liang, Zhenyang Chen, Yanjie Ze, Huazhe Xu

#### Abstract

Catching objects in flight (i.e., thrown objects) is a common daily skill for
humans, yet it presents a significant challenge for robots. This task requires
a robot with agile and accurate motion, a large spatial workspace, and the
ability to interact with diverse objects. In this paper, we build a mobile
manipulator composed of a mobile base, a 6-DoF arm, and a 12-DoF dexterous hand
to tackle such a challenging task. We propose a two-stage reinforcement
learning framework to efficiently train a whole-body-control catching policy
for this high-DoF system in simulation. The objects' throwing configurations,
shapes, and sizes are randomized during training to enhance policy adaptivity
to various trajectories and object characteristics in flight. The results show
that our trained policy catches diverse objects with randomly thrown
trajectories, at a high success rate of about 80\% in simulation, with a
significant improvement over the baselines. The policy trained in simulation
can be directly deployed in the real world with onboard sensing and
computation, which achieves catching sandbags in various shapes, randomly
thrown by humans. Our project page is available at
https://mobile-dex-catch.github.io/.

[Website Link](https://mobile-dex-catch.github.io/.)

[Paper Link](
https://arxiv.org/abs/2409.10319
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-36.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Digital Twins Meet the Koopman Operator: Data-Driven Learning for Robust Autonomy

- **Authors**: Chinmay Vilas Samak, Tanmay Vilas Samak, Ajinkya Joglekar, Umesh Vaidya, Venkat Krovi

#### Abstract

Contrary to on-road autonomous navigation, off-road autonomy is complicated
by various factors ranging from sensing challenges to terrain variability. In
such a milieu, data-driven approaches have been commonly employed to capture
intricate vehicle-environment interactions effectively. However, the success of
data-driven methods depends crucially on the quality and quantity of data,
which can be compromised by large variability in off-road environments. To
address these concerns, we present a novel workflow to recreate the exact
vehicle and its target operating conditions digitally for domain-specific data
generation. This enables us to effectively model off-road vehicle dynamics from
simulation data using the Koopman operator theory, and employ the obtained
models for local motion planning and optimal vehicle control. The capabilities
of the proposed methodology are demonstrated through an autonomous navigation
problem of a 1:5 scale vehicle, where a terrain-informed planner is employed
for global mission planning. Results indicate a substantial improvement in
off-road navigation performance with the proposed algorithm (5.84x) and
underscore the efficacy of digital twinning in terms of improving the sample
efficiency (3.2x) and reducing the sim2real gap (5.2%).

[Paper Link](
https://arxiv.org/abs/2409.10347
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-35.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Point2Graph: An End-to-end Point Cloud-based 3D Open-Vocabulary Scene Graph for Robot Navigation

- **Authors**: Yifan Xu, Ziming Luo, Qianwei Wang, Vineet Kamat, Carol Menassa

#### Abstract

Current open-vocabulary scene graph generation algorithms highly rely on both
3D scene point cloud data and posed RGB-D images and thus have limited
applications in scenarios where RGB-D images or camera poses are not readily
available. To solve this problem, we propose Point2Graph, a novel end-to-end
point cloud-based 3D open-vocabulary scene graph generation framework in which
the requirement of posed RGB-D image series is eliminated. This hierarchical
framework contains room and object detection/segmentation and open-vocabulary
classification. For the room layer, we leverage the advantage of merging the
geometry-based border detection algorithm with the learning-based region
detection to segment rooms and create a "Snap-Lookup" framework for
open-vocabulary room classification. In addition, we create an end-to-end
pipeline for the object layer to detect and classify 3D objects based solely on
3D point cloud data. Our evaluation results show that our framework can
outperform the current state-of-the-art (SOTA) open-vocabulary object and room
segmentation and classification algorithm on widely used real-scene datasets.

[Paper Link](
https://arxiv.org/abs/2409.10350
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-34.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Real-Time Whole-Body Control of Legged Robots with Model-Predictive Path Integral Control

- **Authors**: Juan Alvarez-Padilla, John Z. Zhang, Sofia Kwok, John M. Dolan, Zachary Manchester

#### Abstract

This paper presents a system for enabling real-time synthesis of whole-body
locomotion and manipulation policies for real-world legged robots. Motivated by
recent advancements in robot simulation, we leverage the efficient
parallelization capabilities of the MuJoCo simulator to achieve fast sampling
over the robot state and action trajectories. Our results show surprisingly
effective real-world locomotion and manipulation capabilities with a very
simple control strategy. We demonstrate our approach on several hardware and
simulation experiments: robust locomotion over flat and uneven terrains,
climbing over a box whose height is comparable to the robot, and pushing a box
to a goal position. To our knowledge, this is the first successful deployment
of whole-body sampling-based MPC on real-world legged robot hardware.
Experiment videos and code can be found at: https://whole-body-mppi.github.io/

[Website Link](https://whole-body-mppi.github.io/)

[Paper Link](
https://arxiv.org/abs/2409.10469
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-33.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-16


### EHC-MM: Embodied Holistic Control for Mobile Manipulation

- **Authors**: Jiawen Wang, Yixiang Jin, Jun Shi, Yong A, Dingzhe Li, Bin Fang, Fuchun Sun

#### Abstract

Mobile manipulation typically entails the base for mobility, the arm for
accurate manipulation, and the camera for perception. It is necessary to follow
the principle of Distant Mobility, Close Grasping(DMCG) in holistic control. We
propose Embodied Holistic Control for Mobile Manipulation(EHC-MM) with the
embodied function of sig(w): By formulating the DMCG principle as a Quadratic
Programming (QP) problem, sig(w) dynamically balances the robot's emphasis
between movement and manipulation with the consideration of the robot's state
and environment. In addition, we propose the Monitor-Position-Based Servoing
(MPBS) with sig(w), enabling the tracking of the target during the operation.
This approach allows coordinated control between the robot's base, arm, and
camera. Through extensive simulations and real-world experiments, our approach
significantly improves both the success rate and efficiency of mobile
manipulation tasks, achieving a 95.6% success rate in the real-world scenarios
and a 52.8% increase in time efficiency.

[Paper Link](
https://arxiv.org/abs/2409.08527
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-31.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### DexSim2Real$^{2}$: Building Explicit World Model for Precise Articulated Object Dexterous Manipulation

- **Authors**: Taoran Jiang, Liqian Ma, Yixuan Guan, Jiaojiao Meng, Weihang Chen, Zecui Zeng, Lusong Li, Dan Wu, Jing Xu, Rui Chen

#### Abstract

Articulated object manipulation is ubiquitous in daily life. In this paper,
we present DexSim2Real$^{2}$, a novel robot learning framework for
goal-conditioned articulated object manipulation using both two-finger grippers
and multi-finger dexterous hands. The key of our framework is constructing an
explicit world model of unseen articulated objects through active one-step
interactions. This explicit world model enables sampling-based model predictive
control to plan trajectories achieving different manipulation goals without
needing human demonstrations or reinforcement learning. It first predicts an
interaction motion using an affordance estimation network trained on
self-supervised interaction data or videos of human manipulation from the
internet. After executing this interaction on the real robot, the framework
constructs a digital twin of the articulated object in simulation based on the
two point clouds before and after the interaction. For dexterous multi-finger
manipulation, we propose to utilize eigengrasp to reduce the high-dimensional
action space, enabling more efficient trajectory searching. Extensive
experiments validate the framework's effectiveness for precise articulated
object manipulation in both simulation and the real world using a two-finger
gripper and a 16-DoF dexterous hand. The robust generalizability of the
explicit world model also enables advanced manipulation strategies, such as
manipulating with different tools.

[Paper Link](
https://arxiv.org/abs/2409.08750
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-26.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### AnyBipe: An End-to-End Framework for Training and Deploying Bipedal Robots Guided by Large Language Models

- **Authors**: Yifei Yao, Wentao He, Chenyu Gu, Jiaheng Du, Fuwei Tan, Zhen Zhu, Junguo Lu

#### Abstract

Training and deploying reinforcement learning (RL) policies for robots,
especially in accomplishing specific tasks, presents substantial challenges.
Recent advancements have explored diverse reward function designs, training
techniques, simulation-to-reality (sim-to-real) transfers, and performance
analysis methodologies, yet these still require significant human intervention.
This paper introduces an end-to-end framework for training and deploying RL
policies, guided by Large Language Models (LLMs), and evaluates its
effectiveness on bipedal robots. The framework consists of three interconnected
modules: an LLM-guided reward function design module, an RL training module
leveraging prior work, and a sim-to-real homomorphic evaluation module. This
design significantly reduces the need for human input by utilizing only
essential simulation and deployment platforms, with the option to incorporate
human-engineered strategies and historical data. We detail the construction of
these modules, their advantages over traditional approaches, and demonstrate
the framework's capability to autonomously develop and refine controlling
strategies for bipedal robot locomotion, showcasing its potential to operate
independently of human intervention.

[Paper Link](
https://arxiv.org/abs/2409.08904
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-25_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### ClearDepth: Enhanced Stereo Perception of Transparent Objects for Robotic Manipulation

- **Authors**: Kaixin Bai, Huajian Zeng, Lei Zhang, Yiwen Liu, Hongli Xu, Zhaopeng Chen, Jianwei Zhang

#### Abstract

Transparent object depth perception poses a challenge in everyday life and
logistics, primarily due to the inability of standard 3D sensors to accurately
capture depth on transparent or reflective surfaces. This limitation
significantly affects depth map and point cloud-reliant applications,
especially in robotic manipulation. We developed a vision transformer-based
algorithm for stereo depth recovery of transparent objects. This approach is
complemented by an innovative feature post-fusion module, which enhances the
accuracy of depth recovery by structural features in images. To address the
high costs associated with dataset collection for stereo camera-based
perception of transparent objects, our method incorporates a parameter-aligned,
domain-adaptive, and physically realistic Sim2Real simulation for efficient
data generation, accelerated by AI algorithm. Our experimental results
demonstrate the model's exceptional Sim2Real generalizability in real-world
scenarios, enabling precise depth mapping of transparent objects to assist in
robotic manipulation. Project details are available at
https://sites.google.com/view/cleardepth/ .

[Website Link](https://sites.google.com/view/cleardepth/)

[Paper Link](
https://arxiv.org/abs/2409.08926
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-25.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-13


### An Open-Source Soft Robotic Platform for Autonomous Aerial Manipulation in the Wild

- **Authors**: Erik Bauer, Marc Blöchlinger, Pascal Strauch, Arman Raayatsanati, Curdin Cavelti, Robert K. Katzschmann

#### Abstract

Aerial manipulation combines the versatility and speed of flying platforms
with the functional capabilities of mobile manipulation, which presents
significant challenges due to the need for precise localization and control.
Traditionally, researchers have relied on offboard perception systems, which
are limited to expensive and impractical specially equipped indoor
environments. In this work, we introduce a novel platform for autonomous aerial
manipulation that exclusively utilizes onboard perception systems. Our platform
can perform aerial manipulation in various indoor and outdoor environments
without depending on external perception systems. Our experimental results
demonstrate the platform's ability to autonomously grasp various objects in
diverse settings. This advancement significantly improves the scalability and
practicality of aerial manipulation applications by eliminating the need for
costly tracking solutions. To accelerate future research, we open source our
ROS 2 software stack and custom hardware design, making our contributions
accessible to the broader research community.

[Paper Link](
https://arxiv.org/abs/2409.07662
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-22.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### InterACT: Inter-dependency Aware Action Chunking with Hierarchical Attention Transformers for Bimanual Manipulation

- **Authors**: Andrew Lee, Ian Chuang, Ling-Yuan Chen, Iman Soltani

#### Abstract

Bimanual manipulation presents unique challenges compared to unimanual tasks
due to the complexity of coordinating two robotic arms. In this paper, we
introduce InterACT: Inter-dependency aware Action Chunking with Hierarchical
Attention Transformers, a novel imitation learning framework designed
specifically for bimanual manipulation. InterACT leverages hierarchical
attention mechanisms to effectively capture inter-dependencies between dual-arm
joint states and visual inputs. The framework comprises a Hierarchical
Attention Encoder, which processes multi-modal inputs through segment-wise and
cross-segment attention mechanisms, and a Multi-arm Decoder that generates each
arm's action predictions in parallel, while sharing information between the
arms through synchronization blocks by providing the other arm's intermediate
output as context. Our experiments, conducted on various simulated and
real-world bimanual manipulation tasks, demonstrate that InterACT outperforms
existing methods. Detailed ablation studies further validate the significance
of key components, including the impact of CLS tokens, cross-segment encoders,
and synchronization blocks on task performance. We provide supplementary
materials and videos on our project page.

[Paper Link](
https://arxiv.org/abs/2409.07914
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-21_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Universal Trajectory Optimization Framework for Differential Drive Robot Class

- **Authors**: Mengke Zhang, Nanhe Chen, Hu Wang, Jianxiong Qiu, Zhichao Han, Qiuyu Ren, Chao Xu, Fei Gao, Yanjun Cao

#### Abstract

Differential drive robots are widely used in various scenarios thanks to
their straightforward principle, from household service robots to disaster
response field robots. There are several types of driving mechanisms for
real-world applications, including two-wheeled, four-wheeled skid-steering,
tracked robots, and so on. The differences in the driving mechanisms usually
require specific kinematic modeling when precise control is desired.
Furthermore, the nonholonomic dynamics and possible lateral slip lead to
different degrees of difficulty in getting feasible and high-quality
trajectories. Therefore, a comprehensive trajectory optimization framework to
compute trajectories efficiently for various kinds of differential drive robots
is highly desirable. In this paper, we propose a universal trajectory
optimization framework that can be applied to differential drive robots,
enabling the generation of high-quality trajectories within a restricted
computational timeframe. We introduce a novel trajectory representation based
on polynomial parameterization of motion states or their integrals, such as
angular and linear velocities, which inherently matches the robots' motion to
the control principle. The trajectory optimization problem is formulated to
minimize complexity while prioritizing safety and operational efficiency. We
then build a full-stack autonomous planning and control system to demonstrate
its feasibility and robustness. We conduct extensive simulations and real-world
testing in crowded environments with three kinds of differential drive robots
to validate the effectiveness of our approach.

[Paper Link](
https://arxiv.org/abs/2409.07924
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-21.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Touch2Touch: Cross-Modal Tactile Generation for Object Manipulation

- **Authors**: Samanta Rodriguez, Yiming Dou, Miquel Oller, Andrew Owens, Nima Fazeli

#### Abstract

Today's touch sensors come in many shapes and sizes. This has made it
challenging to develop general-purpose touch processing methods since models
are generally tied to one specific sensor design. We address this problem by
performing cross-modal prediction between touch sensors: given the tactile
signal from one sensor, we use a generative model to estimate how the same
physical contact would be perceived by another sensor. This allows us to apply
sensor-specific methods to the generated signal. We implement this idea by
training a diffusion model to translate between the popular GelSlim and Soft
Bubble sensors. As a downstream task, we perform in-hand object pose estimation
using GelSlim sensors while using an algorithm that operates only on Soft
Bubble signals. The dataset, the code, and additional details can be found at
https://www.mmintlab.com/research/touch2touch/.

[Website Link](https://www.mmintlab.com/research/touch2touch/.)

[Paper Link](
https://arxiv.org/abs/2409.08269
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-20_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Hand-Object Interaction Pretraining from Videos

- **Authors**: Himanshu Gaurav Singh, Antonio Loquercio, Carmelo Sferrazza, Jane Wu, Haozhi Qi, Pieter Abbeel, Jitendra Malik

#### Abstract

We present an approach to learn general robot manipulation priors from 3D
hand-object interaction trajectories. We build a framework to use in-the-wild
videos to generate sensorimotor robot trajectories. We do so by lifting both
the human hand and the manipulated object in a shared 3D space and retargeting
human motions to robot actions. Generative modeling on this data gives us a
task-agnostic base policy. This policy captures a general yet flexible
manipulation prior. We empirically demonstrate that finetuning this policy,
with both reinforcement learning (RL) and behavior cloning (BC), enables
sample-efficient adaptation to downstream tasks and simultaneously improves
robustness and generalizability compared to prior approaches. Qualitative
experiments are available at: \url{https://hgaurav2k.github.io/hop/}.

[Website Link](https://hgaurav2k.github.io/hop/)

[Paper Link](
https://arxiv.org/abs/2409.08273
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-20.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### AnySkin: Plug-and-play Skin Sensing for Robotic Touch

- **Authors**: Raunaq Bhirangi, Venkatesh Pattabiraman, Enes Erciyes, Yifeng Cao, Tess Hellebrekers, Lerrel Pinto

#### Abstract

While tactile sensing is widely accepted as an important and useful sensing
modality, its use pales in comparison to other sensory modalities like vision
and proprioception. AnySkin addresses the critical challenges that impede the
use of tactile sensing -- versatility, replaceability, and data reusability.
Building on the simplistic design of ReSkin, and decoupling the sensing
electronics from the sensing interface, AnySkin simplifies integration making
it as straightforward as putting on a phone case and connecting a charger.
Furthermore, AnySkin is the first uncalibrated tactile-sensor with
cross-instance generalizability of learned manipulation policies. To summarize,
this work makes three key contributions: first, we introduce a streamlined
fabrication process and a design tool for creating an adhesive-free, durable
and easily replaceable magnetic tactile sensor; second, we characterize slip
detection and policy learning with the AnySkin sensor; and third, we
demonstrate zero-shot generalization of models trained on one instance of
AnySkin to new instances, and compare it with popular existing tactile
solutions like DIGIT and ReSkin. Videos of experiments, fabrication details and
design files can be found on https://any-skin.github.io/

[Website Link](https://any-skin.github.io/)

[Paper Link](
https://arxiv.org/abs/2409.08276
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-19.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-12


### Single-View 3D Reconstruction via SO(2)-Equivariant Gaussian Sculpting Networks

- **Authors**: Ruihan Xu, Anthony Opipari, Joshua Mah, Stanley Lewis, Haoran Zhang, Hanzhe Guo, Odest Chadwicke Jenkins

#### Abstract

This paper introduces SO(2)-Equivariant Gaussian Sculpting Networks (GSNs) as
an approach for SO(2)-Equivariant 3D object reconstruction from single-view
image observations.
  GSNs take a single observation as input to generate a Gaussian splat
representation describing the observed object's geometry and texture. By using
a shared feature extractor before decoding Gaussian colors, covariances,
positions, and opacities, GSNs achieve extremely high throughput (>150FPS).
Experiments demonstrate that GSNs can be trained efficiently using a multi-view
rendering loss and are competitive, in quality, with expensive diffusion-based
reconstruction algorithms. The GSN model is validated on multiple benchmark
experiments. Moreover, we demonstrate the potential for GSNs to be used within
a robotic manipulation pipeline for object-centric grasping.

[Paper Link](
https://arxiv.org/abs/2409.07245
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-18.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### End-to-End and Highly-Efficient Differentiable Simulation for Robotics

- **Authors**: Quentin Le Lidec, Louis Montaut, Yann de Mont-Marin, Justin Carpentier

#### Abstract

Over the past few years, robotics simulators have largely improved in
efficiency and scalability, enabling them to generate years of simulated data
in a few hours. Yet, efficiently and accurately computing the simulation
derivatives remains an open challenge, with potentially high gains on the
convergence speed of reinforcement learning and trajectory optimization
algorithms, especially for problems involving physical contact interactions.
This paper contributes to this objective by introducing a unified and efficient
algorithmic solution for computing the analytical derivatives of robotic
simulators. The approach considers both the collision and frictional stages,
accounting for their intrinsic nonsmoothness and also exploiting the sparsity
induced by the underlying multibody systems. These derivatives have been
implemented in C++, and the code will be open-sourced in the Simple simulator.
They depict state-of-the-art timings ranging from 5 microseconds for a 7-dof
manipulator up to 95 microseconds for 36-dof humanoid, outperforming
alternative solutions by a factor of at least 100.

[Paper Link](
https://arxiv.org/abs/2409.07107
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-17.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Mamba Policy: Towards Efficient 3D Diffusion Policy with Hybrid Selective State Models

- **Authors**: Jiahang Cao, Qiang Zhang, Jingkai Sun, Jiaxu Wang, Hao Cheng, Yulin Li, Jun Ma, Yecheng Shao, Wen Zhao, Gang Han, Yijie Guo, Renjing Xu

#### Abstract

Diffusion models have been widely employed in the field of 3D manipulation
due to their efficient capability to learn distributions, allowing for precise
prediction of action trajectories. However, diffusion models typically rely on
large parameter UNet backbones as policy networks, which can be challenging to
deploy on resource-constrained devices. Recently, the Mamba model has emerged
as a promising solution for efficient modeling, offering low computational
complexity and strong performance in sequence modeling. In this work, we
propose the Mamba Policy, a lighter but stronger policy that reduces the
parameter count by over 80% compared to the original policy network while
achieving superior performance. Specifically, we introduce the XMamba Block,
which effectively integrates input information with conditional features and
leverages a combination of Mamba and Attention mechanisms for deep feature
extraction. Extensive experiments demonstrate that the Mamba Policy excels on
the Adroit, Dexart, and MetaWorld datasets, requiring significantly fewer
computational resources. Additionally, we highlight the Mamba Policy's enhanced
robustness in long-horizon scenarios compared to baseline methods and explore
the performance of various Mamba variants within the Mamba Policy framework.
Our project page is in https://andycao1125.github.io/mamba_policy/.

[Website Link](https://andycao1125.github.io/mamba_policy/.)

[Paper Link](
https://arxiv.org/abs/2409.07163
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-14_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Robust Robot Walker: Learning Agile Locomotion over Tiny Traps

- **Authors**: Shaoting Zhu, Runhan Huang, Linzhan Mou, Hang Zhao

#### Abstract

Quadruped robots must exhibit robust walking capabilities in practical
applications. In this work, we propose a novel approach that enables quadruped
robots to pass various small obstacles, or "tiny traps". Existing methods often
rely on exteroceptive sensors, which can be unreliable for detecting such tiny
traps. To overcome this limitation, our approach focuses solely on
proprioceptive inputs. We introduce a two-stage training framework
incorporating a contact encoder and a classification head to learn implicit
representations of different traps. Additionally, we design a set of tailored
reward functions to improve both the stability of training and the ease of
deployment for goal-tracking tasks. To benefit further research, we design a
new benchmark for tiny trap task. Extensive experiments in both simulation and
real-world settings demonstrate the effectiveness and robustness of our method.
Project Page: https://robust-robot-walker.github.io/

[Website Link](https://robust-robot-walker.github.io/)

[Paper Link](
https://arxiv.org/abs/2409.07409
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-14.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-11


### One Policy to Run Them All: an End-to-end Learning Approach to Multi-Embodiment Locomotion

- **Authors**: Nico Bohlinger, Grzegorz Czechmanowski, Maciej Krupka, Piotr Kicki, Krzysztof Walas, Jan Peters, Davide Tateo

#### Abstract

Deep Reinforcement Learning techniques are achieving state-of-the-art results
in robust legged locomotion. While there exists a wide variety of legged
platforms such as quadruped, humanoids, and hexapods, the field is still
missing a single learning framework that can control all these different
embodiments easily and effectively and possibly transfer, zero or few-shot, to
unseen robot embodiments. We introduce URMA, the Unified Robot Morphology
Architecture, to close this gap. Our framework brings the end-to-end Multi-Task
Reinforcement Learning approach to the realm of legged robots, enabling the
learned policy to control any type of robot morphology. The key idea of our
method is to allow the network to learn an abstract locomotion controller that
can be seamlessly shared between embodiments thanks to our morphology-agnostic
encoders and decoders. This flexible architecture can be seen as a potential
first step in building a foundation model for legged robot locomotion. Our
experiments show that URMA can learn a locomotion policy on multiple
embodiments that can be easily transferred to unseen robot platforms in
simulation and the real world.

[Paper Link](
https://arxiv.org/abs/2409.06366
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-11.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### DemoStart: Demonstration-led auto-curriculum applied to sim-to-real with multi-fingered robots

- **Authors**: Maria Bauza, Jose Enrique Chen, Valentin Dalibard, Nimrod Gileadi, Roland Hafner, Murilo F. Martins, Joss Moore, Rugile Pevceviciute, Antoine Laurens, Dushyant Rao, Martina Zambelli, Martin Riedmiller, Jon Scholz, Konstantinos Bousmalis, Francesco Nori, Nicolas Heess

#### Abstract

We present DemoStart, a novel auto-curriculum reinforcement learning method
capable of learning complex manipulation behaviors on an arm equipped with a
three-fingered robotic hand, from only a sparse reward and a handful of
demonstrations in simulation. Learning from simulation drastically reduces the
development cycle of behavior generation, and domain randomization techniques
are leveraged to achieve successful zero-shot sim-to-real transfer. Transferred
policies are learned directly from raw pixels from multiple cameras and robot
proprioception. Our approach outperforms policies learned from demonstrations
on the real robot and requires 100 times fewer demonstrations, collected in
simulation. More details and videos in https://sites.google.com/view/demostart.

[Website Link](https://sites.google.com/view/demostart.)

[Paper Link](
https://arxiv.org/abs/2409.06613
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-09.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-10


### Promptable Closed-loop Traffic Simulation

- **Authors**: Shuhan Tan, Boris Ivanovic, Yuxiao Chen, Boyi Li, Xinshuo Weng, Yulong Cao, Philipp Krähenbühl, Marco Pavone

#### Abstract

Simulation stands as a cornerstone for safe and efficient autonomous driving
development. At its core a simulation system ought to produce realistic,
reactive, and controllable traffic patterns. In this paper, we propose ProSim,
a multimodal promptable closed-loop traffic simulation framework. ProSim allows
the user to give a complex set of numerical, categorical or textual prompts to
instruct each agent's behavior and intention. ProSim then rolls out a traffic
scenario in a closed-loop manner, modeling each agent's interaction with other
traffic participants. Our experiments show that ProSim achieves high prompt
controllability given different user prompts, while reaching competitive
performance on the Waymo Sim Agents Challenge when no prompt is given. To
support research on promptable traffic simulation, we create
ProSim-Instruct-520k, a multimodal prompt-scenario paired driving dataset with
over 10M text prompts for over 520k real-world driving scenarios. We will
release code of ProSim as well as data and labeling tools of
ProSim-Instruct-520k at https://ariostgx.github.io/ProSim.

[Website Link](https://ariostgx.github.io/ProSim.)

[Paper Link](
https://arxiv.org/abs/2409.05863
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-07.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Learning to Open and Traverse Doors with a Legged Manipulator

- **Authors**: Mike Zhang, Yuntao Ma, Takahiro Miki, Marco Hutter

#### Abstract

Using doors is a longstanding challenge in robotics and is of significant
practical interest in giving robots greater access to human-centric spaces. The
task is challenging due to the need for online adaptation to varying door
properties and precise control in manipulating the door panel and navigating
through the confined doorway. To address this, we propose a learning-based
controller for a legged manipulator to open and traverse through doors. The
controller is trained using a teacher-student approach in simulation to learn
robust task behaviors as well as estimate crucial door properties during the
interaction. Unlike previous works, our approach is a single control policy
that can handle both push and pull doors through learned behaviour which infers
the opening direction during deployment without prior knowledge. The policy was
deployed on the ANYmal legged robot with an arm and achieved a success rate of
95.0% in repeated trials conducted in an experimental setting. Additional
experiments validate the policy's effectiveness and robustness to various doors
and disturbances. A video overview of the method and experiments can be found
at youtu.be/tQDZXN_k5NU.

[Paper Link](
https://arxiv.org/abs/2409.04882
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-05.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Neural MP: A Generalist Neural Motion Planner

- **Authors**: Murtaza Dalal, Jiahui Yang, Russell Mendonca, Youssef Khaky, Ruslan Salakhutdinov, Deepak Pathak

#### Abstract

The current paradigm for motion planning generates solutions from scratch for
every new problem, which consumes significant amounts of time and computational
resources. For complex, cluttered scenes, motion planning approaches can often
take minutes to produce a solution, while humans are able to accurately and
safely reach any goal in seconds by leveraging their prior experience. We seek
to do the same by applying data-driven learning at scale to the problem of
motion planning. Our approach builds a large number of complex scenes in
simulation, collects expert data from a motion planner, then distills it into a
reactive generalist policy. We then combine this with lightweight optimization
to obtain a safe path for real world deployment. We perform a thorough
evaluation of our method on 64 motion planning tasks across four diverse
environments with randomized poses, scenes and obstacles, in the real world,
demonstrating an improvement of 23%, 17% and 79% motion planning success rate
over state of the art sampling, optimization and learning based planning
methods. Video results available at mihdalal.github.io/neuralmotionplanner

[Paper Link](
https://arxiv.org/abs/2409.05864
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_23-00.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Robot Utility Models: General Policies for Zero-Shot Deployment in New Environments

- **Authors**: Haritheja Etukuru, Norihito Naka, Zijin Hu, Seungjae Lee, Julian Mehu, Aaron Edsinger, Chris Paxton, Soumith Chintala, Lerrel Pinto, Nur Muhammad Mahi Shafiullah

#### Abstract

Robot models, particularly those trained with large amounts of data, have
recently shown a plethora of real-world manipulation and navigation
capabilities. Several independent efforts have shown that given sufficient
training data in an environment, robot policies can generalize to demonstrated
variations in that environment. However, needing to finetune robot models to
every new environment stands in stark contrast to models in language or vision
that can be deployed zero-shot for open-world problems. In this work, we
present Robot Utility Models (RUMs), a framework for training and deploying
zero-shot robot policies that can directly generalize to new environments
without any finetuning. To create RUMs efficiently, we develop new tools to
quickly collect data for mobile manipulation tasks, integrate such data into a
policy with multi-modal imitation learning, and deploy policies on-device on
Hello Robot Stretch, a cheap commodity robot, with an external mLLM verifier
for retrying. We train five such utility models for opening cabinet doors,
opening drawers, picking up napkins, picking up paper bags, and reorienting
fallen objects. Our system, on average, achieves 90% success rate in unseen,
novel environments interacting with unseen objects. Moreover, the utility
models can also succeed in different robot and camera set-ups with no further
data, training, or fine-tuning. Primary among our lessons are the importance of
training data over training algorithm and policy class, guidance about data
scaling, necessity for diverse yet high-quality demonstrations, and a recipe
for robot introspection and retrying to improve performance on individual
environments. Our code, data, models, hardware designs, as well as our
experiment and deployment videos are open sourced and can be found on our
project website: https://robotutilitymodels.com

[Website Link](https://robotutilitymodels.com)

[Paper Link](
https://arxiv.org/abs/2409.05865
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-59.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-06


### Incorporating dense metric depth into neural 3D representations for view synthesis and relighting

- **Authors**: Arkadeep Narayan Chaudhury, Igor Vasiljevic, Sergey Zakharov, Vitor Guizilini, Rares Ambrus, Srinivasa Narasimhan, Christopher G. Atkeson

#### Abstract

Synthesizing accurate geometry and photo-realistic appearance of small scenes
is an active area of research with compelling use cases in gaming, virtual
reality, robotic-manipulation, autonomous driving, convenient product capture,
and consumer-level photography. When applying scene geometry and appearance
estimation techniques to robotics, we found that the narrow cone of possible
viewpoints due to the limited range of robot motion and scene clutter caused
current estimation techniques to produce poor quality estimates or even fail.
On the other hand, in robotic applications, dense metric depth can often be
measured directly using stereo and illumination can be controlled. Depth can
provide a good initial estimate of the object geometry to improve
reconstruction, while multi-illumination images can facilitate relighting. In
this work we demonstrate a method to incorporate dense metric depth into the
training of neural 3D representations and address an artifact observed while
jointly refining geometry and appearance by disambiguating between texture and
geometry edges. We also discuss a multi-flash stereo camera system developed to
capture the necessary data for our pipeline and show results on relighting and
view synthesis with a few training views.

[Paper Link](
https://arxiv.org/abs/2409.03061
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-52_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### OccLLaMA: An Occupancy-Language-Action Generative World Model for Autonomous Driving

- **Authors**: Julong Wei, Shanshuai Yuan, Pengfei Li, Qingda Hu, Zhongxue Gan, Wenchao Ding

#### Abstract

The rise of multi-modal large language models(MLLMs) has spurred their
applications in autonomous driving. Recent MLLM-based methods perform action by
learning a direct mapping from perception to action, neglecting the dynamics of
the world and the relations between action and world dynamics. In contrast,
human beings possess world model that enables them to simulate the future
states based on 3D internal visual representation and plan actions accordingly.
To this end, we propose OccLLaMA, an occupancy-language-action generative world
model, which uses semantic occupancy as a general visual representation and
unifies vision-language-action(VLA) modalities through an autoregressive model.
Specifically, we introduce a novel VQVAE-like scene tokenizer to efficiently
discretize and reconstruct semantic occupancy scenes, considering its sparsity
and classes imbalance. Then, we build a unified multi-modal vocabulary for
vision, language and action. Furthermore, we enhance LLM, specifically LLaMA,
to perform the next token/scene prediction on the unified vocabulary to
complete multiple tasks in autonomous driving. Extensive experiments
demonstrate that OccLLaMA achieves competitive performance across multiple
tasks, including 4D occupancy forecasting, motion planning, and visual question
answering, showcasing its potential as a foundation model in autonomous
driving.

[Paper Link](
https://arxiv.org/abs/2409.03272
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-52.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Game On: Towards Language Models as RL Experimenters

- **Authors**: Jingwei Zhang, Thomas Lampe, Abbas Abdolmaleki, Jost Tobias Springenberg, Martin Riedmiller

#### Abstract

We propose an agent architecture that automates parts of the common
reinforcement learning experiment workflow, to enable automated mastery of
control domains for embodied agents. To do so, it leverages a VLM to perform
some of the capabilities normally required of a human experimenter, including
the monitoring and analysis of experiment progress, the proposition of new
tasks based on past successes and failures of the agent, decomposing tasks into
a sequence of subtasks (skills), and retrieval of the skill to execute -
enabling our system to build automated curricula for learning. We believe this
is one of the first proposals for a system that leverages a VLM throughout the
full experiment cycle of reinforcement learning. We provide a first prototype
of this system, and examine the feasibility of current models and techniques
for the desired level of automation. For this, we use a standard Gemini model,
without additional fine-tuning, to provide a curriculum of skills to a
language-conditioned Actor-Critic algorithm, in order to steer data collection
so as to aid learning new skills. Data collected in this way is shown to be
useful for learning and iteratively improving control policies in a robotics
domain. Additional examination of the ability of the system to build a growing
library of skills, and to judge the progress of the training of those skills,
also shows promising results, suggesting that the proposed architecture
provides a potential recipe for fully automated mastery of tasks and domains
for embodied agents.

[Paper Link](
https://arxiv.org/abs/2409.03402
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-51.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Lexicon3D: Probing Visual Foundation Models for Complex 3D Scene Understanding

- **Authors**: Yunze Man, Shuhong Zheng, Zhipeng Bao, Martial Hebert, Liang-Yan Gui, Yu-Xiong Wang

#### Abstract

Complex 3D scene understanding has gained increasing attention, with scene
encoding strategies playing a crucial role in this success. However, the
optimal scene encoding strategies for various scenarios remain unclear,
particularly compared to their image-based counterparts. To address this issue,
we present a comprehensive study that probes various visual encoding models for
3D scene understanding, identifying the strengths and limitations of each model
across different scenarios. Our evaluation spans seven vision foundation
encoders, including image-based, video-based, and 3D foundation models. We
evaluate these models in four tasks: Vision-Language Scene Reasoning, Visual
Grounding, Segmentation, and Registration, each focusing on different aspects
of scene understanding. Our evaluations yield key findings: DINOv2 demonstrates
superior performance, video models excel in object-level tasks, diffusion
models benefit geometric tasks, and language-pretrained models show unexpected
limitations in language-related tasks. These insights challenge some
conventional understandings, provide novel perspectives on leveraging visual
foundation models, and highlight the need for more flexible encoder selection
in future vision-language and scene-understanding tasks.

[Paper Link](
https://arxiv.org/abs/2409.03757
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-50.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RoboKoop: Efficient Control Conditioned Representations from Visual Input in Robotics using Koopman Operator

- **Authors**: Hemant Kumawat, Biswadeep Chakraborty, Saibal Mukhopadhyay

#### Abstract

Developing agents that can perform complex control tasks from
high-dimensional observations is a core ability of autonomous agents that
requires underlying robust task control policies and adapting the underlying
visual representations to the task. Most existing policies need a lot of
training samples and treat this problem from the lens of two-stage learning
with a controller learned on top of pre-trained vision models. We approach this
problem from the lens of Koopman theory and learn visual representations from
robotic agents conditioned on specific downstream tasks in the context of
learning stabilizing control for the agent. We introduce a Contrastive Spectral
Koopman Embedding network that allows us to learn efficient linearized visual
representations from the agent's visual data in a high dimensional latent space
and utilizes reinforcement learning to perform off-policy control on top of the
extracted representations with a linear controller. Our method enhances
stability and control in gradient dynamics over time, significantly
outperforming existing approaches by improving efficiency and accuracy in
learning task policies over extended horizons.

[Paper Link](
https://arxiv.org/abs/2409.03107
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-49.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-05


### Multi-modal Situated Reasoning in 3D Scenes

- **Authors**: Xiongkun Linghu, Jiangyong Huang, Xuesong Niu, Xiaojian Ma, Baoxiong Jia, Siyuan Huang

#### Abstract

Situation awareness is essential for understanding and reasoning about 3D
scenes in embodied AI agents. However, existing datasets and benchmarks for
situated understanding are limited in data modality, diversity, scale, and task
scope. To address these limitations, we propose Multi-modal Situated Question
Answering (MSQA), a large-scale multi-modal situated reasoning dataset,
scalably collected leveraging 3D scene graphs and vision-language models (VLMs)
across a diverse range of real-world 3D scenes. MSQA includes 251K situated
question-answering pairs across 9 distinct question categories, covering
complex scenarios within 3D scenes. We introduce a novel interleaved
multi-modal input setting in our benchmark to provide text, image, and point
cloud for situation and question description, resolving ambiguity in previous
single-modality convention (e.g., text). Additionally, we devise the
Multi-modal Situated Next-step Navigation (MSNN) benchmark to evaluate models'
situated reasoning for navigation. Comprehensive evaluations on MSQA and MSNN
highlight the limitations of existing vision-language models and underscore the
importance of handling multi-modal interleaved inputs and situation modeling.
Experiments on data scaling and cross-domain transfer further demonstrate the
efficacy of leveraging MSQA as a pre-training dataset for developing more
powerful situated reasoning models.

[Paper Link](
https://arxiv.org/abs/2409.02389
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-45.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Reinforcement Learning for Wheeled Mobility on Vertically Challenging Terrain

- **Authors**: Tong Xu, Chenhui Pan, Xuesu Xiao

#### Abstract

Off-road navigation on vertically challenging terrain, involving steep slopes
and rugged boulders, presents significant challenges for wheeled robots both at
the planning level to achieve smooth collision-free trajectories and at the
control level to avoid rolling over or getting stuck. Considering the complex
model of wheel-terrain interactions, we develop an end-to-end Reinforcement
Learning (RL) system for an autonomous vehicle to learn wheeled mobility
through simulated trial-and-error experiences. Using a custom-designed
simulator built on the Chrono multi-physics engine, our approach leverages
Proximal Policy Optimization (PPO) and a terrain difficulty curriculum to
refine a policy based on a reward function to encourage progress towards the
goal and penalize excessive roll and pitch angles, which circumvents the need
of complex and expensive kinodynamic modeling, planning, and control.
Additionally, we present experimental results in the simulator and deploy our
approach on a physical Verti-4-Wheeler (V4W) platform, demonstrating that RL
can equip conventional wheeled robots with previously unrealized potential of
navigating vertically challenging terrain.

[Paper Link](
https://arxiv.org/abs/2409.02383
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-42.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RoboTwin: Dual-Arm Robot Benchmark with Generative Digital Twins (early version)

- **Authors**: Yao Mu, Tianxing Chen, Shijia Peng, Zanxin Chen, Zeyu Gao, Yude Zou, Lunkai Lin, Zhiqiang Xie, Ping Luo

#### Abstract

Effective collaboration of dual-arm robots and their tool use capabilities
are increasingly important areas in the advancement of robotics. These skills
play a significant role in expanding robots' ability to operate in diverse
real-world environments. However, progress is impeded by the scarcity of
specialized training data. This paper introduces RoboTwin, a novel benchmark
dataset combining real-world teleoperated data with synthetic data from digital
twins, designed for dual-arm robotic scenarios. Using the COBOT Magic platform,
we have collected diverse data on tool usage and human-robot interaction. We
present a innovative approach to creating digital twins using AI-generated
content, transforming 2D images into detailed 3D models. Furthermore, we
utilize large language models to generate expert-level training data and
task-specific pose sequences oriented toward functionality. Our key
contributions are: 1) the RoboTwin benchmark dataset, 2) an efficient
real-to-simulation pipeline, and 3) the use of language models for automatic
expert-level data generation. These advancements are designed to address the
shortage of robotic training data, potentially accelerating the development of
more capable and versatile robotic systems for a wide range of real-world
applications. The project page is available at
https://robotwin-benchmark.github.io/early-version/

[Website Link](https://robotwin-benchmark.github.io/early-version/)

[Paper Link](
https://arxiv.org/abs/2409.02920
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-39.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-04


### Constraint-Aware Intent Estimation for Dynamic Human-Robot Object Co-Manipulation

- **Authors**: Yifei Simon Shao, Tianyu Li, Shafagh Keyvanian, Pratik Chaudhari, Vijay Kumar, Nadia Figueroa

#### Abstract

Constraint-aware estimation of human intent is essential for robots to
physically collaborate and interact with humans. Further, to achieve fluid
collaboration in dynamic tasks intent estimation should be achieved in
real-time. In this paper, we present a framework that combines online
estimation and control to facilitate robots in interpreting human intentions,
and dynamically adjust their actions to assist in dynamic object
co-manipulation tasks while considering both robot and human constraints.
Central to our approach is the adoption of a Dynamic Systems (DS) model to
represent human intent. Such a low-dimensional parameterized model, along with
human manipulability and robot kinematic constraints, enables us to predict
intent using a particle filter solely based on past motion data and tracking
errors. For safe assistive control, we propose a variable impedance controller
that adapts the robot's impedance to offer assistance based on the intent
estimation confidence from the DS particle filter. We validate our framework on
a challenging real-world human-robot co-manipulation task and present promising
results over baselines. Our framework represents a significant step forward in
physical human-robot collaboration (pHRC), ensuring that robot cooperative
interactions with humans are both feasible and effective.

[Paper Link](
https://arxiv.org/abs/2409.00215
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-37.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Rapid and Robust Trajectory Optimization for Humanoids

- **Authors**: Bohao Zhang, Ram Vasudevan

#### Abstract

Performing trajectory design for humanoid robots with high degrees of freedom
is computationally challenging. The trajectory design process also often
involves carefully selecting various hyperparameters and requires a good
initial guess which can further complicate the development process. This work
introduces a generalized gait optimization framework that directly generates
smooth and physically feasible trajectories. The proposed method demonstrates
faster and more robust convergence than existing techniques and explicitly
incorporates closed-loop kinematic constraints that appear in many modern
humanoids. The method is implemented as an open-source C++ codebase which can
be found at https://roahmlab.github.io/RAPTOR/.

[Website Link](https://roahmlab.github.io/RAPTOR/.)

[Paper Link](
https://arxiv.org/abs/2409.00303
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-36.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Diffusion Policy Policy Optimization

- **Authors**: Allen Z. Ren, Justin Lidard, Lars L. Ankile, Anthony Simeonov, Pulkit Agrawal, Anirudha Majumdar, Benjamin Burchfiel, Hongkai Dai, Max Simchowitz

#### Abstract

We introduce Diffusion Policy Policy Optimization, DPPO, an algorithmic
framework including best practices for fine-tuning diffusion-based policies
(e.g. Diffusion Policy) in continuous control and robot learning tasks using
the policy gradient (PG) method from reinforcement learning (RL). PG methods
are ubiquitous in training RL policies with other policy parameterizations;
nevertheless, they had been conjectured to be less efficient for
diffusion-based policies. Surprisingly, we show that DPPO achieves the
strongest overall performance and efficiency for fine-tuning in common
benchmarks compared to other RL methods for diffusion-based policies and also
compared to PG fine-tuning of other policy parameterizations. Through
experimental investigation, we find that DPPO takes advantage of unique
synergies between RL fine-tuning and the diffusion parameterization, leading to
structured and on-manifold exploration, stable training, and strong policy
robustness. We further demonstrate the strengths of DPPO in a range of
realistic settings, including simulated robotic tasks with pixel observations,
and via zero-shot deployment of simulation-trained policies on robot hardware
in a long-horizon, multi-stage manipulation task. Website with code:
diffusion-ppo.github.io

[Paper Link](
https://arxiv.org/abs/2409.00588
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-35.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### ReKep: Spatio-Temporal Reasoning of Relational Keypoint Constraints for Robotic Manipulation

- **Authors**: Wenlong Huang, Chen Wang, Yunzhu Li, Ruohan Zhang, Li Fei-Fei

#### Abstract

Representing robotic manipulation tasks as constraints that associate the
robot and the environment is a promising way to encode desired robot behaviors.
However, it remains unclear how to formulate the constraints such that they are
1) versatile to diverse tasks, 2) free of manual labeling, and 3) optimizable
by off-the-shelf solvers to produce robot actions in real-time. In this work,
we introduce Relational Keypoint Constraints (ReKep), a visually-grounded
representation for constraints in robotic manipulation. Specifically, ReKep is
expressed as Python functions mapping a set of 3D keypoints in the environment
to a numerical cost. We demonstrate that by representing a manipulation task as
a sequence of Relational Keypoint Constraints, we can employ a hierarchical
optimization procedure to solve for robot actions (represented by a sequence of
end-effector poses in SE(3)) with a perception-action loop at a real-time
frequency. Furthermore, in order to circumvent the need for manual
specification of ReKep for each new task, we devise an automated procedure that
leverages large vision models and vision-language models to produce ReKep from
free-form language instructions and RGB-D observations. We present system
implementations on a wheeled single-arm platform and a stationary dual-arm
platform that can perform a large variety of manipulation tasks, featuring
multi-stage, in-the-wild, bimanual, and reactive behaviors, all without
task-specific data or environment models. Website at
https://rekep-robot.github.io.

[Website Link](https://rekep-robot.github.io.)

[Paper Link](
https://arxiv.org/abs/2409.01652
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-31.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### GraspSplats: Efficient Manipulation with 3D Feature Splatting

- **Authors**: Mazeyu Ji, Ri-Zhao Qiu, Xueyan Zou, Xiaolong Wang

#### Abstract

The ability for robots to perform efficient and zero-shot grasping of object
parts is crucial for practical applications and is becoming prevalent with
recent advances in Vision-Language Models (VLMs). To bridge the 2D-to-3D gap
for representations to support such a capability, existing methods rely on
neural fields (NeRFs) via differentiable rendering or point-based projection
methods. However, we demonstrate that NeRFs are inappropriate for scene changes
due to their implicitness and point-based methods are inaccurate for part
localization without rendering-based optimization. To amend these issues, we
propose GraspSplats. Using depth supervision and a novel reference feature
computation method, GraspSplats generates high-quality scene representations in
under 60 seconds. We further validate the advantages of Gaussian-based
representation by showing that the explicit and optimized geometry in
GraspSplats is sufficient to natively support (1) real-time grasp sampling and
(2) dynamic and articulated object manipulation with point trackers. With
extensive experiments on a Franka robot, we demonstrate that GraspSplats
significantly outperforms existing methods under diverse task settings. In
particular, GraspSplats outperforms NeRF-based methods like F3RM and LERF-TOGO,
and 2D detection methods.

[Paper Link](
https://arxiv.org/abs/2409.02084
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-30.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-09-02


### Robotic Object Insertion with a Soft Wrist through Sim-to-Real Privileged Training

- **Authors**: Yuni Fuchioka, Cristian C. Beltran-Hernandez, Hai Nguyen, Masashi Hamaya

#### Abstract

This study addresses contact-rich object insertion tasks under unstructured
environments using a robot with a soft wrist, enabling safe contact
interactions. For the unstructured environments, we assume that there are
uncertainties in object grasp and hole pose and that the soft wrist pose cannot
be directly measured. Recent methods employ learning approaches and
force/torque sensors for contact localization; however, they require data
collection in the real world. This study proposes a sim-to-real approach using
a privileged training strategy. This method has two steps. 1) The teacher
policy is trained to complete the task with sensor inputs and ground truth
privileged information such as the peg pose, and then 2) the student encoder is
trained with data produced from teacher policy rollouts to estimate the
privileged information from sensor history. We performed sim-to-real
experiments under grasp and hole pose uncertainties. This resulted in 100\%,
95\%, and 80\% success rates for circular peg insertion with 0, +5, and -5
degree peg misalignments, respectively, and start positions randomly shifted
$\pm$ 10 mm from a default position. Also, we tested the proposed method with a
square peg that was never seen during training. Additional simulation
evaluations revealed that using the privileged strategy improved success rates
compared to training with only simulated sensor data. Our results demonstrate
the advantage of using sim-to-real privileged training for soft robots, which
has the potential to alleviate human engineering efforts for robotic assembly.

[Paper Link](
https://arxiv.org/abs/2408.17061
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-24.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-30


### 3D Whole-body Grasp Synthesis with Directional Controllability

- **Authors**: Georgios Paschalidis, Romana Wilschut, Dimitrije Antić, Omid Taheri, Dimitrios Tzionas

#### Abstract

Synthesizing 3D whole-bodies that realistically grasp objects is useful for
animation, mixed reality, and robotics. This is challenging, because the hands
and body need to look natural w.r.t. each other, the grasped object, as well as
the local scene (i.e., a receptacle supporting the object). Only recent work
tackles this, with a divide-and-conquer approach; it first generates a
"guiding" right-hand grasp, and then searches for bodies that match this.
However, the guiding-hand synthesis lacks controllability and receptacle
awareness, so it likely has an implausible direction (i.e., a body can't match
this without penetrating the receptacle) and needs corrections through major
post-processing. Moreover, the body search needs exhaustive sampling and is
expensive. These are strong limitations. We tackle these with a novel method
called CWGrasp. Our key idea is that performing geometry-based reasoning "early
on," instead of "too late," provides rich "control" signals for inference. To
this end, CWGrasp first samples a plausible reaching-direction vector (used
later for both the arm and hand) from a probabilistic model built via
raycasting from the object and collision checking. Then, it generates a
reaching body with a desired arm direction, as well as a "guiding" grasping
hand with a desired palm direction that complies with the arm's one.
Eventually, CWGrasp refines the body to match the "guiding" hand, while
plausibly contacting the scene. Notably, generating already-compatible "parts"
greatly simplifies the "whole." Moreover, CWGrasp uniquely tackles both right-
and left-hand grasps. We evaluate on the GRAB and ReplicaGrasp datasets.
CWGrasp outperforms baselines, at lower runtime and budget, while all
components help performance. Code and models will be released.

[Paper Link](
https://arxiv.org/abs/2408.16770
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-19.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Hitting the Gym: Reinforcement Learning Control of Exercise-Strengthened Biohybrid Robots in Simulation

- **Authors**: Saul Schaffer, Hima Hrithik Pamu, Victoria A. Webster-Wood

#### Abstract

Animals can accomplish many incredible behavioral feats across a wide range
of operational environments and scales that current robots struggle to match.
One explanation for this performance gap is the extraordinary properties of the
biological materials that comprise animals, such as muscle tissue. Using living
muscle tissue as an actuator can endow robotic systems with highly desirable
properties such as self-healing, compliance, and biocompatibility. Unlike
traditional soft robotic actuators, living muscle biohybrid actuators exhibit
unique adaptability, growing stronger with use. The dependency of a muscle's
force output on its use history endows muscular organisms the ability to
dynamically adapt to their environment, getting better at tasks over time.
While muscle adaptability is a benefit to muscular organisms, it currently
presents a challenge for biohybrid researchers: how does one design and control
a robot whose actuators' force output changes over time? Here, we incorporate
muscle adaptability into a many-muscle biohybrid robot design and modeling
tool, leveraging reinforcement learning as both a co-design partner and system
controller. As a controller, our learning agents coordinated the independent
contraction of 42 muscles distributed on a lattice worm structure to
successfully steer it towards eight distinct targets while incorporating muscle
adaptability. As a co-design tool, our agents enable users to identify which
muscles are important to accomplishing a given task. Our results show that
adaptive agents outperform non-adaptive agents in terms of maximum rewards and
training time. Together, these contributions can both enable the elucidation of
muscle actuator adaptation and inform the design and modeling of adaptive,
performant, many-muscle robots.

[Paper Link](
https://arxiv.org/abs/2408.16069
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-18.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Identifying Terrain Physical Parameters from Vision -- Towards Physical-Parameter-Aware Locomotion and Navigation

- **Authors**: Jiaqi Chen, Jonas Frey, Ruyi Zhou, Takahiro Miki, Georg Martius, Marco Hutter

#### Abstract

Identifying the physical properties of the surrounding environment is
essential for robotic locomotion and navigation to deal with non-geometric
hazards, such as slippery and deformable terrains. It would be of great benefit
for robots to anticipate these extreme physical properties before contact;
however, estimating environmental physical parameters from vision is still an
open challenge. Animals can achieve this by using their prior experience and
knowledge of what they have seen and how it felt. In this work, we propose a
cross-modal self-supervised learning framework for vision-based environmental
physical parameter estimation, which paves the way for future
physical-property-aware locomotion and navigation. We bridge the gap between
existing policies trained in simulation and identification of physical terrain
parameters from vision. We propose to train a physical decoder in simulation to
predict friction and stiffness from multi-modal input. The trained network
allows the labeling of real-world images with physical parameters in a
self-supervised manner to further train a visual network during deployment,
which can densely predict the friction and stiffness from image data. We
validate our physical decoder in simulation and the real world using a
quadruped ANYmal robot, outperforming an existing baseline method. We show that
our visual network can predict the physical properties in indoor and outdoor
experiments while allowing fast adaptation to new environments.

[Paper Link](
https://arxiv.org/abs/2408.16567
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-15.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-29


### SkillMimic: Learning Reusable Basketball Skills from Demonstrations

- **Authors**: Yinhuai Wang, Qihan Zhao, Runyi Yu, Ailing Zeng, Jing Lin, Zhengyi Luo, Hok Wai Tsui, Jiwen Yu, Xiu Li, Qifeng Chen, Jian Zhang, Lei Zhang, Ping Tan

#### Abstract

Mastering basketball skills such as diverse layups and dribbling involves
complex interactions with the ball and requires real-time adjustments.
Traditional reinforcement learning methods for interaction skills rely on
labor-intensive, manually designed rewards that do not generalize well across
different skills. Inspired by how humans learn from demonstrations, we propose
SkillMimic, a data-driven approach that mimics both human and ball motions to
learn a wide variety of basketball skills. SkillMimic employs a unified
configuration to learn diverse skills from human-ball motion datasets, with
skill diversity and generalization improving as the dataset grows. This
approach allows training a single policy to learn multiple skills, enabling
smooth skill switching even if these switches are not present in the reference
dataset. The skills acquired by SkillMimic can be easily reused by a high-level
controller to accomplish complex basketball tasks. To evaluate our approach, we
introduce two basketball datasets: one estimated through monocular RGB videos
and the other using advanced motion capture equipment, collectively containing
about 35 minutes of diverse basketball skills. Experiments show that our method
can effectively learn various basketball skills included in the dataset with a
unified configuration, including various styles of dribbling, layups, and
shooting. Furthermore, by training a high-level controller to reuse the
acquired skills, we can achieve complex basketball tasks such as layup scoring,
which involves dribbling toward the basket, timing the dribble and layup to
score, retrieving the rebound, and repeating the process. The project page and
video demonstrations are available at https://ingrid789.github.io/SkillMimic/

[Website Link](https://ingrid789.github.io/SkillMimic/)

[Paper Link](
https://arxiv.org/abs/2408.15270
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_22-10.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### DeMoBot: Deformable Mobile Manipulation with Vision-based Sub-goal Retrieval

- **Authors**: Yuying Zhang, Wenyan Yang, Joni Pajarinen

#### Abstract

Imitation learning (IL) algorithms typically distill experience into
parametric behavior policies to mimic expert demonstrations. Despite their
effectiveness, previous methods often struggle with data efficiency and
accurately aligning the current state with expert demonstrations, especially in
deformable mobile manipulation tasks characterized by partial observations and
dynamic object deformations. In this paper, we introduce \textbf{DeMoBot}, a
novel IL approach that directly retrieves observations from demonstrations to
guide robots in \textbf{De}formable \textbf{Mo}bile manipulation tasks. DeMoBot
utilizes vision foundation models to identify relevant expert data based on
visual similarity and matches the current trajectory with demonstrated
trajectories using trajectory similarity and forward reachability constraints
to select suitable sub-goals. Once a goal is determined, a motion generation
policy will guide the robot to the next state until the task is completed. We
evaluated DeMoBot using a Spot robot in several simulated and real-world
settings, demonstrating its effectiveness and generalizability. With only 20
demonstrations, DeMoBot significantly outperforms the baselines, reaching a
50\% success rate in curtain opening and 85\% in gap covering in simulation.

[Paper Link](
https://arxiv.org/abs/2408.15919
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-55.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-28


### Benchmarking Reinforcement Learning Methods for Dexterous Robotic Manipulation with a Three-Fingered Gripper

- **Authors**: Elizabeth Cutler, Yuning Xing, Tony Cui, Brendan Zhou, Koen van Rijnsoever, Ben Hart, David Valencia, Lee Violet C. Ong, Trevor Gee, Minas Liarokapis, Henry Williams

#### Abstract

Reinforcement Learning (RL) training is predominantly conducted in
cost-effective and controlled simulation environments. However, the transfer of
these trained models to real-world tasks often presents unavoidable challenges.
This research explores the direct training of RL algorithms in controlled yet
realistic real-world settings for the execution of dexterous manipulation. The
benchmarking results of three RL algorithms trained on intricate in-hand
manipulation tasks within practical real-world contexts are presented. Our
study not only demonstrates the practicality of RL training in authentic
real-world scenarios, facilitating direct real-world applications, but also
provides insights into the associated challenges and considerations.
Additionally, our experiences with the employed experimental methods are
shared, with the aim of empowering and engaging fellow researchers and
practitioners in this dynamic field of robotics.

[Paper Link](
https://arxiv.org/abs/2408.14747
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-49.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Points2Plans: From Point Clouds to Long-Horizon Plans with Composable Relational Dynamics

- **Authors**: Yixuan Huang, Christopher Agia, Jimmy Wu, Tucker Hermans, Jeannette Bohg

#### Abstract

We present Points2Plans, a framework for composable planning with a
relational dynamics model that enables robots to solve long-horizon
manipulation tasks from partial-view point clouds. Given a language instruction
and a point cloud of the scene, our framework initiates a hierarchical planning
procedure, whereby a language model generates a high-level plan and a
sampling-based planner produces constraint-satisfying continuous parameters for
manipulation primitives sequenced according to the high-level plan. Key to our
approach is the use of a relational dynamics model as a unifying interface
between the continuous and symbolic representations of states and actions, thus
facilitating language-driven planning from high-dimensional perceptual input
such as point clouds. Whereas previous relational dynamics models require
training on datasets of multi-step manipulation scenarios that align with the
intended test scenarios, Points2Plans uses only single-step simulated training
data while generalizing zero-shot to a variable number of steps during
real-world evaluations. We evaluate our approach on tasks involving geometric
reasoning, multi-object interactions, and occluded object reasoning in both
simulated and real-world settings. Results demonstrate that Points2Plans offers
strong generalization to unseen long-horizon tasks in the real world, where it
solves over 85% of evaluated tasks while the next best baseline solves only
50%. Qualitative demonstrations of our approach operating on a mobile
manipulator platform are made available at
sites.google.com/stanford.edu/points2plans.

[Paper Link](
https://arxiv.org/abs/2408.14769
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-48.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Depth Restoration of Hand-Held Transparent Objects for Human-to-Robot Handover

- **Authors**: Ran Yu, Haixin Yu, Shoujie Li, Huang Yan, Ziwu Song, Wenbo Ding

#### Abstract

Transparent objects are common in daily life, while their optical properties
pose challenges for RGB-D cameras to capture accurate depth information. This
issue is further amplified when these objects are hand-held, as hand occlusions
further complicate depth estimation. For assistant robots, however, accurately
perceiving hand-held transparent objects is critical to effective human-robot
interaction. This paper presents a Hand-Aware Depth Restoration (HADR) method
based on creating an implicit neural representation function from a single
RGB-D image. The proposed method utilizes hand posture as an important guidance
to leverage semantic and geometric information of hand-object interaction. To
train and evaluate the proposed method, we create a high-fidelity synthetic
dataset named TransHand-14K with a real-to-sim data generation scheme.
Experiments show that our method has better performance and generalization
ability compared with existing methods. We further develop a real-world
human-to-robot handover system based on HADR, demonstrating its potential in
human-robot interaction applications.

[Paper Link](
https://arxiv.org/abs/2408.14997
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-47.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-27


### PIE: Parkour with Implicit-Explicit Learning Framework for Legged Robots

- **Authors**: Shixin Luo, Songbo Li, Ruiqi Yu, Zhicheng Wang, Jun Wu, Qiuguo Zhu

#### Abstract

Parkour presents a highly challenging task for legged robots, requiring them
to traverse various terrains with agile and smooth locomotion. This
necessitates comprehensive understanding of both the robot's own state and the
surrounding terrain, despite the inherent unreliability of robot perception and
actuation. Current state-of-the-art methods either rely on complex pre-trained
high-level terrain reconstruction modules or limit the maximum potential of
robot parkour to avoid failure due to inaccurate perception. In this paper, we
propose a one-stage end-to-end learning-based parkour framework: Parkour with
Implicit-Explicit learning framework for legged robots (PIE) that leverages
dual-level implicit-explicit estimation. With this mechanism, even a low-cost
quadruped robot equipped with an unreliable egocentric depth camera can achieve
exceptional performance on challenging parkour terrains using a relatively
simple training process and reward function. While the training process is
conducted entirely in simulation, our real-world validation demonstrates
successful zero-shot deployment of our framework, showcasing superior parkour
performance on harsh terrains.

[Paper Link](
https://arxiv.org/abs/2408.13740
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-41.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### MASQ: Multi-Agent Reinforcement Learning for Single Quadruped Robot Locomotion

- **Authors**: Qi Liu, Jingxiang Guo, Sixu Lin, Shuaikang Ma, Jinxuan Zhu, Yanjie Li

#### Abstract

This paper proposes a novel method to improve locomotion learning for a
single quadruped robot using multi-agent deep reinforcement learning (MARL).
Many existing methods use single-agent reinforcement learning for an individual
robot or MARL for the cooperative task in multi-robot systems. Unlike existing
methods, this paper proposes using MARL for the locomotion learning of a single
quadruped robot. We develop a learning structure called Multi-Agent
Reinforcement Learning for Single Quadruped Robot Locomotion (MASQ),
considering each leg as an agent to explore the action space of the quadruped
robot, sharing a global critic, and learning collaboratively. Experimental
results indicate that MASQ not only speeds up learning convergence but also
enhances robustness in real-world settings, suggesting that applying MASQ to
single robots such as quadrupeds could surpass traditional single-robot
reinforcement learning approaches. Our study provides insightful guidance on
integrating MARL with single-robot locomotion learning.

[Paper Link](
https://arxiv.org/abs/2408.13759
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-33.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>
<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-33_1.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### FAST-LIVO2: Fast, Direct LiDAR-Inertial-Visual Odometry

- **Authors**: Chunran Zheng, Wei Xu, Zuhao Zou, Tong Hua, Chongjian Yuan, Dongjiao He, Bingyang Zhou, Zheng Liu, Jiarong Lin, Fangcheng Zhu, Yunfan Ren, Rong Wang, Fanle Meng, Fu Zhang

#### Abstract

This paper proposes FAST-LIVO2: a fast, direct LiDAR-inertial-visual odometry
framework to achieve accurate and robust state estimation in SLAM tasks and
provide great potential in real-time, onboard robotic applications. FAST-LIVO2
fuses the IMU, LiDAR and image measurements efficiently through an ESIKF. To
address the dimension mismatch between the heterogeneous LiDAR and image
measurements, we use a sequential update strategy in the Kalman filter. To
enhance the efficiency, we use direct methods for both the visual and LiDAR
fusion, where the LiDAR module registers raw points without extracting edge or
plane features and the visual module minimizes direct photometric errors
without extracting ORB or FAST corner features. The fusion of both visual and
LiDAR measurements is based on a single unified voxel map where the LiDAR
module constructs the geometric structure for registering new LiDAR scans and
the visual module attaches image patches to the LiDAR points. To enhance the
accuracy of image alignment, we use plane priors from the LiDAR points in the
voxel map (and even refine the plane prior) and update the reference patch
dynamically after new images are aligned. Furthermore, to enhance the
robustness of image alignment, FAST-LIVO2 employs an on-demanding raycast
operation and estimates the image exposure time in real time. Lastly, we detail
three applications of FAST-LIVO2: UAV onboard navigation demonstrating the
system's computation efficiency for real-time onboard navigation, airborne
mapping showcasing the system's mapping accuracy, and 3D model rendering
(mesh-based and NeRF-based) underscoring the suitability of our reconstructed
dense map for subsequent rendering tasks. We open source our code, dataset and
application on GitHub to benefit the robotics community.

[Paper Link](
https://arxiv.org/abs/2408.14035
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-16.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Equivariant Reinforcement Learning under Partial Observability

- **Authors**: Hai Nguyen, Andrea Baisero, David Klee, Dian Wang, Robert Platt, Christopher Amato

#### Abstract

Incorporating inductive biases is a promising approach for tackling
challenging robot learning domains with sample-efficient solutions. This paper
identifies partially observable domains where symmetries can be a useful
inductive bias for efficient learning. Specifically, by encoding the
equivariance regarding specific group symmetries into the neural networks, our
actor-critic reinforcement learning agents can reuse solutions in the past for
related scenarios. Consequently, our equivariant agents outperform
non-equivariant approaches significantly in terms of sample efficiency and
final performance, demonstrated through experiments on a range of robotic tasks
in simulation and real hardware.

[Paper Link](
https://arxiv.org/abs/2408.14336
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_21-02.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Advancing Humanoid Locomotion: Mastering Challenging Terrains with Denoising World Model Learning

- **Authors**: Xinyang Gu, Yen-Jen Wang, Xiang Zhu, Chengming Shi, Yanjiang Guo, Yichen Liu, Jianyu Chen

#### Abstract

Humanoid robots, with their human-like skeletal structure, are especially
suited for tasks in human-centric environments. However, this structure is
accompanied by additional challenges in locomotion controller design,
especially in complex real-world environments. As a result, existing humanoid
robots are limited to relatively simple terrains, either with model-based
control or model-free reinforcement learning. In this work, we introduce
Denoising World Model Learning (DWL), an end-to-end reinforcement learning
framework for humanoid locomotion control, which demonstrates the world's first
humanoid robot to master real-world challenging terrains such as snowy and
inclined land in the wild, up and down stairs, and extremely uneven terrains.
All scenarios run the same learned neural network with zero-shot sim-to-real
transfer, indicating the superior robustness and generalization capability of
the proposed method.

[Paper Link](
https://arxiv.org/abs/2408.14472
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_20-58.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-26


### Multi-finger Manipulation via Trajectory Optimization with Differentiable Rolling and Geometric Constraints

- **Authors**: Fan Yang, Thomas Power, Sergio Aguilera Marinovic, Soshi Iba, Rana Soltani Zarrin, Dmitry Berenson

#### Abstract

Parameterizing finger rolling and finger-object contacts in a differentiable
manner is important for formulating dexterous manipulation as a trajectory
optimization problem. In contrast to previous methods which often assume
simplified geometries of the robot and object or do not explicitly model finger
rolling, we propose a method to further extend the capabilities of dexterous
manipulation by accounting for non-trivial geometries of both the robot and the
object. By integrating the object's Signed Distance Field (SDF) with a sampling
method, our method estimates contact and rolling-related variables and includes
those in a trajectory optimization framework. This formulation naturally allows
for the emergence of finger-rolling behaviors, enabling the robot to locally
adjust the contact points. Our method is tested in a peg alignment task and a
screwdriver turning task, where it outperforms the baselines in terms of
achieving desired object configurations and avoiding dropping the object. We
also successfully apply our method to a real-world screwdriver turning task,
demonstrating its robustness to the sim2real gap.

[Paper Link](
https://arxiv.org/abs/2408.13229
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_20-53.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-23


### LLM-enhanced Scene Graph Learning for Household Rearrangement

- **Authors**: Wenhao Li, Zhiyuan Yu, Qijin She, Zhinan Yu, Yuqing Lan, Chenyang Zhu, Ruizhen Hu, Kai Xu

#### Abstract

The household rearrangement task involves spotting misplaced objects in a
scene and accommodate them with proper places. It depends both on common-sense
knowledge on the objective side and human user preference on the subjective
side. In achieving such task, we propose to mine object functionality with user
preference alignment directly from the scene itself, without relying on human
intervention. To do so, we work with scene graph representation and propose
LLM-enhanced scene graph learning which transforms the input scene graph into
an affordance-enhanced graph (AEG) with information-enhanced nodes and newly
discovered edges (relations). In AEG, the nodes corresponding to the receptacle
objects are augmented with context-induced affordance which encodes what kind
of carriable objects can be placed on it. New edges are discovered with newly
discovered non-local relations. With AEG, we perform task planning for scene
rearrangement by detecting misplaced carriables and determining a proper
placement for each of them. We test our method by implementing a tiding robot
in simulator and perform evaluation on a new benchmark we build. Extensive
evaluations demonstrate that our method achieves state-of-the-art performance
on misplacement detection and the following rearrangement planning.

[Paper Link](
https://arxiv.org/abs/2408.12093
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_20-39.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-22


### EmbodiedSAM: Online Segment Any 3D Thing in Real Time

- **Authors**: Xiuwei Xu, Huangxing Chen, Linqing Zhao, Ziwei Wang, Jie Zhou, Jiwen Lu

#### Abstract

Embodied tasks require the agent to fully understand 3D scenes simultaneously
with its exploration, so an online, real-time, fine-grained and
highly-generalized 3D perception model is desperately needed. Since
high-quality 3D data is limited, directly training such a model in 3D is almost
infeasible. Meanwhile, vision foundation models (VFM) has revolutionized the
field of 2D computer vision with superior performance, which makes the use of
VFM to assist embodied 3D perception a promising direction. However, most
existing VFM-assisted 3D perception methods are either offline or too slow that
cannot be applied in practical embodied tasks. In this paper, we aim to
leverage Segment Anything Model (SAM) for real-time 3D instance segmentation in
an online setting. This is a challenging problem since future frames are not
available in the input streaming RGB-D video, and an instance may be observed
in several frames so object matching between frames is required. To address
these challenges, we first propose a geometric-aware query lifting module to
represent the 2D masks generated by SAM by 3D-aware queries, which is then
iteratively refined by a dual-level query decoder. In this way, the 2D masks
are transferred to fine-grained shapes on 3D point clouds. Benefit from the
query representation for 3D masks, we can compute the similarity matrix between
the 3D masks from different views by efficient matrix operation, which enables
real-time inference. Experiments on ScanNet, ScanNet200, SceneNN and 3RScan
show our method achieves leading performance even compared with offline
methods. Our method also demonstrates great generalization ability in several
zero-shot dataset transferring experiments and show great potential in
open-vocabulary and data-efficient setting. Code and demo are available at
https://xuxw98.github.io/ESAM/, with only one RTX 3090 GPU required for
training and evaluation.

[Website Link](https://xuxw98.github.io/ESAM/,)

[Paper Link](
https://arxiv.org/abs/2408.11811
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_20-32.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Scaling Cross-Embodied Learning: One Policy for Manipulation, Navigation, Locomotion and Aviation

- **Authors**: Ria Doshi, Homer Walke, Oier Mees, Sudeep Dasari, Sergey Levine

#### Abstract

Modern machine learning systems rely on large datasets to attain broad
generalization, and this often poses a challenge in robot learning, where each
robotic platform and task might have only a small dataset. By training a single
policy across many different kinds of robots, a robot learning method can
leverage much broader and more diverse datasets, which in turn can lead to
better generalization and robustness. However, training a single policy on
multi-robot data is challenging because robots can have widely varying sensors,
actuators, and control frequencies. We propose CrossFormer, a scalable and
flexible transformer-based policy that can consume data from any embodiment. We
train CrossFormer on the largest and most diverse dataset to date, 900K
trajectories across 20 different robot embodiments. We demonstrate that the
same network weights can control vastly different robots, including single and
dual arm manipulation systems, wheeled robots, quadcopters, and quadrupeds.
Unlike prior work, our model does not require manual alignment of the
observation or action spaces. Extensive experiments in the real world show that
our method matches the performance of specialist policies tailored for each
embodiment, while also significantly outperforming the prior state of the art
in cross-embodiment learning.

[Paper Link](
https://arxiv.org/abs/2408.11812
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_20-24.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-21


### ZebraPose: Zebra Detection and Pose Estimation using only Synthetic Data

- **Authors**: Elia Bonetto, Aamir Ahmad

#### Abstract

Synthetic data is increasingly being used to address the lack of labeled
images in uncommon domains for deep learning tasks. A prominent example is 2D
pose estimation of animals, particularly wild species like zebras, for which
collecting real-world data is complex and impractical. However, many approaches
still require real images, consistency and style constraints, sophisticated
animal models, and/or powerful pre-trained networks to bridge the syn-to-real
gap. Moreover, they often assume that the animal can be reliably detected in
images or videos, a hypothesis that often does not hold, e.g. in wildlife
scenarios or aerial images. To solve this, we use synthetic data generated with
a 3D photorealistic simulator to obtain the first synthetic dataset that can be
used for both detection and 2D pose estimation of zebras without applying any
of the aforementioned bridging strategies. Unlike previous works, we
extensively train and benchmark our detection and 2D pose estimation models on
multiple real-world and synthetic datasets using both pre-trained and
non-pre-trained backbones. These experiments show how the models trained from
scratch and only with synthetic data can consistently generalize to real-world
images of zebras in both tasks. Moreover, we show it is possible to easily
generalize those same models to 2D pose estimation of horses with a minimal
amount of real-world images to account for the domain transfer. Code, results,
trained models; and the synthetic, training, and validation data, including
104K manually labeled frames, are provided as open-source at
https://zebrapose.is.tue.mpg.de/

[Website Link](https://zebrapose.is.tue.mpg.de/)

[Paper Link](
https://arxiv.org/abs/2408.10831
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_20-12.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### RUMI: Rummaging Using Mutual Information

- **Authors**: Sheng Zhong, Nima Fazeli, Dmitry Berenson

#### Abstract

This paper presents Rummaging Using Mutual Information (RUMI), a method for
online generation of robot action sequences to gather information about the
pose of a known movable object in visually-occluded environments. Focusing on
contact-rich rummaging, our approach leverages mutual information between the
object pose distribution and robot trajectory for action planning. From an
observed partial point cloud, RUMI deduces the compatible object pose
distribution and approximates the mutual information of it with workspace
occupancy in real time. Based on this, we develop an information gain cost
function and a reachability cost function to keep the object within the robot's
reach. These are integrated into a model predictive control (MPC) framework
with a stochastic dynamics model, updating the pose distribution in a closed
loop. Key contributions include a new belief framework for object pose
estimation, an efficient information gain computation strategy, and a robust
MPC-based control scheme. RUMI demonstrates superior performance in both
simulated and real tasks compared to baseline methods.

[Paper Link](
https://arxiv.org/abs/2408.10450
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_19-50.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### All Robots in One: A New Standard and Unified Dataset for Versatile, General-Purpose Embodied Agents

- **Authors**: Zhiqiang Wang, Hao Zheng, Yunshuang Nie, Wenjun Xu, Qingwei Wang, Hua Ye, Zhe Li, Kaidong Zhang, Xuewen Cheng, Wanxi Dong, Chang Cai, Liang Lin, Feng Zheng, Xiaodan Liang

#### Abstract

Embodied AI is transforming how AI systems interact with the physical world,
yet existing datasets are inadequate for developing versatile, general-purpose
agents. These limitations include a lack of standardized formats, insufficient
data diversity, and inadequate data volume. To address these issues, we
introduce ARIO (All Robots In One), a new data standard that enhances existing
datasets by offering a unified data format, comprehensive sensory modalities,
and a combination of real-world and simulated data. ARIO aims to improve the
training of embodied AI agents, increasing their robustness and adaptability
across various tasks and environments. Building upon the proposed new standard,
we present a large-scale unified ARIO dataset, comprising approximately 3
million episodes collected from 258 series and 321,064 tasks. The ARIO standard
and dataset represent a significant step towards bridging the gaps of existing
data resources. By providing a cohesive framework for data collection and
representation, ARIO paves the way for the development of more powerful and
versatile embodied AI agents, capable of navigating and interacting with the
physical world in increasingly complex and diverse ways. The project is
available on https://imaei.github.io/project_pages/ario/

[Website Link](https://imaei.github.io/project_pages/ario/)

[Paper Link](
https://arxiv.org/abs/2408.10899
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_19-43.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### Enhancing End-to-End Autonomous Driving Systems Through Synchronized Human Behavior Data

- **Authors**: Yiqun Duan, Zhuoli Zhuang, Jinzhao Zhou, Yu-Cheng Chang, Yu-Kai Wang, Chin-Teng Lin

#### Abstract

This paper presents a pioneering exploration into the integration of
fine-grained human supervision within the autonomous driving domain to enhance
system performance. The current advances in End-to-End autonomous driving
normally are data-driven and rely on given expert trials. However, this
reliance limits the systems' generalizability and their ability to earn human
trust. Addressing this gap, our research introduces a novel approach by
synchronously collecting data from human and machine drivers under identical
driving scenarios, focusing on eye-tracking and brainwave data to guide machine
perception and decision-making processes. This paper utilizes the Carla
simulation to evaluate the impact brought by human behavior guidance.
Experimental results show that using human attention to guide machine attention
could bring a significant improvement in driving performance. However, guidance
by human intention still remains a challenge. This paper pioneers a promising
direction and potential for utilizing human behavior guidance to enhance
autonomous systems.

[Paper Link](
https://arxiv.org/abs/2408.10908
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_19-42.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-20


### LEGENT: Open Platform for Embodied Agents

- **Authors**: Zhili Cheng, Zhitong Wang, Jinyi Hu, Shengding Hu, An Liu, Yuge Tu, Pengkai Li, Lei Shi, Zhiyuan Liu, Maosong Sun

#### Abstract

Despite advancements in Large Language Models (LLMs) and Large Multimodal
Models (LMMs), their integration into language-grounded, human-like embodied
agents remains incomplete, hindering complex real-life task performance in
physical environments. Existing integrations often feature limited open
sourcing, challenging collective progress in this field. We introduce LEGENT,
an open, scalable platform for developing embodied agents using LLMs and LMMs.
LEGENT offers a dual approach: a rich, interactive 3D environment with
communicable and actionable agents, paired with a user-friendly interface, and
a sophisticated data generation pipeline utilizing advanced algorithms to
exploit supervision from simulated worlds at scale. In our experiments, an
embryonic vision-language-action model trained on LEGENT-generated data
surpasses GPT-4V in embodied tasks, showcasing promising generalization
capabilities.

[Paper Link](
https://arxiv.org/abs/2404.18243
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_19-39.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---

### ContactSDF: Signed Distance Functions as Multi-Contact Models for Dexterous Manipulation

- **Authors**: Wen Yang, Wanxin Jin

#### Abstract

In this paper, we propose ContactSDF, a method that uses signed distance
functions (SDFs) to approximate multi-contact models, including both collision
detection and time-stepping routines. ContactSDF first establishes an SDF using
the supporting plane representation of an object for collision detection, and
then use the generated contact dual cones to build a second SDF for time
stepping prediction of the next state. Those two SDFs create a differentiable
and closed-form multi-contact dynamic model for state prediction, enabling
efficient model learning and optimization for contact-rich manipulation. We
perform extensive simulation experiments to show the effectiveness of
ContactSDF for model learning and real-time control of dexterous manipulation.
We further evaluate the ContactSDF on a hardware Allegro hand for on-palm
reorientation tasks. Results show with around 2 minutes of learning on
hardware, the ContactSDF achieves high-quality dexterous manipulation at a
frequency of 30-60Hz.

[Paper Link](
https://arxiv.org/abs/2408.09612
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_19-20.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-19


### D5RL: Diverse Datasets for Data-Driven Deep Reinforcement Learning

- **Authors**: Rafael Rafailov, Kyle Hatch, Anikait Singh, Laura Smith, Aviral Kumar, Ilya Kostrikov, Philippe Hansen-Estruch, Victor Kolev, Philip Ball, Jiajun Wu, Chelsea Finn, Sergey Levine

#### Abstract

Offline reinforcement learning algorithms hold the promise of enabling
data-driven RL methods that do not require costly or dangerous real-world
exploration and benefit from large pre-collected datasets. This in turn can
facilitate real-world applications, as well as a more standardized approach to
RL research. Furthermore, offline RL methods can provide effective
initializations for online finetuning to overcome challenges with exploration.
However, evaluating progress on offline RL algorithms requires effective and
challenging benchmarks that capture properties of real-world tasks, provide a
range of task difficulties, and cover a range of challenges both in terms of
the parameters of the domain (e.g., length of the horizon, sparsity of rewards)
and the parameters of the data (e.g., narrow demonstration data or broad
exploratory data). While considerable progress in offline RL in recent years
has been enabled by simpler benchmark tasks, the most widely used datasets are
increasingly saturating in performance and may fail to reflect properties of
realistic tasks. We propose a new benchmark for offline RL that focuses on
realistic simulations of robotic manipulation and locomotion environments,
based on models of real-world robotic systems, and comprising a variety of data
sources, including scripted data, play-style data collected by human
teleoperators, and other data sources. Our proposed benchmark covers
state-based and image-based domains, and supports both offline RL and online
fine-tuning evaluation, with some of the tasks specifically designed to require
both pre-training and fine-tuning. We hope that our proposed benchmark will
facilitate further progress on both offline RL and fine-tuning algorithms.
Website with code, examples, tasks, and data is available at
\url{https://sites.google.com/view/d5rl/}

[Website Link](https://sites.google.com/view/d5rl/)

[Paper Link](
https://arxiv.org/abs/2408.08441
)

<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_17-45.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>
<div style={{ textAlign: "center", marginRight: "10px" }}>
    <img src="/img/daily/2024-10-19_17-46.png" alt="img" style={{ width: "auto", maxHeight: "400px" }} />
    </div>
<br/>

---
## 2024-08-16

### Autonomous Behavior Planning For Humanoid Loco-manipulation Through Grounded Language Model

- **Authors**: Jin Wang, Arturo Laurenzi, Nikos Tsagarakis

#### Abstract

Enabling humanoid robots to perform autonomously loco-manipulation in unstructured environments is crucial and highly challenging for achieving embodied intelligence. This involves robots being able to plan their actions and behaviors in long-horizon tasks while using multi-modality to perceive deviations between task execution and high-level planning. Recently, large language models (LLMs) have demonstrated powerful planning and reasoning capabilities for comprehension and processing of semantic information through robot control tasks, as well as the usability of analytical judgment and decision-making for multi-modal inputs. To leverage the power of LLMs towards humanoid loco-manipulation, we propose a novel language-model based framework that enables robots to autonomously plan behaviors and low-level execution under given textual instructions, while observing and correcting failures that may occur during task execution. To systematically evaluate this framework in grounding LLMs, we created the robot 'action' and 'sensing' behavior library for task planning, and conducted mobile manipulation tasks and experiments in both simulated and real environments using the CENTAURO robot, and verified the effectiveness and application of this approach in robotic tasks with autonomous behavioral planning.

[Paper Link](https://arxiv.org/abs/2408.08282)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-20_23-02.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-08-15

### Learning Multi-Modal Whole-Body Control for Real-World Humanoid Robots

- **Authors**: Pranay Dugar, Aayam Shrestha, Fangzhou Yu, Bart van Marum, Alan Fern

#### Abstract

We introduce the Masked Humanoid Controller (MHC) for whole-body tracking of target trajectories over arbitrary subsets of humanoid state variables. This enables the realization of whole-body motions from diverse sources such as video, motion capture, and VR, while ensuring balance and robustness against disturbances. The MHC is trained in simulation using a carefully designed curriculum that imitates partially masked motions from a library of behaviors spanning pre-trained policy rollouts, optimized reference trajectories, re-targeted video clips, and human motion capture data. We showcase simulation experiments validating the MHC's ability to execute a wide variety of behavior from partially-specified target motions. Moreover, we also highlight sim-to-real transfer as demonstrated by real-world trials on the Digit humanoid robot. To our knowledge, this is the first instance of a learned controller that can realize whole-body control of a real-world humanoid for such diverse multi-modal targets.

[Paper Link](https://arxiv.org/abs/2408.07295)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-20_22-57.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-08-14

### Grasping by Hanging: a Learning-Free Grasping Detection Method for Previously Unseen Objects

- **Authors**: Wanze Li, Wan Su, Gregory S. Chirikjian

#### Abstract

This paper proposes a novel learning-free three-stage method that predicts grasping poses, enabling robots to pick up and transfer previously unseen objects. Our method first identifies potential structures that can afford the action of hanging by analyzing the hanging mechanics and geometric properties. Then 6D poses are detected for a parallel gripper retrofitted with an extending bar, which when closed forms loops to hook each hangable structure. Finally, an evaluation policy qualities and rank grasp candidates for execution attempts. Compared to the traditional physical model-based and deep learning-based methods, our approach is closer to the human natural action of grasping unknown objects. And it also eliminates the need for a vast amount of training data. To evaluate the effectiveness of the proposed method, we conducted experiments with a real robot. Experimental results indicate that the grasping accuracy and stability are significantly higher than the state-of-the-art learning-based method, especially for thin and flat objects.

[Paper Link](https://arxiv.org/abs/2408.06734)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-20_22-21.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-08-02

### MuJoCo MPC for Humanoid Control: Evaluation on HumanoidBench

- **Authors**: Moritz Meser, Aditya Bhatt, Boris Belousov, Jan Peters

#### Abstract

We tackle the recently introduced benchmark for whole-body humanoid control HumanoidBench using MuJoCo MPC. We find that sparse reward functions of HumanoidBench yield undesirable and unrealistic behaviors when optimized; therefore, we propose a set of regularization terms that stabilize the robot behavior across tasks. Current evaluations on a subset of tasks demonstrate that our proposed reward function allows achieving the highest HumanoidBench scores while maintaining realistic posture and smooth control signals. Our code is publicly available and will become a part of MuJoCo MPC, enabling rapid prototyping of robot behaviors.

[Paper Link](https://arxiv.org/abs/2408.00342)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-13_00-42.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-08-01

### Berkeley Humanoid: A Research Platform for Learning-based Control

- **Authors**: Qiayuan Liao, Bike Zhang, Xuanyu Huang, Xiaoyu Huang, Zhongyu Li, Koushil Sreenath

#### Abstract

We introduce Berkeley Humanoid, a reliable and low-cost mid-scale humanoid research platform for learning-based control. Our lightweight, in-house-built robot is designed specifically for learning algorithms with low simulation complexity, anthropomorphic motion, and high reliability against falls. The robot's narrow sim-to-real gap enables agile and robust locomotion across various terrains in outdoor environments, achieved with a simple reinforcement learning controller using light domain randomization. Furthermore, we demonstrate the robot traversing for hundreds of meters, walking on a steep unpaved trail, and hopping with single and double legs as a testimony to its high performance in dynamical walking. Capable of omnidirectional locomotion and withstanding large perturbations with a compact setup, our system aims for scalable, sim-to-real deployment of learning-based humanoid systems. Please check this http URL for more details.

[Paper Link](https://arxiv.org/abs/2407.21781)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-13_00-39.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-25

### DexGANGrasp: Dexterous Generative Adversarial Grasping Synthesis for Task-Oriented Manipulation

- **Authors**: Qian Feng, David S. Martinez Lema, Mohammadhossein Malmir, Hang Li, Jianxiang Feng, Zhaopeng Chen, Alois Knoll

#### Abstract

We introduce DexGanGrasp, a dexterous grasping synthesis method that generates and evaluates grasps with single view in real time. DexGanGrasp comprises a Conditional Generative Adversarial Networks (cGANs)-based DexGenerator to generate dexterous grasps and a discriminator-like DexEvalautor to assess the stability of these grasps. Extensive simulation and real-world expriments showcases the effectiveness of our proposed method, outperforming the baseline FFHNet with an 18.57% higher success rate in real-world evaluation. We further extend DexGanGrasp to DexAfford-Prompt, an open-vocabulary affordance grounding pipeline for dexterous grasping leveraging Multimodal Large Language Models (MLLMs) and Vision Language Models (VLMs), to achieve task-oriented grasping with successful real-world deployments.

[Paper Link](https://arxiv.org/abs/2407.17348)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-13_00-20.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-24

### Cross Anything: General Quadruped Robot Navigation through Complex Terrains

- **Authors**: Shaoting Zhu, Derun Li, Yong Liu, Ningyi Xu, Hang Zhao

#### Abstract

The application of vision-language models (VLMs) has achieved impressive success in various robotics tasks, but there are few explorations for foundation models used in quadruped robot navigation. We introduce Cross Anything System (CAS), an innovative system composed of a high-level reasoning module and a low-level control policy, enabling the robot to navigate across complex 3D terrains and reach the goal position. For high-level reasoning and motion planning, we propose a novel algorithmic system taking advantage of a VLM, with a design of task decomposition and a closed-loop sub-task execution mechanism. For low-level locomotion control, we utilize the Probability Annealing Selection (PAS) method to train a control policy by reinforcement learning. Numerous experiments show that our whole system can accurately and robustly navigate across complex 3D terrains, and its strong generalization ability ensures the applications in diverse indoor and outdoor scenarios and terrains. Project page: this https URL

[Paper Link](https://arxiv.org/abs/2407.16412)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-13_00-07.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-08-12

### From Imitation to Refinement -- Residual RL for Precise Visual Assembly

- **Authors**: Lars Ankile, Anthony Simeonov, Idan Shenfeld, Marcel Torne, Pulkit Agrawal

#### Abstract

Behavior cloning (BC) currently stands as a dominant paradigm for learning real-world visual manipulation. However, in tasks that require locally corrective behaviors like multi-part assembly, learning robust policies purely from human demonstrations remains challenging. Reinforcement learning (RL) can mitigate these limitations by allowing policies to acquire locally corrective behaviors through task reward supervision and exploration. This paper explores the use of RL fine-tuning to improve upon BC-trained policies in precise manipulation tasks. We analyze and overcome technical challenges associated with using RL to directly train policy networks that incorporate modern architectural components like diffusion models and action chunking. We propose training residual policies on top of frozen BC-trained diffusion models using standard policy gradient methods and sparse rewards, an approach we call ResiP (Residual for Precise manipulation). Our experimental results demonstrate that this residual learning framework can significantly improve success rates beyond the base BC-trained models in high-precision assembly tasks by learning corrective actions. We also show that by combining ResiP with teacher-student distillation and visual domain randomization, our method can enable learning real-world policies for robotic assembly directly from RGB images. Find videos and code at \url{this https URL}.

[Paper Link](https://arxiv.org/abs/2407.16677)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-12_23-58.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### A Simulation Benchmark for Autonomous Racing with Large-Scale Human Data

- **Authors**: Adrian Remonda, Nicklas Hansen, Ayoub Raji, Nicola Musiu, Marko Bertogna, Eduardo Veas, Xiaolong Wang

#### Abstract

Despite the availability of international prize-money competitions, scaled vehicles, and simulation environments, research on autonomous racing and the control of sports cars operating close to the limit of handling has been limited by the high costs of vehicle acquisition and management, as well as the limited physics accuracy of open-source simulators. In this paper, we propose a racing simulation platform based on the simulator Assetto Corsa to test, validate, and benchmark autonomous driving algorithms, including reinforcement learning (RL) and classical Model Predictive Control (MPC), in realistic and challenging scenarios. Our contributions include the development of this simulation platform, several state-of-the-art algorithms tailored to the racing environment, and a comprehensive dataset collected from human drivers. Additionally, we evaluate algorithms in the offline RL setting. All the necessary code (including environment and benchmarks), working examples, datasets, and videos are publicly released and can be found at: this https URL

[Paper Link](https://arxiv.org/abs/2407.16680)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-08-12_23-55.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-23

### GET-Zero: Graph Embodiment Transformer for Zero-shot Embodiment Generalization

- **Authors**: Austin Patel, Shuran Song

#### Abstract

This paper introduces GET-Zero, a model architecture and training procedure for learning an embodiment-aware control policy that can immediately adapt to new hardware changes without retraining. To do so, we present Graph Embodiment Transformer (GET), a transformer model that leverages the embodiment graph connectivity as a learned structural bias in the attention mechanism. We use behavior cloning to distill demonstration data from embodiment-specific expert policies into an embodiment-aware GET model that conditions on the hardware configuration of the robot to make control decisions. We conduct a case study on a dexterous in-hand object rotation task using different configurations of a four-fingered robot hand with joints removed and with link length extensions. Using the GET model along with a self-modeling loss enables GET-Zero to zero-shot generalize to unseen variation in graph structure and link length, yielding a 20% improvement over baseline methods. All code and qualitative video results are on this https URL

[Paper Link](https://arxiv.org/abs/2407.15002)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_23-55.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-19

### R+X: Retrieval and Execution from Everyday Human Videos

- **Authors**: Georgios Papagiannis, Norman Di Palo, Pietro Vitiello, Edward Johns

#### Abstract

We present R+X, a framework which enables robots to learn skills from long, unlabelled, first-person videos of humans performing everyday tasks. Given a language command from a human, R+X first retrieves short video clips containing relevant behaviour, and then executes the skill by conditioning an in-context imitation learning method on this behaviour. By leveraging a Vision Language Model (VLM) for retrieval, R+X does not require any manual annotation of the videos, and by leveraging in-context learning for execution, robots can perform commanded skills immediately, without requiring a period of training on the retrieved videos. Experiments studying a range of everyday household tasks show that R+X succeeds at translating unlabelled human videos into robust robot skills, and that R+X outperforms several recent alternative methods. Videos are available at this https URL.

[Paper Link](https://arxiv.org/abs/2407.12957)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_23-43.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-18

### NavGPT-2: Unleashing Navigational Reasoning Capability for Large Vision-Language Models

- **Authors**: Gengze Zhou, Yicong Hong, Zun Wang, Xin Eric Wang, Qi Wu

#### Abstract

Capitalizing on the remarkable advancements in Large Language Models (LLMs), there is a burgeoning initiative to harness LLMs for instruction following robotic navigation. Such a trend underscores the potential of LLMs to generalize navigational reasoning and diverse language understanding. However, a significant discrepancy in agent performance is observed when integrating LLMs in the Vision-and-Language navigation (VLN) tasks compared to previous downstream specialist models. Furthermore, the inherent capacity of language to interpret and facilitate communication in agent interactions is often underutilized in these integrations. In this work, we strive to bridge the divide between VLN-specialized models and LLM-based navigation paradigms, while maintaining the interpretative prowess of LLMs in generating linguistic navigational reasoning. By aligning visual content in a frozen LLM, we encompass visual observation comprehension for LLMs and exploit a way to incorporate LLMs and navigation policy networks for effective action predictions and navigational reasoning. We demonstrate the data efficiency of the proposed methods and eliminate the gap between LM-based agents and state-of-the-art VLN specialists.

[Paper Link](https://arxiv.org/abs/2407.12366)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_23-27.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-17

### ThinkGrasp: A Vision-Language System for Strategic Part Grasping in Clutter

- **Authors**: Yaoyao Qian, Xupeng Zhu, Ondrej Biza, Shuo Jiang, Linfeng Zhao, Haojie Huang, Yu Qi, Robert Platt

#### Abstract

Robotic grasping in cluttered environments remains a significant challenge due to occlusions and complex object arrangements. We have developed ThinkGrasp, a plug-and-play vision-language grasping system that makes use of GPT-4o's advanced contextual reasoning for heavy clutter environment grasping strategies. ThinkGrasp can effectively identify and generate grasp poses for target objects, even when they are heavily obstructed or nearly invisible, by using goal-oriented language to guide the removal of obstructing objects. This approach progressively uncovers the target object and ultimately grasps it with a few steps and a high success rate. In both simulated and real experiments, ThinkGrasp achieved a high success rate and significantly outperformed state-of-the-art methods in heavily cluttered environments or with diverse unseen objects, demonstrating strong generalization capabilities.

[Paper Link](https://arxiv.org/abs/2407.11298)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_23-17.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Grasping Diverse Objects with Simulated Humanoids

- **Authors**: Zhengyi Luo, Jinkun Cao, Sammy Christen, Alexander Winkler, Kris Kitani, Weipeng Xu

#### Abstract

We present a method for controlling a simulated humanoid to grasp an object and move it to follow an object trajectory. Due to the challenges in controlling a humanoid with dexterous hands, prior methods often use a disembodied hand and only consider vertical lifts or short trajectories. This limited scope hampers their applicability for object manipulation required for animation and simulation. To close this gap, we learn a controller that can pick up a large number (>1200) of objects and carry them to follow randomly generated trajectories. Our key insight is to leverage a humanoid motion representation that provides human-like motor skills and significantly speeds up training. Using only simplistic reward, state, and object representations, our method shows favorable scalability on diverse object and trajectories. For training, we do not need dataset of paired full-body motion and object trajectories. At test time, we only require the object mesh and desired trajectories for grasping and transporting. To demonstrate the capabilities of our method, we show state-of-the-art success rates in following object trajectories and generalizing to unseen objects. Code and models will be released.

[Paper Link](https://arxiv.org/abs/2407.11385)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_23-06.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-16

### DexGrasp-Diffusion: Diffusion-based Unified Functional Grasp Synthesis Pipeline for Multi-Dexterous Robotic Hands

- **Authors**: Zhengshen Zhang, Lei Zhou, Chenchen Liu, Zhiyang Liu, Chengran Yuan, Sheng Guo, Ruiteng Zhao, Marcelo H. Ang Jr., Francis EH Tay

#### Abstract

The versatility and adaptability of human grasping catalyze advancing dexterous robotic manipulation. While significant strides have been made in dexterous grasp generation, current research endeavors pivot towards optimizing object manipulation while ensuring functional integrity, emphasizing the synthesis of functional grasps following desired affordance instructions. This paper addresses the challenge of synthesizing functional grasps tailored to diverse dexterous robotic hands by proposing DexGrasp-Diffusion, an end-to-end modularized diffusion-based pipeline. DexGrasp-Diffusion integrates MultiHandDiffuser, a novel unified data-driven diffusion model for multi-dexterous hands grasp estimation, with DexDiscriminator, which employs a Physics Discriminator and a Functional Discriminator with open-vocabulary setting to filter physically plausible functional grasps based on object affordances. The experimental evaluation conducted on the MultiDex dataset provides substantiating evidence supporting the superior performance of MultiHandDiffuser over the baseline model in terms of success rate, grasp diversity, and collision depth. Moreover, we demonstrate the capacity of DexGrasp-Diffusion to reliably generate functional grasps for household objects aligned with specific affordance instructions.

[Paper Link](https://arxiv.org/abs/2407.09899)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-54.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### UMI on Legs: Making Manipulation Policies Mobile with Manipulation-Centric Whole-body Controllers

- **Authors**: Huy Ha, Yihuai Gao, Zipeng Fu, Jie Tan, Shuran Song

#### Abstract

We introduce UMI-on-Legs, a new framework that combines real-world and simulation data for quadruped manipulation systems. We scale task-centric data collection in the real world using a hand-held gripper (UMI), providing a cheap way to demonstrate task-relevant manipulation skills without a robot. Simultaneously, we scale robot-centric data in simulation by training whole-body controller for task-tracking without task simulation setups. The interface between these two policies is end-effector trajectories in the task frame, inferred by the manipulation policy and passed to the whole-body controller for tracking. We evaluate UMI-on-Legs on prehensile, non-prehensile, and dynamic manipulation tasks, and report over 70% success rate on all tasks. Lastly, we demonstrate the zero-shot cross-embodiment deployment of a pre-trained manipulation policy checkpoint from prior work, originally intended for a fixed-base robot arm, on our quadruped system. We believe this framework provides a scalable path towards learning expressive manipulation skills on dynamic robot embodiments. Please checkout our website for robot videos, code, and data: this https URL

[Paper Link](https://arxiv.org/abs/2407.10353)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-43.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-12

### OmniNOCS: A unified NOCS dataset and model for 3D lifting of 2D objects

- **Authors**: Akshay Krishnan, Abhijit Kundu, Kevis-Kokitsi Maninis, James Hays, Matthew Brown

#### Abstract

We propose OmniNOCS, a large-scale monocular dataset with 3D Normalized Object Coordinate Space (NOCS) maps, object masks, and 3D bounding box annotations for indoor and outdoor scenes. OmniNOCS has 20 times more object classes and 200 times more instances than existing NOCS datasets (NOCS-Real275, Wild6D). We use OmniNOCS to train a novel, transformer-based monocular NOCS prediction model (NOCSformer) that can predict accurate NOCS, instance masks and poses from 2D object detections across diverse classes. It is the first NOCS model that can generalize to a broad range of classes when prompted with 2D boxes. We evaluate our model on the task of 3D oriented bounding box prediction, where it achieves comparable results to state-of-the-art 3D detection methods such as Cube R-CNN. Unlike other 3D detection methods, our model also provides detailed and accurate 3D object shape and segmentation. We propose a novel benchmark for the task of NOCS prediction based on OmniNOCS, which we hope will serve as a useful baseline for future work in this area. Our dataset and code will be at the project website: this https URL.

[Paper Link](https://arxiv.org/abs/2407.08711)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-27.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### MetaUrban: A Simulation Platform for Embodied AI in Urban Spaces

- **Authors**: Wayne Wu, Honglin He, Yiran Wang, Chenda Duan, Jack He, Zhizheng Liu, Quanyi Li, Bolei Zhou

#### Abstract

Public urban spaces like streetscapes and plazas serve residents and accommodate social life in all its vibrant variations. Recent advances in Robotics and Embodied AI make public urban spaces no longer exclusive to humans. Food delivery bots and electric wheelchairs have started sharing sidewalks with pedestrians, while diverse robot dogs and humanoids have recently emerged in the street. Ensuring the generalizability and safety of these forthcoming mobile machines is crucial when navigating through the bustling streets in urban spaces. In this work, we present MetaUrban, a compositional simulation platform for Embodied AI research in urban spaces. MetaUrban can construct an infinite number of interactive urban scenes from compositional elements, covering a vast array of ground plans, object placements, pedestrians, vulnerable road users, and other mobile agents' appearances and dynamics. We design point navigation and social navigation tasks as the pilot study using MetaUrban for embodied AI research and establish various baselines of Reinforcement Learning and Imitation Learning. Experiments demonstrate that the compositional nature of the simulated environments can substantially improve the generalizability and safety of the trained mobile agents. MetaUrban will be made publicly available to provide more research opportunities and foster safe and trustworthy embodied AI in urban spaces.

[Paper Link](https://arxiv.org/abs/2407.08725)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-26.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Robotic Control via Embodied Chain-of-Thought Reasoning

- **Authors**: Michał Zawalski, William Chen, Karl Pertsch, Oier Mees, Chelsea Finn, Sergey Levine

#### Abstract

A key limitation of learned robot control policies is their inability to generalize outside their training data. Recent works on vision-language-action models (VLAs) have shown that the use of large, internet pre-trained vision-language models as the backbone of learned robot policies can substantially improve their robustness and generalization ability. Yet, one of the most exciting capabilities of large vision-language models in other domains is their ability to reason iteratively through complex problems. Can that same capability be brought into robotics to allow policies to improve performance by reasoning about a given task before acting? Naive use of "chain-of-thought" (CoT) style prompting is significantly less effective with standard VLAs because of the relatively simple training examples that are available to them. Additionally, purely semantic reasoning about sub-tasks, as is common in regular CoT, is insufficient for robot policies that need to ground their reasoning in sensory observations and the robot state. To this end, we introduce Embodied Chain-of-Thought Reasoning (ECoT) for VLAs, in which we train VLAs to perform multiple steps of reasoning about plans, sub-tasks, motions, and visually grounded features like object bounding boxes and end effector positions, before predicting the robot action. We design a scalable pipeline for generating synthetic training data for ECoT on large robot datasets. We demonstrate, that ECoT increases the absolute success rate of OpenVLA, the current strongest open-source VLA policy, by 28% across challenging generalization tasks, without any additional robot training data. Additionally, ECoT makes it easier for humans to interpret a policy's failures and correct its behavior using natural language.

[Paper Link](https://arxiv.org/abs/2407.08693)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-16.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-11

### FLAIR: Feeding via Long-horizon AcquIsition of Realistic dishes

- **Authors**: Rajat Kumar Jenamani, Priya Sundaresan, Maram Sakr, Tapomayukh Bhattacharjee, Dorsa Sadigh

#### Abstract

Robot-assisted feeding has the potential to improve the quality of life for individuals with mobility limitations who are unable to feed themselves independently. However, there exists a large gap between the homogeneous, curated plates existing feeding systems can handle, and truly in-the-wild meals. Feeding realistic plates is immensely challenging due to the sheer range of food items that a robot may encounter, each requiring specialized manipulation strategies which must be sequenced over a long horizon to feed an entire meal. An assistive feeding system should not only be able to sequence different strategies efficiently in order to feed an entire meal, but also be mindful of user preferences given the personalized nature of the task. We address this with FLAIR, a system for long-horizon feeding which leverages the commonsense and few-shot reasoning capabilities of foundation models, along with a library of parameterized skills, to plan and execute user-preferred and efficient bite sequences. In real-world evaluations across 6 realistic plates, we find that FLAIR can effectively tap into a varied library of skills for efficient food pickup, while adhering to the diverse preferences of 42 participants without mobility limitations as evaluated in a user study. We demonstrate the seamless integration of FLAIR with existing bite transfer methods [19, 28], and deploy it across 2 institutions and 3 robots, illustrating its adaptability. Finally, we illustrate the real-world efficacy of our system by successfully feeding a care recipient with severe mobility limitations. Supplementary materials and videos can be found at: this https URL .

[Paper Link](https://arxiv.org/abs/2407.07561)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-11.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Mobility VLA: Multimodal Instruction Navigation with Long-Context VLMs and Topological Graphs

- **Authors**: Hao-Tien Lewis Chiang, Zhuo Xu, Zipeng Fu, Mithun George Jacob, Tingnan Zhang, Tsang-Wei Edward Lee, Wenhao Yu, Connor Schenck, David Rendleman, Dhruv Shah, Fei Xia, Jasmine Hsu, Jonathan Hoech, Pete Florence, Sean Kirmani, Sumeet Singh, Vikas Sindhwani, Carolina Parada, Chelsea Finn, Peng Xu, Sergey Levine, Jie Tan

#### Abstract

An elusive goal in navigation research is to build an intelligent agent that can understand multimodal instructions including natural language and image, and perform useful navigation. To achieve this, we study a widely useful category of navigation tasks we call Multimodal Instruction Navigation with demonstration Tours (MINT), in which the environment prior is provided through a previously recorded demonstration video. Recent advances in Vision Language Models (VLMs) have shown a promising path in achieving this goal as it demonstrates capabilities in perceiving and reasoning about multimodal inputs. However, VLMs are typically trained to predict textual output and it is an open research question about how to best utilize them in navigation. To solve MINT, we present Mobility VLA, a hierarchical Vision-Language-Action (VLA) navigation policy that combines the environment understanding and common sense reasoning power of long-context VLMs and a robust low-level navigation policy based on topological graphs. The high-level policy consists of a long-context VLM that takes the demonstration tour video and the multimodal user instruction as input to find the goal frame in the tour video. Next, a low-level policy uses the goal frame and an offline constructed topological graph to generate robot actions at every timestep. We evaluated Mobility VLA in a 836m^2 real world environment and show that Mobility VLA has a high end-to-end success rates on previously unsolved multimodal instructions such as "Where should I return this?" while holding a plastic bin. A video demonstrating Mobility VLA can be found here: this https URL

[Paper Link](https://arxiv.org/abs/2407.07775)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-08.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### BiGym: A Demo-Driven Mobile Bi-Manual Manipulation Benchmark

- **Authors**: Nikita Chernyadev, Nicholas Backshall, Xiao Ma, Yunfan Lu, Younggyo Seo, Stephen James

#### Abstract

We introduce BiGym, a new benchmark and learning environment for mobile bi-manual demo-driven robotic manipulation. BiGym features 40 diverse tasks set in home environments, ranging from simple target reaching to complex kitchen cleaning. To capture the real-world performance accurately, we provide human-collected demonstrations for each task, reflecting the diverse modalities found in real-world robot trajectories. BiGym supports a variety of observations, including proprioceptive data and visual inputs such as RGB, and depth from 3 camera views. To validate the usability of BiGym, we thoroughly benchmark the state-of-the-art imitation learning algorithms and demo-driven reinforcement learning algorithms within the environment and discuss the future opportunities.

[Paper Link](https://arxiv.org/abs/2407.07788)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-01.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Green Screen Augmentation Enables Scene Generalisation in Robotic Manipulation

- **Authors**: Eugene Teoh, Sumit Patidar, Xiao Ma, Stephen James

#### Abstract

Generalising vision-based manipulation policies to novel environments remains a challenging area with limited exploration. Current practices involve collecting data in one location, training imitation learning or reinforcement learning policies with this data, and deploying the policy in the same location. However, this approach lacks scalability as it necessitates data collection in multiple locations for each task. This paper proposes a novel approach where data is collected in a location predominantly featuring green screens. We introduce Green-screen Augmentation (GreenAug), employing a chroma key algorithm to overlay background textures onto a green screen. Through extensive real-world empirical studies with over 850 training demonstrations and 8.2k evaluation episodes, we demonstrate that GreenAug surpasses no augmentation, standard computer vision augmentation, and prior generative augmentation methods in performance. While no algorithmic novelties are claimed, our paper advocates for a fundamental shift in data collection practices. We propose that real-world demonstrations in future research should utilise green screens, followed by the application of GreenAug. We believe GreenAug unlocks policy generalisation to visually distinct novel locations, addressing the current scene generalisation limitations in robot learning.

[Paper Link](https://arxiv.org/abs/2407.07868)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-00_1.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Generative Image as Action Models

- **Authors**: Mohit Shridhar, Yat Long Lo, Stephen James

#### Abstract

Image-generation diffusion models have been fine-tuned to unlock new capabilities such as image-editing and novel view synthesis. Can we similarly unlock image-generation models for visuomotor control? We present GENIMA, a behavior-cloning agent that fine-tunes Stable Diffusion to 'draw joint-actions' as targets on RGB images. These images are fed into a controller that maps the visual targets into a sequence of joint-positions. We study GENIMA on 25 RLBench and 9 real-world manipulation tasks. We find that, by lifting actions into image-space, internet pre-trained diffusion models can generate policies that outperform state-of-the-art visuomotor approaches, especially in robustness to scene perturbations and generalizing to novel objects. Our method is also competitive with 3D agents, despite lacking priors such as depth, keypoints, or motion-planners.

[Paper Link](https://arxiv.org/abs/2407.07875)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_22-00.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Vegetable Peeling: A Case Study in Constrained Dexterous Manipulation

- **Authors**: Tao Chen, Eric Cousineau, Naveen Kuppuswamy, Pulkit Agrawal

#### Abstract

Recent studies have made significant progress in addressing dexterous manipulation problems, particularly in in-hand object reorientation. However, there are few existing works that explore the potential utilization of developed dexterous manipulation controllers for downstream tasks. In this study, we focus on constrained dexterous manipulation for food peeling. Food peeling presents various constraints on the reorientation controller, such as the requirement for the hand to securely hold the object after reorientation for peeling. We propose a simple system for learning a reorientation controller that facilitates the subsequent peeling task. Videos are available at: this https URL.

[Paper Link](https://arxiv.org/abs/2407.07884)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_21-58.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Learning In-Hand Translation Using Tactile Skin With Shear and Normal Force Sensing

- **Authors**: Jessica Yin, Haozhi Qi, Jitendra Malik, James Pikul, Mark Yim, Tess Hellebrekers

#### Abstract

Recent progress in reinforcement learning (RL) and tactile sensing has significantly advanced dexterous manipulation. However, these methods often utilize simplified tactile signals due to the gap between tactile simulation and the real world. We introduce a sensor model for tactile skin that enables zero-shot sim-to-real transfer of ternary shear and binary normal forces. Using this model, we develop an RL policy that leverages sliding contact for dexterous in-hand translation. We conduct extensive real-world experiments to assess how tactile sensing facilitates policy adaptation to various unseen object properties and robot hand orientations. We demonstrate that our 3-axis tactile policies consistently outperform baselines that use only shear forces, only normal forces, or only proprioception. Website: this https URL

[Paper Link](https://arxiv.org/abs/2407.07885)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-24_21-56.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-09

### JaywalkerVR: A VR System for Collecting Safety-Critical Pedestrian-Vehicle Interactions

- **Authors**: Kenta Mukoya, Erica Weng, Rohan Choudhury, Kris Kitani

#### Abstract

Developing autonomous vehicles that can safely interact with pedestrians requires large amounts of pedestrian and vehicle data in order to learn accurate pedestrian-vehicle interaction models. However, gathering data that include crucial but rare scenarios - such as pedestrians jaywalking into heavy traffic - can be costly and unsafe to collect. We propose a virtual reality human-in-the-loop simulator, JaywalkerVR, to obtain vehicle-pedestrian interaction data to address these challenges. Our system enables efficient, affordable, and safe collection of long-tail pedestrian-vehicle interaction data. Using our proposed simulator, we create a high-quality dataset with vehicle-pedestrian interaction data from safety critical scenarios called CARLA-VR. The CARLA-VR dataset addresses the lack of long-tail data samples in commonly used real world autonomous driving datasets. We demonstrate that models trained with CARLA-VR improve displacement error and collision rate by 10.7% and 4.9%, respectively, and are more robust in rare vehicle-pedestrian scenarios.

[Paper Link](https://arxiv.org/abs/2407.04843)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-12_00-31.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### ClutterGen: A Cluttered Scene Generator for Robot Learning

- **Authors**: Yinsen Jia, Boyuan Chen

#### Abstract

We introduce ClutterGen, a physically compliant simulation scene generator capable of producing highly diverse, cluttered, and stable scenes for robot learning. Generating such scenes is challenging as each object must adhere to physical laws like gravity and collision. As the number of objects increases, finding valid poses becomes more difficult, necessitating significant human engineering effort, which limits the diversity of the scenes. To overcome these challenges, we propose a reinforcement learning method that can be trained with physics-based reward signals provided by the simulator. Our experiments demonstrate that ClutterGen can generate cluttered object layouts with up to ten objects on confined table surfaces. Additionally, our policy design explicitly encourages the diversity of the generated scenes for open-ended generation. Our real-world robot results show that ClutterGen can be directly used for clutter rearrangement and stable placement policy training.

[Paper Link](https://arxiv.org/abs/2407.05425)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-12_00-26.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### TARGO: Benchmarking Target-driven Object Grasping under Occlusions

- **Authors**: Yan Xia, Ran Ding, Ziyuan Qin, Guanqi Zhan, Kaichen Zhou, Long Yang, Hao Dong, Daniel Cremers

#### Abstract

Recent advances in predicting 6D grasp poses from a single depth image have led to promising performance in robotic grasping. However, previous grasping models face challenges in cluttered environments where nearby objects impact the target object's grasp. In this paper, we first establish a new benchmark dataset for TARget-driven Grasping under Occlusions, named TARGO. We make the following contributions: 1) We are the first to study the occlusion level of grasping. 2) We set up an evaluation benchmark consisting of large-scale synthetic data and part of real-world data, and we evaluated five grasp models and found that even the current SOTA model suffers when the occlusion level increases, leaving grasping under occlusion still a challenge. 3) We also generate a large-scale training dataset via a scalable pipeline, which can be used to boost the performance of grasping under occlusion and generalized to the real world. 4) We further propose a transformer-based grasping model involving a shape completion module, termed TARGO-Net, which performs most robustly as occlusion increases. Our benchmark dataset can be found at this https URL.

[Paper Link](https://arxiv.org/abs/2407.06168)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-12_00-16.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-08

### VoxAct-B: Voxel-Based Acting and Stabilizing Policy for Bimanual Manipulation

- **Authors**: I-Chun Arthur Liu, Sicheng He, Daniel Seita, Gaurav Sukhatme

#### Abstract

Bimanual manipulation is critical to many robotics applications. In contrast to single-arm manipulation, bimanual manipulation tasks are challenging due to higher-dimensional action spaces. Prior works leverage large amounts of data and primitive actions to address this problem, but may suffer from sample inefficiency and limited generalization across various tasks. To this end, we propose VoxAct-B, a language-conditioned, voxel-based method that leverages Vision Language Models (VLMs) to prioritize key regions within the scene and reconstruct a voxel grid. We provide this voxel grid to our bimanual manipulation policy to learn acting and stabilizing actions. This approach enables more efficient policy learning from voxels and is generalizable to different tasks. In simulation, we show that VoxAct-B outperforms strong baselines on fine-grained bimanual manipulation tasks. Furthermore, we demonstrate VoxAct-B on real-world $\texttt{Open Drawer}$ and $\texttt{Open Jar}$ tasks using two UR5s. Code, data, and videos will be available at this https URL.

[Paper Link](https://arxiv.org/abs/2407.04152)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-11_23-55.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### RAM: Retrieval-Based Affordance Transfer for Generalizable Zero-Shot Robotic Manipulation

- **Authors**: Yuxuan Kuang, Junjie Ye, Haoran Geng, Jiageng Mao, Congyue Deng, Leonidas Guibas, He Wang, Yue Wang

#### Abstract

This work proposes a retrieve-and-transfer framework for zero-shot robotic manipulation, dubbed RAM, featuring generalizability across various objects, environments, and embodiments. Unlike existing approaches that learn manipulation from expensive in-domain demonstrations, RAM capitalizes on a retrieval-based affordance transfer paradigm to acquire versatile manipulation capabilities from abundant out-of-domain data. First, RAM extracts unified affordance at scale from diverse sources of demonstrations including robotic data, human-object interaction (HOI) data, and custom data to construct a comprehensive affordance memory. Then given a language instruction, RAM hierarchically retrieves the most similar demonstration from the affordance memory and transfers such out-of-domain 2D affordance to in-domain 3D executable affordance in a zero-shot and embodiment-agnostic manner. Extensive simulation and real-world evaluations demonstrate that our RAM consistently outperforms existing works in diverse daily tasks. Additionally, RAM shows significant potential for downstream applications such as automatic and efficient data collection, one-shot visual imitation, and LLM/VLM-integrated long-horizon manipulation. For more details, please check our website at this https URL.

[Paper Link](https://arxiv.org/abs/2407.04689)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-11_23-50.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-04

### IntentionNet: Map-Lite Visual Navigation at the Kilometre Scale

- **Authors**: Wei Gao, Bo Ai, Joel Loo, Vinay, David Hsu

#### Abstract

This work explores the challenges of creating a scalable and robust robot navigation system that can traverse both indoor and outdoor environments to reach distant goals. We propose a navigation system architecture called IntentionNet that employs a monolithic neural network as the low-level planner/controller, and uses a general interface that we call intentions to steer the controller. The paper proposes two types of intentions, Local Path and Environment (LPE) and Discretised Local Move (DLM), and shows that DLM is robust to significant metric positioning and mapping errors. The paper also presents Kilo-IntentionNet, an instance of the IntentionNet system using the DLM intention that is deployed on a Boston Dynamics Spot robot, and which successfully navigates through complex indoor and outdoor environments over distances of up to a kilometre with only noisy odometry.

[Paper Link](https://arxiv.org/abs/2407.03122)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-07_21-29.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### TieBot: Learning to Knot a Tie from Visual Demonstration through a Real-to-Sim-to-Real Approach

- **Authors**: Weikun Peng, Jun Lv, Yuwei Zeng, Haonan Chen, Siheng Zhao, Jicheng Sun, Cewu Lu, Lin Shao

#### Abstract

The tie-knotting task is highly challenging due to the tie's high deformation and long-horizon manipulation actions. This work presents TieBot, a Real-to-Sim-to-Real learning from visual demonstration system for the robots to learn to knot a tie. We introduce the Hierarchical Feature Matching approach to estimate a sequence of tie's meshes from the demonstration video. With these estimated meshes used as subgoals, we first learn a teacher policy using privileged information. Then, we learn a student policy with point cloud observation by imitating teacher policy. Lastly, our pipeline learns a residual policy when the learned policy is applied to real-world execution, mitigating the Sim2Real gap. We demonstrate the effectiveness of TieBot in simulation and the real world. In the real-world experiment, a dual-arm robot successfully knots a tie, achieving 50% success rate among 10 trials. Videos can be found on our $\href{this https URL}{\text{website}}$.

[Paper Link](https://arxiv.org/abs/2407.03245)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-07_21-25.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-03

### Learning Granular Media Avalanche Behavior for Indirectly Manipulating Obstacles on a Granular Slope

- **Authors**: Haodi Hu, Feifei Qian, Daniel Seita

#### Abstract

Legged robot locomotion on sand slopes is challenging due to the complex dynamics of granular media and how the lack of solid surfaces can hinder locomotion. A promising strategy, inspired by ghost crabs and other organisms in nature, is to strategically interact with rocks, debris, and other obstacles to facilitate movement. To provide legged robots with this ability, we present a novel approach that leverages avalanche dynamics to indirectly manipulate objects on a granular slope. We use a Vision Transformer (ViT) to process image representations of granular dynamics and robot excavation actions. The ViT predicts object movement, which we use to determine which leg excavation action to execute. We collect training data from 100 real physical trials and, at test time, deploy our trained model in novel settings. Experimental results suggest that our model can accurately predict object movements and achieve a success rate $\geq 80\%$ in a variety of manipulation tasks with up to four obstacles, and can also generalize to objects with different physics properties. To our knowledge, this is the first paper to leverage granular media avalanche dynamics to indirectly manipulate objects on granular slopes. Supplementary material is available at this https URL.

[Paper Link](https://arxiv.org/abs/2407.01898)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-49.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Open Scene Graphs for Open World Object-Goal Navigation

- **Authors**: Joel Loo, Zhanxin Wu, David Hsu

#### Abstract

How can we build robots for open-world semantic navigation tasks, like searching for target objects in novel scenes? While foundation models have the rich knowledge and generalisation needed for these tasks, a suitable scene representation is needed to connect them into a complete robot system. We address this with Open Scene Graphs (OSGs), a topo-semantic representation that retains and organises open-set scene information for these models, and has a structure that can be configured for different environment types. We integrate foundation models and OSGs into the OpenSearch system for Open World Object-Goal Navigation, which is capable of searching for open-set objects specified in natural language, while generalising zero-shot across diverse environments and embodiments. Our OSGs enhance reasoning with Large Language Models (LLM), enabling robust object-goal navigation outperforming existing LLM approaches. Through simulation and real-world experiments, we validate OpenSearch's generalisation across varied environments, robots and novel instructions.

[Paper Link](https://arxiv.org/abs/2407.02473)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-42.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-02

### Tokenize the World into Object-level Knowledge to Address Long-tail Events in Autonomous Driving

- **Authors**: Ran Tian, Boyi Li, Xinshuo Weng, Yuxiao Chen, Edward Schmerling, Yue Wang, Boris Ivanovic, Marco Pavone

#### Abstract

The autonomous driving industry is increasingly adopting end-to-end learning from sensory inputs to minimize human biases in system design. Traditional end-to-end driving models, however, suffer from long-tail events due to rare or unseen inputs within their training distributions. To address this, we propose TOKEN, a novel Multi-Modal Large Language Model (MM-LLM) that tokenizes the world into object-level knowledge, enabling better utilization of LLM's reasoning capabilities to enhance autonomous vehicle planning in long-tail scenarios. TOKEN effectively alleviates data scarcity and inefficient tokenization by leveraging a traditional end-to-end driving model to produce condensed and semantically enriched representations of the scene, which are optimized for LLM planning compatibility through deliberate representation and reasoning alignment training stages. Our results demonstrate that TOKEN excels in grounding, reasoning, and planning capabilities, outperforming existing frameworks with a 27% reduction in trajectory L2 error and a 39% decrease in collision rates in long-tail scenarios. Additionally, our work highlights the importance of representation alignment and structured reasoning in sparking the common-sense reasoning capabilities of MM-LLMs for effective planning.

[Paper Link](https://arxiv.org/abs/2407.00959)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-40.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-07-01

### HumanVLA: Towards Vision-Language Directed Object Rearrangement by Physical Humanoid

- **Authors**: Xinyu Xu, Yizheng Zhang, Yong-Lu Li, Lei Han, Cewu Lu

#### Abstract

Physical Human-Scene Interaction (HSI) plays a crucial role in numerous applications. However, existing HSI techniques are limited to specific object dynamics and privileged information, which prevents the development of more comprehensive applications. To address this limitation, we introduce HumanVLA for general object rearrangement directed by practical vision and language. A teacher-student framework is utilized to develop HumanVLA. A state-based teacher policy is trained first using goal-conditioned reinforcement learning and adversarial motion prior. Then, it is distilled into a vision-language-action model via behavior cloning. We propose several key insights to facilitate the large-scale learning process. To support general object rearrangement by physical humanoid, we introduce a novel Human-in-the-Room dataset encompassing various rearrangement tasks. Through extensive experiments and analysis, we demonstrate the effectiveness of the proposed approach.

[Paper Link](https://arxiv.org/abs/2406.19972)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-29.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-28

### Human-Aware Vision-and-Language Navigation: Bridging Simulation to Reality with Dynamic Human Interactions

- **Authors**: Minghan Li, Heng Li, Zhi-Qi Cheng, Yifei Dong, Yuxuan Zhou, Jun-Yan He, Qi Dai, Teruko Mitamura, Alexander G. Hauptmann

#### Abstract

Vision-and-Language Navigation (VLN) aims to develop embodied agents that navigate based on human instructions. However, current VLN frameworks often rely on static environments and optimal expert supervision, limiting their real-world applicability. To address this, we introduce Human-Aware Vision-and-Language Navigation (HA-VLN), extending traditional VLN by incorporating dynamic human activities and relaxing key assumptions. We propose the Human-Aware 3D (HA3D) simulator, which combines dynamic human activities with the Matterport3D dataset, and the Human-Aware Room-to-Room (HA-R2R) dataset, extending R2R with human activity descriptions. To tackle HA-VLN challenges, we present the Expert-Supervised Cross-Modal (VLN-CM) and Non-Expert-Supervised Decision Transformer (VLN-DT) agents, utilizing cross-modal fusion and diverse training strategies for effective navigation in dynamic human environments. A comprehensive evaluation, including metrics considering human activities, and systematic analysis of HA-VLN's unique challenges, underscores the need for further research to enhance HA-VLN agents' real-world robustness and adaptability. Ultimately, this work provides benchmarks and insights for future research on embodied AI and Sim2Real transfer, paving the way for more realistic and applicable VLN systems in human-populated environments.

[Paper Link](https://arxiv.org/abs/2406.19236)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-26.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Manipulate-Anything: Automating Real-World Robots using Vision-Language Models

- **Authors**: Jiafei Duan, Wentao Yuan, Wilbert Pumacay, Yi Ru Wang, Kiana Ehsani, Dieter Fox, Ranjay Krishna

#### Abstract

Large-scale endeavors like RT-1 and widespread community efforts such as Open-X-Embodiment have contributed to growing the scale of robot demonstration data. However, there is still an opportunity to improve the quality, quantity, and diversity of robot demonstration data. Although vision-language models have been shown to automatically generate demonstration data, their utility has been limited to environments with privileged state information, they require hand-designed skills, and are limited to interactions with few object instances. We propose Manipulate-Anything, a scalable automated generation method for real-world robotic manipulation. Unlike prior work, our method can operate in real-world environments without any privileged state information, hand-designed skills, and can manipulate any static object. We evaluate our method using two setups. First, Manipulate-Anything successfully generates trajectories for all 5 real-world and 12 simulation tasks, significantly outperforming existing methods like VoxPoser. Second, Manipulate-Anything's demonstrations can train more robust behavior cloning policies than training with human demonstrations, or from data generated by VoxPoser and Code-As-Policies. We believe Manipulate-Anything can be the scalable method for both generating data for robotics and solving novel tasks in a zero-shot setting.

[Paper Link](https://arxiv.org/abs/2406.18915)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-24.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-27

### Open-vocabulary Mobile Manipulation in Unseen Dynamic Environments with 3D Semantic Maps

- **Authors**: Dicong Qiu, Wenzong Ma, Zhenfu Pan, Hui Xiong, Junwei Liang

#### Abstract

Open-Vocabulary Mobile Manipulation (OVMM) is a crucial capability for autonomous robots, especially when faced with the challenges posed by unknown and dynamic environments. This task requires robots to explore and build a semantic understanding of their surroundings, generate feasible plans to achieve manipulation goals, adapt to environmental changes, and comprehend natural language instructions from humans. To address these challenges, we propose a novel framework that leverages the zero-shot detection and grounded recognition capabilities of pretraining visual-language models (VLMs) combined with dense 3D entity reconstruction to build 3D semantic maps. Additionally, we utilize large language models (LLMs) for spatial region abstraction and online planning, incorporating human instructions and spatial semantic context. We have built a 10-DoF mobile manipulation robotic platform JSR-1 and demonstrated in real-world robot experiments that our proposed framework can effectively capture spatial semantics and process natural language user instructions for zero-shot OVMM tasks under dynamic environment settings, with an overall navigation and task success rate of 80.95% and 73.33% over 105 episodes, and better SFT and SPL by 157.18% and 19.53% respectively compared to the baseline. Furthermore, the framework is capable of replanning towards the next most probable candidate location based on the spatial semantic context derived from the 3D semantic map when initial plans fail, keeping an average success rate of 76.67%.

[Paper Link](https://arxiv.org/abs/2406.18115)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-22_1.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### 3D-MVP: 3D Multiview Pretraining for Robotic Manipulation

- **Authors**: Shengyi Qian, Kaichun Mo, Valts Blukis, David F. Fouhey, Dieter Fox, Ankit Goyal

#### Abstract

Recent works have shown that visual pretraining on egocentric datasets using masked autoencoders (MAE) can improve generalization for downstream robotics tasks. However, these approaches pretrain only on 2D images, while many robotics applications require 3D scene understanding. In this work, we propose 3D-MVP, a novel approach for 3D multi-view pretraining using masked autoencoders. We leverage Robotic View Transformer (RVT), which uses a multi-view transformer to understand the 3D scene and predict gripper pose actions. We split RVT's multi-view transformer into visual encoder and action decoder, and pretrain its visual encoder using masked autoencoding on large-scale 3D datasets such as Objaverse. We evaluate 3D-MVP on a suite of virtual robot manipulation tasks and demonstrate improved performance over baselines. We also show promising results on a real robot platform with minimal finetuning. Our results suggest that 3D-aware pretraining is a promising approach to improve sample efficiency and generalization of vision-based robotic manipulation policies. We will release code and pretrained models for 3D-MVP to facilitate future research. Project site: this https URL

[Paper Link](https://arxiv.org/abs/2406.18158)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-22.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-25

### QuadrupedGPT: Towards a Versatile Quadruped Agent in Open-ended Worlds

- **Authors**: Ye Wang, Yuting Mei, Sipeng Zheng, Qin Jin

#### Abstract

While pets offer companionship, their limited intelligence restricts advanced reasoning and autonomous interaction with humans. Considering this, we propose QuadrupedGPT, a versatile agent designed to master a broad range of complex tasks with agility comparable to that of a pet. To achieve this goal, the primary challenges include: i) effectively leveraging multimodal observations for decision-making; ii) mastering agile control of locomotion and path planning; iii) developing advanced cognition to execute long-term objectives. QuadrupedGPT processes human command and environmental contexts using a large multimodal model (LMM). Empowered by its extensive knowledge base, our agent autonomously assigns appropriate parameters for adaptive locomotion policies and guides the agent in planning a safe but efficient path towards the goal, utilizing semantic-aware terrain analysis. Moreover, QuadrupedGPT is equipped with problem-solving capabilities that enable it to decompose long-term goals into a sequence of executable subgoals through high-level reasoning. Extensive experiments across various benchmarks confirm that QuadrupedGPT can adeptly handle multiple tasks with intricate instructions, demonstrating a significant step towards the versatile quadruped agents in open-ended worlds. Our website and codes can be found at this https URL.

[Paper Link](https://arxiv.org/abs/2406.16578)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_23-09.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-18

### RoboPoint: A Vision-Language Model for Spatial Affordance Prediction for Robotics

- **Authors**: Wentao Yuan, Jiafei Duan, Valts Blukis, Wilbert Pumacay, Ranjay Krishna, Adithyavairavan Murali, Arsalan Mousavian, Dieter Fox

#### Abstract

From rearranging objects on a table to putting groceries into shelves, robots must plan precise action points to perform tasks accurately and reliably. In spite of the recent adoption of vision language models (VLMs) to control robot behavior, VLMs struggle to precisely articulate robot actions using language. We introduce an automatic synthetic data generation pipeline that instruction-tunes VLMs to robotic domains and needs. Using the pipeline, we train RoboPoint, a VLM that predicts image keypoint affordances given language instructions. Compared to alternative approaches, our method requires no real-world data collection or human demonstration, making it much more scalable to diverse environments and viewpoints. In addition, RoboPoint is a general model that enables several downstream applications such as robot navigation, manipulation, and augmented reality (AR) assistance. Our experiments demonstrate that RoboPoint outperforms state-of-the-art VLMs (GPT-4o) and visual prompting techniques (PIVOT) by 21.8% in the accuracy of predicting spatial affordance and by 30.5% in the success rate of downstream tasks. Project website: this https URL.

[Paper Link](https://arxiv.org/abs/2406.10721)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_22-23.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Humanoid Parkour Learning

- **Authors**: Ziwen Zhuang, Shenzhe Yao, Hang Zhao

#### Abstract

Parkour is a grand challenge for legged locomotion, even for quadruped robots, requiring active perception and various maneuvers to overcome multiple challenging obstacles. Existing methods for humanoid locomotion either optimize a trajectory for a single parkour track or train a reinforcement learning policy only to walk with a significant amount of motion references. In this work, we propose a framework for learning an end-to-end vision-based whole-body-control parkour policy for humanoid robots that overcomes multiple parkour skills without any motion prior. Using the parkour policy, the humanoid robot can jump on a 0.42m platform, leap over hurdles, 0.8m gaps, and much more. It can also run at 1.8m/s in the wild and walk robustly on different terrains. We test our policy in indoor and outdoor environments to demonstrate that it can autonomously select parkour skills while following the rotation command of the joystick. We override the arm actions and show that this framework can easily transfer to humanoid mobile manipulation tasks. Videos can be found at this https URL

[Paper Link](https://arxiv.org/abs/2406.10759)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_22-21.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Imagination Policy: Using Generative Point Cloud Models for Learning Manipulation Policies

- **Authors**: Haojie Huang, Karl Schmeckpeper, Dian Wang, Ondrej Biza, Yaoyao Qian, Haotian Liu, Mingxi Jia, Robert Platt, Robin Walters

#### Abstract

Humans can imagine goal states during planning and perform actions to match those goals. In this work, we propose Imagination Policy, a novel multi-task key-frame policy network for solving high-precision pick and place tasks. Instead of learning actions directly, Imagination Policy generates point clouds to imagine desired states which are then translated to actions using rigid action estimation. This transforms action inference into a local generative task. We leverage pick and place symmetries underlying the tasks in the generation process and achieve extremely high sample efficiency and generalizability to unseen configurations. Finally, we demonstrate state-of-the-art performance across various tasks on the RLbench benchmark compared with several strong baselines.

[Paper Link](https://arxiv.org/abs/2406.11740)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_22-11.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-17

### GPT-Fabric: Folding and Smoothing Fabric by Leveraging Pre-Trained Foundation Models

- **Authors**: Vedant Raval, Enyu Zhao, Hejia Zhang, Stefanos Nikolaidis, Daniel Seita

#### Abstract

Fabric manipulation has applications in folding blankets, handling patient clothing, and protecting items with covers. It is challenging for robots to perform fabric manipulation since fabrics have infinite-dimensional configuration spaces, complex dynamics, and may be in folded or crumpled configurations with severe self-occlusions. Prior work on robotic fabric manipulation relies either on heavily engineered setups or learning-based approaches that create and train on robot-fabric interaction data. In this paper, we propose GPT-Fabric for the canonical tasks of fabric folding and smoothing, where GPT directly outputs an action informing a robot where to grasp and pull a fabric. We perform extensive experiments in simulation to test GPT-Fabric against prior state of the art methods for folding and smoothing. We obtain comparable or better performance to most methods even without explicitly training on a fabric-specific dataset (i.e., zero-shot manipulation). Furthermore, we apply GPT-Fabric in physical experiments over 12 folding and 10 smoothing rollouts. Our results suggest that GPT-Fabric is a promising approach for high-precision fabric manipulation tasks.

[Paper Link](https://arxiv.org/abs/2406.09640)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-46.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Language-Guided Manipulation with Diffusion Policies and Constrained Inpainting

- **Authors**: Ce Hao, Kelvin Lin, Siyuan Luo, Harold Soh

#### Abstract

Diffusion policies have demonstrated robust performance in generative modeling, prompting their application in robotic manipulation controlled via language descriptions. In this paper, we introduce a zero-shot, open-vocabulary diffusion policy method for robot manipulation. Using Vision-Language Models (VLMs), our method transforms linguistic task descriptions into actionable keyframes in 3D space. These keyframes serve to guide the diffusion process via inpainting. However, naively enforcing the diffusion process to adhere to the generated keyframes is problematic: the keyframes from the VLMs may be incorrect and lead to out-of-distribution (OOD) action sequences where the diffusion model performs poorly. To address these challenges, we develop an inpainting optimization strategy that balances adherence to the keyframes v.s. the training data distribution. Experimental evaluations demonstrate that our approach surpasses the performance of traditional fine-tuned language-conditioned methods in both simulated and real-world settings.

[Paper Link](https://arxiv.org/abs/2406.09767)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-44.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Sim-to-Real Transfer via 3D Feature Fields for Vision-and-Language Navigation

- **Authors**: Zihan Wang, Xiangyang Li, Jiahao Yang, Yeqi Liu, Shuqiang Jiang

#### Abstract

Vision-and-language navigation (VLN) enables the agent to navigate to a remote location in 3D environments following the natural language instruction. In this field, the agent is usually trained and evaluated in the navigation simulators, lacking effective approaches for sim-to-real transfer. The VLN agents with only a monocular camera exhibit extremely limited performance, while the mainstream VLN models trained with panoramic observation, perform better but are difficult to deploy on most monocular robots. For this case, we propose a sim-to-real transfer approach to endow the monocular robots with panoramic traversability perception and panoramic semantic understanding, thus smoothly transferring the high-performance panoramic VLN models to the common monocular robots. In this work, the semantic traversable map is proposed to predict agent-centric navigable waypoints, and the novel view representations of these navigable waypoints are predicted through the 3D feature fields. These methods broaden the limited field of view of the monocular robots and significantly improve navigation performance in the real world. Our VLN system outperforms previous SOTA monocular VLN methods in R2R-CE and RxR-CE benchmarks within the simulation environments and is also validated in real-world environments, providing a practical and high-performance solution for real-world VLN.

[Paper Link](https://arxiv.org/abs/2406.09798)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-34.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-14

### MMScan: A Multi-Modal 3D Scene Dataset with Hierarchical Grounded Language Annotations

- **Authors**: Ruiyuan Lyu, Tai Wang, Jingli Lin, Shuai Yang, Xiaohan Mao, Yilun Chen, Runsen Xu, Haifeng Huang, Chenming Zhu, Dahua Lin, Jiangmiao Pang

#### Abstract

With the emergence of LLMs and their integration with other data modalities, multi-modal 3D perception attracts more attention due to its connectivity to the physical world and makes rapid progress. However, limited by existing datasets, previous works mainly focus on understanding object properties or inter-object spatial relationships in a 3D scene. To tackle this problem, this paper builds the first largest ever multi-modal 3D scene dataset and benchmark with hierarchical grounded language annotations, MMScan. It is constructed based on a top-down logic, from region to object level, from a single target to inter-target relationships, covering holistic aspects of spatial and attribute understanding. The overall pipeline incorporates powerful VLMs via carefully designed prompts to initialize the annotations efficiently and further involve humans' correction in the loop to ensure the annotations are natural, correct, and comprehensive. Built upon existing 3D scanning data, the resulting multi-modal 3D dataset encompasses 1.4M meta-annotated captions on 109k objects and 7.7k regions as well as over 3.04M diverse samples for 3D visual grounding and question-answering benchmarks. We evaluate representative baselines on our benchmarks, analyze their capabilities in different aspects, and showcase the key problems to be addressed in the future. Furthermore, we use this high-quality dataset to train state-of-the-art 3D visual grounding and LLMs and obtain remarkable performance improvement both on existing benchmarks and in-the-wild evaluation. Codes, datasets, and benchmarks will be available at this https URL.

[Paper Link](https://arxiv.org/abs/2406.09401)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-21.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### RVT-2: Learning Precise Manipulation from Few Demonstrations

- **Authors**: Ankit Goyal, Valts Blukis, Jie Xu, Yijie Guo, Yu-Wei Chao, Dieter Fox

#### Abstract

In this work, we study how to build a robotic system that can solve multiple 3D manipulation tasks given language instructions. To be useful in industrial and household domains, such a system should be capable of learning new tasks with few demonstrations and solving them precisely. Prior works, like PerAct and RVT, have studied this problem, however, they often struggle with tasks requiring high precision. We study how to make them more effective, precise, and fast. Using a combination of architectural and system-level improvements, we propose RVT-2, a multitask 3D manipulation model that is 6X faster in training and 2X faster in inference than its predecessor RVT. RVT-2 achieves a new state-of-the-art on RLBench, improving the success rate from 65% to 82%. RVT-2 is also effective in the real world, where it can learn tasks requiring high precision, like picking up and inserting plugs, with just 10 demonstrations. Visual results, code, and trained model are provided at: this https URL.

[Paper Link](https://arxiv.org/abs/2406.08545)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-20.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### LLM-Craft: Robotic Crafting of Elasto-Plastic Objects with Large Language Models

- **Authors**: Alison Bartsch, Amir Barati Farimani

#### Abstract

When humans create sculptures, we are able to reason about how geometrically we need to alter the clay state to reach our target goal. We are not computing point-wise similarity metrics, or reasoning about low-level positioning of our tools, but instead determining the higher-level changes that need to be made. In this work, we propose LLM-Craft, a novel pipeline that leverages large language models (LLMs) to iteratively reason about and generate deformation-based crafting action sequences. We simplify and couple the state and action representations to further encourage shape-based reasoning. To the best of our knowledge, LLM-Craft is the first system successfully leveraging LLMs for complex deformable object interactions. Through our experiments, we demonstrate that with the LLM-Craft framework, LLMs are able to successfully reason about the deformation behavior of elasto-plastic objects. Furthermore, we find that LLM-Craft is able to successfully create a set of simple letter shapes. Finally, we explore extending the framework to reaching more ambiguous semantic goals, such as "thinner" or "bumpy". For videos please see our website: this https URL.

[Paper Link](https://arxiv.org/abs/2406.08648)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-19.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### LLM-Driven Robots Risk Enacting Discrimination, Violence, and Unlawful Actions

- **Authors**: Rumaisa Azeem, Andrew Hundt, Masoumeh Mansouri, Martim Brandão

#### Abstract

Members of the Human-Robot Interaction (HRI) and Artificial Intelligence (AI) communities have proposed Large Language Models (LLMs) as a promising resource for robotics tasks such as natural language interactions, doing household and workplace tasks, approximating `common sense reasoning', and modeling humans. However, recent research has raised concerns about the potential for LLMs to produce discriminatory outcomes and unsafe behaviors in real-world robot experiments and applications. To address these concerns, we conduct an HRI-based evaluation of discrimination and safety criteria on several highly-rated LLMs. Our evaluation reveals that LLMs currently lack robustness when encountering people across a diverse range of protected identity characteristics (e.g., race, gender, disability status, nationality, religion, and their intersections), producing biased outputs consistent with directly discriminatory outcomes -- e.g. `gypsy' and `mute' people are labeled untrustworthy, but not `european' or `able-bodied' people. Furthermore, we test models in settings with unconstrained natural language (open vocabulary) inputs, and find they fail to act safely, generating responses that accept dangerous, violent, or unlawful instructions -- such as incident-causing misstatements, taking people's mobility aids, and sexual predation. Our results underscore the urgent need for systematic, routine, and comprehensive risk assessments and assurances to improve outcomes and ensure LLMs only operate on robots when it is safe, effective, and just to do so. Data and code will be made available.

[Paper Link](https://arxiv.org/abs/2406.08824)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-16.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### OmniH2O: Universal and Dexterous Human-to-Humanoid Whole-Body Teleoperation and Learning

- **Authors**: Tairan He, Zhengyi Luo, Xialin He, Wenli Xiao, Chong Zhang, Weinan Zhang, Kris Kitani, Changliu Liu, Guanya Shi

#### Abstract

We present OmniH2O (Omni Human-to-Humanoid), a learning-based system for whole-body humanoid teleoperation and autonomy. Using kinematic pose as a universal control interface, OmniH2O enables various ways for a human to control a full-sized humanoid with dexterous hands, including using real-time teleoperation through VR headset, verbal instruction, and RGB camera. OmniH2O also enables full autonomy by learning from teleoperated demonstrations or integrating with frontier models such as GPT-4. OmniH2O demonstrates versatility and dexterity in various real-world whole-body tasks through teleoperation or autonomy, such as playing multiple sports, moving and manipulating objects, and interacting with humans. We develop an RL-based sim-to-real pipeline, which involves large-scale retargeting and augmentation of human motion datasets, learning a real-world deployable policy with sparse sensor input by imitating a privileged teacher policy, and reward designs to enhance robustness and stability. We release the first humanoid whole-body control dataset, OmniH2O-6, containing six everyday tasks, and demonstrate humanoid whole-body skill learning from teleoperated datasets.

[Paper Link](https://arxiv.org/abs/2406.08858)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-15.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### OpenVLA: An Open-Source Vision-Language-Action Model

- **Authors**: Moo Jin Kim, Karl Pertsch, Siddharth Karamcheti, Ted Xiao, Ashwin Balakrishna, Suraj Nair, Rafael Rafailov, Ethan Foster, Grace Lam, Pannag Sanketi, Quan Vuong, Thomas Kollar, Benjamin Burchfiel, Russ Tedrake, Dorsa Sadigh, Sergey Levine, Percy Liang, Chelsea Finn

#### Abstract

Large policies pretrained on a combination of Internet-scale vision-language data and diverse robot demonstrations have the potential to change how we teach robots new skills: rather than training new behaviors from scratch, we can fine-tune such vision-language-action (VLA) models to obtain robust, generalizable policies for visuomotor control. Yet, widespread adoption of VLAs for robotics has been challenging as 1) existing VLAs are largely closed and inaccessible to the public, and 2) prior work fails to explore methods for efficiently fine-tuning VLAs for new tasks, a key component for adoption. Addressing these challenges, we introduce OpenVLA, a 7B-parameter open-source VLA trained on a diverse collection of 970k real-world robot demonstrations. OpenVLA builds on a Llama 2 language model combined with a visual encoder that fuses pretrained features from DINOv2 and SigLIP. As a product of the added data diversity and new model components, OpenVLA demonstrates strong results for generalist manipulation, outperforming closed models such as RT-2-X (55B) by 16.5% in absolute task success rate across 29 tasks and multiple robot embodiments, with 7x fewer parameters. We further show that we can effectively fine-tune OpenVLA for new settings, with especially strong generalization results in multi-task environments involving multiple objects and strong language grounding abilities, and outperform expressive from-scratch imitation learning methods such as Diffusion Policy by 20.4%. We also explore compute efficiency; as a separate contribution, we show that OpenVLA can be fine-tuned on consumer GPUs via modern low-rank adaptation methods and served efficiently via quantization without a hit to downstream success rate. Finally, we release model checkpoints, fine-tuning notebooks, and our PyTorch codebase with built-in support for training VLAs at scale on Open X-Embodiment datasets.

[Paper Link](https://arxiv.org/abs/2406.09246)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-07-06_21-03.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-12

### BAKU: An Efficient Transformer for Multi-Task Policy Learning

- **Authors**: Siddhant Haldar, Zhuoran Peng, Lerrel Pinto
- **Main Affiliations**: New York University
- **Tags**: `Policy Learning`

#### Abstract

Training generalist agents capable of solving diverse tasks is challenging, often requiring large datasets of expert demonstrations. This is particularly problematic in robotics, where each data point requires physical execution of actions in the real world. Thus, there is a pressing need for architectures that can effectively leverage the available training data. In this work, we present BAKU, a simple transformer architecture that enables efficient learning of multi-task robot policies. BAKU builds upon recent advancements in offline imitation learning and meticulously combines observation trunks, action chunking, multi-sensory observations, and action heads to substantially improve upon prior work. Our experiments on 129 simulated tasks across LIBERO, Meta-World suite, and the Deepmind Control suite exhibit an overall 18% absolute improvement over RT-1 and MT-ACT, with a 36% improvement on the harder LIBERO benchmark. On 30 real-world manipulation tasks, given an average of just 17 demonstrations per task, BAKU achieves a 91% success rate. Videos of the robot are best viewed at this https URL.

[Paper Link](https://arxiv.org/abs/2406.07539)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-47.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### A3VLM: Actionable Articulation-Aware Vision Language Model

- **Authors**: Siyuan Huang, Haonan Chang, Yuhan Liu, Yimeng Zhu, Hao Dong, Peng Gao, Abdeslam Boularias, Hongsheng Li
- **Main Affiliations**: SJTU, Shanghai AI Lab, Rutgers University, Yuandao AI, PKU, CUHK MMLab
- **Tags**: `LLM`

#### Abstract

Vision Language Models (VLMs) have received significant attention in recent years in the robotics community. VLMs are shown to be able to perform complex visual reasoning and scene understanding tasks, which makes them regarded as a potential universal solution for general robotics problems such as manipulation and navigation. However, previous VLMs for robotics such as RT-1, RT-2, and ManipLLM~ have focused on directly learning robot-centric actions. Such approaches require collecting a significant amount of robot interaction data, which is extremely costly in the real world. Thus, we propose A3VLM, an object-centric, actionable, articulation-aware vision language model. A3VLM focuses on the articulation structure and action affordances of objects. Its representation is robot-agnostic and can be translated into robot actions using simple action primitives. Extensive experiments in both simulation benchmarks and real-world settings demonstrate the effectiveness and stability of A3VLM. We release our code and other materials at this https URL.

[Paper Link](https://arxiv.org/abs/2406.07549)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-45.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-11

### Demonstrating HumanTHOR: A Simulation Platform and Benchmark for Human-Robot Collaboration in a Shared Workspace

- **Authors**: Chenxu Wang, Boyuan Du, Jiaxin Xu, Peiyan Li, Di Guo, Huaping Liu
- **Main Affiliations**: Tsinghua University
- **Tags**: `Simulation`

#### Abstract

Human-robot collaboration (HRC) in a shared workspace has become a common pattern in real-world robot applications and has garnered significant research interest. However, most existing studies for human-in-the-loop (HITL) collaboration with robots in a shared workspace evaluate in either simplified game environments or physical platforms, falling short in limited realistic significance or limited scalability. To support future studies, we build an embodied framework named HumanTHOR, which enables humans to act in the simulation environment through VR devices to support HITL collaborations in a shared workspace. To validate our system, we build a benchmark of everyday tasks and conduct a preliminary user study with two baseline algorithms. The results show that the robot can effectively assist humans in collaboration, demonstrating the significance of HRC. The comparison among different levels of baselines affirms that our system can adequately evaluate robot capabilities and serve as a benchmark for different robot algorithms. The experimental results also indicate that there is still much room in the area and our system can provide a preliminary foundation for future HRC research in a shared workspace. More information about the simulation environment, experiment videos, benchmark descriptions, and additional supplementary materials can be found on the website: this https URL.

[Paper Link](https://arxiv.org/abs/2406.06498)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-41.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-5

### DrEureka: Language Model Guided Sim-To-Real Transfer

- **Authors**: Yecheng Jason Ma, William Liang, Hung-Ju Wang, Sam Wang, Yuke Zhu, Linxi Fan, Osbert Bastani, Dinesh Jayaraman
- **Main Affiliations**: University of Pennsylvania, NVIDIA, University of Texas, Austin
- **Tags**: `Simulation`

#### Abstract

Transferring policies learned in simulation to the real world is a promising strategy for acquiring robot skills at scale. However, sim-to-real approaches typically rely on manual design and tuning of the task reward function as well as the simulation physics parameters, rendering the process slow and human-labor intensive. In this paper, we investigate using Large Language Models (LLMs) to automate and accelerate sim-to-real design. Our LLM-guided sim-to-real approach, DrEureka, requires only the physics simulation for the target task and automatically constructs suitable reward functions and domain randomization distributions to support real-world transfer. We first demonstrate that our approach can discover sim-to-real configurations that are competitive with existing human-designed ones on quadruped locomotion and dexterous manipulation tasks. Then, we showcase that our approach is capable of solving novel robot tasks, such as quadruped balancing and walking atop a yoga ball, without iterative manual design.

[Paper Link](https://arxiv.org/abs/2406.01967)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-27.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Query-based Semantic Gaussian Field for Scene Representation in Reinforcement Learning

- **Authors**: Jiaxu Wang, Ziyi Zhang, Qiang Zhang, Jia Li, Jingkai Sun, Mingyuan Sun, Junhao He, Renjing Xu
- **Main Affiliations**: HKUST (GZ), HKU, NEU
- **Tags**: `RL, 3DGS`

#### Abstract

Latent scene representation plays a significant role in training reinforcement learning (RL) agents. To obtain good latent vectors describing the scenes, recent works incorporate the 3D-aware latent-conditioned NeRF pipeline into scene representation learning. However, these NeRF-related methods struggle to perceive 3D structural information due to the inefficient dense sampling in volumetric rendering. Moreover, they lack fine-grained semantic information included in their scene representation vectors because they evenly consider free and occupied spaces. Both of them can destroy the performance of downstream RL tasks. To address the above challenges, we propose a novel framework that adopts the efficient 3D Gaussian Splatting (3DGS) to learn 3D scene representation for the first time. In brief, we present the Query-based Generalizable 3DGS to bridge the 3DGS technique and scene representations with more geometrical awareness than those in NeRFs. Moreover, we present the Hierarchical Semantics Encoding to ground the fine-grained semantic features to 3D Gaussians and further distilled to the scene representation vectors. We conduct extensive experiments on two RL platforms including Maniskill2 and Robomimic across 10 different tasks. The results show that our method outperforms the other 5 baselines by a large margin. We achieve the best success rates on 8 tasks and the second-best on the other two tasks.

[Paper Link](https://arxiv.org/abs/2406.02370)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-22.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### RoboCasa: Large-Scale Simulation of Everyday Tasks for Generalist Robots

- **Authors**: Soroush Nasiriany, Abhiram Maddukuri, Lance Zhang, Adeet Parikh, Aaron Lo, Abhishek Joshi, Ajay Mandlekar, Yuke Zhu
- **Main Affiliations**: The University of Texas at Austin, NVIDIA Research
- **Tags**: `Simulation`

#### Abstract

Recent advancements in Artificial Intelligence (AI) have largely been propelled by scaling. In Robotics, scaling is hindered by the lack of access to massive robot datasets. We advocate using realistic physical simulation as a means to scale environments, tasks, and datasets for robot learning methods. We present RoboCasa, a large-scale simulation framework for training generalist robots in everyday environments. RoboCasa features realistic and diverse scenes focusing on kitchen environments. We provide thousands of 3D assets across over 150 object categories and dozens of interactable furniture and appliances. We enrich the realism and diversity of our simulation with generative AI tools, such as object assets from text-to-3D models and environment textures from text-to-image models. We design a set of 100 tasks for systematic evaluation, including composite tasks generated by the guidance of large language models. To facilitate learning, we provide high-quality human demonstrations and integrate automated trajectory generation methods to substantially enlarge our datasets with minimal human burden. Our experiments show a clear scaling trend in using synthetically generated robot data for large-scale imitation learning and show great promise in harnessing simulation data in real-world tasks. Videos and open-source code are available at this https URL

[Paper Link](https://arxiv.org/abs/2406.02523)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-19.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-06-4

### PDP: Physics-Based Character Animation via Diffusion Policy

- **Authors**: Takara E. Truong, Michael Piseno, Zhaoming Xie, C. Karen Liu
- **Main Affiliations**: Stanford University
- **Tags**: `Diffusion Policy`

#### Abstract

Generating diverse and realistic human motion that can physically interact with an environment remains a challenging research area in character animation. Meanwhile, diffusion-based methods, as proposed by the robotics community, have demonstrated the ability to capture highly diverse and multi-modal skills. However, naively training a diffusion policy often results in unstable motions for high-frequency, under-actuated control tasks like bipedal locomotion due to rapidly accumulating compounding errors, pushing the agent away from optimal training trajectories. The key idea lies in using RL policies not just for providing optimal trajectories but for providing corrective actions in sub-optimal states, giving the policy a chance to correct for errors caused by environmental stimulus, model errors, or numerical errors in simulation. Our method, Physics-Based Character Animation via Diffusion Policy (PDP), combines reinforcement learning (RL) and behavior cloning (BC) to create a robust diffusion policy for physics-based character animation. We demonstrate PDP on perturbation recovery, universal motion tracking, and physics-based text-to-motion synthesis.

[Paper Link](https://arxiv.org/abs/2406.00960)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-15.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Learning Manipulation by Predicting Interaction

- **Authors**: Jia Zeng, Qingwen Bu, Bangjun Wang, Wenke Xia, Li Chen, Hao Dong, Haoming Song, Dong Wang, Di Hu, Ping Luo, Heming Cui, Bin Zhao, Xuelong Li, Yu Qiao, Hongyang Li
- **Main Affiliations**: Shanghai AI Lab, Shanghai Jiao Tong University, Renmin University of China, Peking University, Northwestern Polytechnical University, TeleAI, China Telecom Corp Ltd
- **Tags**: `Manipulation`

#### Abstract

Representation learning approaches for robotic manipulation have boomed in recent years. Due to the scarcity of in-domain robot data, prevailing methodologies tend to leverage large-scale human video datasets to extract generalizable features for visuomotor policy learning. Despite the progress achieved, prior endeavors disregard the interactive dynamics that capture behavior patterns and physical interaction during the manipulation process, resulting in an inadequate understanding of the relationship between objects and the environment. To this end, we propose a general pre-training pipeline that learns Manipulation by Predicting the Interaction (MPI) and enhances the visual representation.Given a pair of keyframes representing the initial and final states, along with language instructions, our algorithm predicts the transition frame and detects the interaction object, respectively. These two learning objectives achieve superior comprehension towards "how-to-interact" and "where-to-interact". We conduct a comprehensive evaluation of several challenging robotic tasks.The experimental results demonstrate that MPI exhibits remarkable improvement by 10% to 64% compared with previous state-of-the-art in real-world robot platforms as well as simulation environments. Code and checkpoints are publicly shared at this https URL.

[Paper Link](https://arxiv.org/abs/2406.00439)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-07.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Unsupervised Neural Motion Retargeting for Humanoid Teleoperation

- **Authors**: Satoshi Yagi, Mitsunori Tada, Eiji Uchibe, Suguru Kanoga, Takamitsu Matsubara, Jun Morimoto
- **Main Affiliations**: Kyoto University, National Institute of Advanced Industrial Science and Technology (AIST), Advanced Telecommunications Research Institute International (ATR), Graduate School of Science Technology, Nara Institute of Science and Technology
- **Tags**: `Humanoid`

#### Abstract

This study proposes an approach to human-to-humanoid teleoperation using GAN-based online motion retargeting, which obviates the need for the construction of pairwise datasets to identify the relationship between the human and the humanoid kinematics. Consequently, it can be anticipated that our proposed teleoperation system will reduce the complexity and setup requirements typically associated with humanoid controllers, thereby facilitating the development of more accessible and intuitive teleoperation systems for users without robotics knowledge. The experiments demonstrated the efficacy of the proposed method in retargeting a range of upper-body human motions to humanoid, including a body jab motion and a basketball shoot motion. Moreover, the human-in-the-loop teleoperation performance was evaluated by measuring the end-effector position errors between the human and the retargeted humanoid motions. The results demonstrated that the error was comparable to those of conventional motion retargeting methods that require pairwise motion datasets. Finally, a box pick-and-place task was conducted to demonstrate the usability of the developed humanoid teleoperation system.

[Paper Link](https://arxiv.org/abs/2406.00727)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_23-01.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Learning-based legged locomotion; state of the art and future perspectives

- **Authors**: Sehoon Ha, Joonho Lee, Michiel van de Panne, Zhaoming Xie, Wenhao Yu, Majid Khadiv
- **Main Affiliations**: Georgia Institute of Technology, Neuromeka, University of British Columbia, The AI Institute, 5Google DeepMind, Technical University of Munich
- **Tags**: `Locomotion`

#### Abstract

Legged locomotion holds the premise of universal mobility, a critical capability for many real-world robotic applications. Both model-based and learning-based approaches have advanced the field of legged locomotion in the past three decades. In recent years, however, a number of factors have dramatically accelerated progress in learning-based methods, including the rise of deep learning, rapid progress in simulating robotic systems, and the availability of high-performance and affordable hardware. This article aims to give a brief history of the field, to summarize recent efforts in learning locomotion skills for quadrupeds, and to provide researchers new to the area with an understanding of the key issues involved. With the recent proliferation of humanoid robots, we further outline the rapid rise of analogous methods for bipedal locomotion. We conclude with a discussion of open problems as well as related societal impact.

[Paper Link](https://arxiv.org/abs/2406.01152)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_22-53.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### ManiCM: Real-time 3D Diffusion Policy via Consistency Model for Robotic Manipulation

- **Authors**: Guanxing Lu, Zifeng Gao, Tianxing Chen, Wenxun Dai, Ziwei Wang, Yansong Tang
- **Main Affiliations**: Tsinghua University, Shanghai AI Laboratory, Carnegie Mellon University
- **Tags**: `Diffusion Policy, Consistency Model`

#### Abstract

Diffusion models have been verified to be effective in generating complex distributions from natural images to motion trajectories. Recent diffusion-based methods show impressive performance in 3D robotic manipulation tasks, whereas they suffer from severe runtime inefficiency due to multiple denoising steps, especially with high-dimensional observations. To this end, we propose a real-time robotic manipulation model named ManiCM that imposes the consistency constraint to the diffusion process, so that the model can generate robot actions in only one-step inference. Specifically, we formulate a consistent diffusion process in the robot action space conditioned on the point cloud input, where the original action is required to be directly denoised from any point along the ODE trajectory. To model this process, we design a consistency distillation technique to predict the action sample directly instead of predicting the noise within the vision community for fast convergence in the low-dimensional action manifold. We evaluate ManiCM on 31 robotic manipulation tasks from Adroit and Metaworld, and the results demonstrate that our approach accelerates the state-of-the-art method by 10 times in average inference speed while maintaining competitive average success rate.

[Paper Link](https://arxiv.org/abs/2406.01586)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-12_22-46.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-30

### Grasp as You Say: Language-guided Dexterous Grasp Generation

- **Authors**: Yi-Lin Wei, Jian-Jian Jiang, Chengyi Xing, Xiantuo Tan, Xiao-Ming Wu, Hao Li, Mark Cutkosky, Wei-Shi Zheng
- **Main Affiliations**: Sun Yat-sen University, Stanford University, Wuhan University
- **Tags**: `Simulation`

#### Abstract

This paper explores a novel task ""Dexterous Grasp as You Say"" (DexGYS), enabling robots to perform dexterous grasping based on human commands expressed in natural language. However, the development of this field is hindered by the lack of datasets with natural human guidance; thus, we propose a language-guided dexterous grasp dataset, named DexGYSNet, offering high-quality dexterous grasp annotations along with flexible and fine-grained human language guidance. Our dataset construction is cost-efficient, with the carefully-design hand-object interaction retargeting strategy, and the LLM-assisted language guidance annotation system. Equipped with this dataset, we introduce the DexGYSGrasp framework for generating dexterous grasps based on human language instructions, with the capability of producing grasps that are intent-aligned, high quality and diversity. To achieve this capability, our framework decomposes the complex learning process into two manageable progressive objectives and introduce two components to realize them. The first component learns the grasp distribution focusing on intention alignment and generation diversity. And the second component refines the grasp quality while maintaining intention consistency. Extensive experiments are conducted on DexGYSNet and real world environment for validation.

[Paper Link](https://arxiv.org/abs/2405.19291)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-06-01_18-02.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-21

### URDFormer: A Pipeline for Constructing Articulated Simulation Environments from Real-World Images

- **Authors**: Zoey Chen, Aaron Walsman, Marius Memmel, Kaichun Mo, Alex Fang, Karthikeya Vemuri, Alan Wu, Dieter Fox, Abhishek Gupta
- **Main Affiliations**: University of Washington, Nvidia
- **Tags**: `Simulation`

#### Abstract

Constructing simulation scenes that are both visually and physically realistic is a problem of practical interest in domains ranging from robotics to computer vision. This problem has become even more relevant as researchers wielding large data-hungry learning methods seek new sources of training data for physical decision-making systems. However, building simulation models is often still done by hand. A graphic designer and a simulation engineer work with predefined assets to construct rich scenes with realistic dynamic and kinematic properties. While this may scale to small numbers of scenes, to achieve the generalization properties that are required for data-driven robotic control, we require a pipeline that is able to synthesize large numbers of realistic scenes, complete with 'natural' kinematic and dynamic structures. To attack this problem, we develop models for inferring structure and generating simulation scenes from natural images, allowing for scalable scene generation from web-scale datasets. To train these image-to-simulation models, we show how controllable text-to-image generative models can be used in generating paired training data that allows for modeling of the inverse problem, mapping from realistic images back to complete scene models. We show how this paradigm allows us to build large datasets of scenes in simulation with semantic and physical realism. We present an integrated end-to-end pipeline that generates simulation scenes complete with articulated kinematic and dynamic structures from real-world images and use these for training robotic control policies. We then robustly deploy in the real world for tasks like articulated object manipulation. In doing so, our work provides both a pipeline for large-scale generation of simulation environments and an integrated system for training robust robotic control policies in the resulting environments.

[Paper Link](https://arxiv.org/abs/2405.11656)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-21_22-43.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Octo: An Open-Source Generalist Robot Policy

- **Authors**: Octo Model Team, Dibya Ghosh, Homer Walke, Karl Pertsch, Kevin Black, Oier Mees, Sudeep Dasari, Joey Hejna, Tobias Kreiman, Charles Xu, Jianlan Luo, You Liang Tan, Pannag Sanketi, Quan Vuong, Ted Xiao, Dorsa Sadigh, Chelsea Finn, Sergey Levine
- **Main Affiliations**: University of California, Berkeley, Carnegie Mellon University, Google DeepMind
- **Tags**: `large policy`

#### Abstract

Large policies pretrained on diverse robot datasets have the potential to transform robotic learning: instead of training new policies from scratch, such generalist robot policies may be finetuned with only a little in-domain data, yet generalize broadly. However, to be widely applicable across a range of robotic learning scenarios, environments, and tasks, such policies need to handle diverse sensors and action spaces, accommodate a variety of commonly used robotic platforms, and finetune readily and efficiently to new domains. In this work, we aim to lay the groundwork for developing open-source, widely applicable, generalist policies for robotic manipulation. As a first step, we introduce Octo, a large transformer-based policy trained on 800k trajectories from the Open X-Embodiment dataset, the largest robot manipulation dataset to date. It can be instructed via language commands or goal images and can be effectively finetuned to robot setups with new sensory inputs and action spaces within a few hours on standard consumer GPUs. In experiments across 9 robotic platforms, we demonstrate that Octo serves as a versatile policy initialization that can be effectively finetuned to new observation and action spaces. We also perform detailed ablations of design decisions for the Octo model, from architecture to training data, to guide future research on building generalist robot models.

[Paper Link](https://arxiv.org/abs/2405.12213)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-21_21-57.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-17

### Natural Language Can Help Bridge the Sim2Real Gap

- **Authors**: Albert Yu, Adeline Foote, Raymond Mooney, Roberto Martín-Martín
- **Main Affiliations**: University of Texas at Austin
- **Tags**: `Simulation to Reality`

#### Abstract

The main challenge in learning image-conditioned robotic policies is acquiring a visual representation conducive to low-level control. Due to the high dimensionality of the image space, learning a good visual representation requires a considerable amount of visual data. However, when learning in the real world, data is expensive. Sim2Real is a promising paradigm for overcoming data scarcity in the real-world target domain by using a simulator to collect large amounts of cheap data closely related to the target task. However, it is difficult to transfer an image-conditioned policy from sim to real when the domains are very visually dissimilar. To bridge the sim2real visual gap, we propose using natural language descriptions of images as a unifying signal across domains that captures the underlying task-relevant semantics. Our key insight is that if two image observations from different domains are labeled with similar language, the policy should predict similar action distributions for both images. We demonstrate that training the image encoder to predict the language description or the distance between descriptions of a sim or real image serves as a useful, data-efficient pretraining step that helps learn a domain-invariant image representation. We can then use this image encoder as the backbone of an IL policy trained simultaneously on a large amount of simulated and a handful of real demonstrations. Our approach outperforms widely used prior sim2real methods and strong vision-language pretraining baselines like CLIP and R3M by 25 to 40%.

[Paper Link](https://arxiv.org/abs/2405.10020)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_22-04.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-14

### Scene Action Maps: Behavioural Maps for Navigation without Metric Information

- **Authors**: Joel Loo, David Hsu
- **Main Affiliations**: National University of Singapore
- **Tags**: `Navigation`

#### Abstract

Humans are remarkable in their ability to navigate without metric information. We can read abstract 2D maps, such as floor-plans or hand-drawn sketches, and use them to navigate in unseen rich 3D environments, without requiring prior traversals to map out these scenes in detail. We posit that this is enabled by the ability to represent the environment abstractly as interconnected navigational behaviours, e.g., "follow the corridor" or "turn right", while avoiding detailed, accurate spatial information at the metric level. We introduce the Scene Action Map (SAM), a behavioural topological graph, and propose a learnable map-reading method, which parses a variety of 2D maps into SAMs. Map-reading extracts salient information about navigational behaviours from the overlooked wealth of pre-existing, abstract and inaccurate maps, ranging from floor-plans to sketches. We evaluate the performance of SAMs for navigation, by building and deploying a behavioural navigation stack on a quadrupedal robot. Videos and more information is available at: this https URL.

[Paper Link](https://arxiv.org/abs/2405.07948)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_17-52.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### SPIN: Simultaneous Perception, Interaction and Navigation

- **Authors**: Shagun Uppal, Ananye Agarwal, Haoyu Xiong, Kenneth Shaw, Deepak Pathak
- **Main Affiliations**: Carnegie Mellon University
- **Tags**: `whole body navigation`

#### Abstract

While there has been remarkable progress recently in the fields of manipulation and locomotion, mobile manipulation remains a long-standing challenge. Compared to locomotion or static manipulation, a mobile system must make a diverse range of long-horizon tasks feasible in unstructured and dynamic environments. While the applications are broad and interesting, there are a plethora of challenges in developing these systems such as coordination between the base and arm, reliance on onboard perception for perceiving and interacting with the environment, and most importantly, simultaneously integrating all these parts together. Prior works approach the problem using disentangled modular skills for mobility and manipulation that are trivially tied together. This causes several limitations such as compounding errors, delays in decision-making, and no whole-body coordination. In this work, we present a reactive mobile manipulation framework that uses an active visual system to consciously perceive and react to its environment. Similar to how humans leverage whole-body and hand-eye coordination, we develop a mobile manipulator that exploits its ability to move and see, more specifically -- to move in order to see and to see in order to move. This allows it to not only move around and interact with its environment but also, choose "when" to perceive "what" using an active visual system. We observe that such an agent learns to navigate around complex cluttered scenarios while displaying agile whole-body coordination using only ego-vision without needing to create environment maps. Results visualizations and videos at this https URL

[Paper Link](https://arxiv.org/abs/2405.07991)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_17-36.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-10

### ASGrasp: Generalizable Transparent Object Reconstruction and Grasping from RGB-D Active Stereo Camera

- **Authors**: Jun Shi, Yong A, Yixiang Jin, Dingzhe Li, Haoyu Niu, Zhezhu Jin, He Wang
- **Main Affiliations**: Samsung R&D Institute China-Beijing, Peking University, Galbot, BAAI
- **Tags**: `Large Language Models`

#### Abstract

In this paper, we tackle the problem of grasping transparent and specular objects. This issue holds importance, yet it remains unsolved within the field of robotics due to failure of recover their accurate geometry by depth cameras. For the first time, we propose ASGrasp, a 6-DoF grasp detection network that uses an RGB-D active stereo camera. ASGrasp utilizes a two-layer learning-based stereo network for the purpose of transparent object reconstruction, enabling material-agnostic object grasping in cluttered environments. In contrast to existing RGB-D based grasp detection methods, which heavily depend on depth restoration networks and the quality of depth maps generated by depth cameras, our system distinguishes itself by its ability to directly utilize raw IR and RGB images for transparent object geometry reconstruction. We create an extensive synthetic dataset through domain randomization, which is based on GraspNet-1Billion. Our experiments demonstrate that ASGrasp can achieve over 90% success rate for generalizable transparent object grasping in both simulation and the real via seamless sim-to-real transfer. Our method significantly outperforms SOTA networks and even surpasses the performance upper bound set by perfect visible point cloud inputs.Project page: this https URL

[Paper Link](https://arxiv.org/abs/2405.05648)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_16-05.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### RoboHop: Segment-based Topological Map Representation for Open-World Visual Navigation

- **Authors**: Sourav Garg, Krishan Rana, Mehdi Hosseinzadeh, Lachlan Mares, Niko Sünderhauf, Feras Dayoub, Ian Reid
- **Main Affiliations**: The University of Adelaide
- **Tags**: `Large Language Models`

#### Abstract

Mapping is crucial for spatial reasoning, planning and robot navigation. Existing approaches range from metric, which require precise geometry-based optimization, to purely topological, where image-as-node based graphs lack explicit object-level reasoning and interconnectivity. In this paper, we propose a novel topological representation of an environment based on "image segments", which are semantically meaningful and open-vocabulary queryable, conferring several advantages over previous works based on pixel-level features. Unlike 3D scene graphs, we create a purely topological graph with segments as nodes, where edges are formed by a) associating segment-level descriptors between pairs of consecutive images and b) connecting neighboring segments within an image using their pixel centroids. This unveils a "continuous sense of a place", defined by inter-image persistence of segments along with their intra-image neighbours. It further enables us to represent and update segment-level descriptors through neighborhood aggregation using graph convolution layers, which improves robot localization based on segment-level retrieval. Using real-world data, we show how our proposed map representation can be used to i) generate navigation plans in the form of "hops over segments" and ii) search for target objects using natural language queries describing spatial relations of objects. Furthermore, we quantitatively analyze data association at the segment level, which underpins inter-image connectivity during mapping and segment-level localization when revisiting the same place. Finally, we show preliminary trials on segment-level `hopping' based zero-shot real-world navigation. Project page with supplementary details: this http URL

[Paper Link](https://arxiv.org/abs/2405.05792)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_16-02.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Robots Can Feel: LLM-based Framework for Robot Ethical Reasoning

- **Authors**: Artem Lykov, Miguel Altamirano Cabrera, Koffivi Fidèle Gbagbe, Dzmitry Tsetserukou
- **Main Affiliations**: Intelligent Space Robotics Laboratory, Center for Digital Engineering, Skolkovo Institute of Science and Technology, Moscow, Russia
- **Tags**: `Large Language Models`

#### Abstract

This paper presents the development of a novel ethical reasoning framework for robots. "Robots Can Feel" is the first system for robots that utilizes a combination of logic and human-like emotion simulation to make decisions in morally complex situations akin to humans. The key feature of the approach is the management of the Emotion Weight Coefficient - a customizable parameter to assign the role of emotions in robot decision-making. The system aims to serve as a tool that can equip robots of any form and purpose with ethical behavior close to human standards. Besides the platform, the system is independent of the choice of the base model. During the evaluation, the system was tested on 8 top up-to-date LLMs (Large Language Models). This list included both commercial and open-source models developed by various companies and countries. The research demonstrated that regardless of the model choice, the Emotions Weight Coefficient influences the robot's decision similarly. According to ANOVA analysis, the use of different Emotion Weight Coefficients influenced the final decision in a range of situations, such as in a request for a dietary violation F(4, 35) = 11.2, p = 0.0001 and in an animal compassion situation F(4, 35) = 8.5441, p = 0.0001. A demonstration code repository is provided at: this https URL

[Paper Link](https://arxiv.org/abs/2405.05824)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_15-56.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Evaluating Real-World Robot Manipulation Policies in Simulation

- **Authors**: Xuanlin Li, Kyle Hsu, Jiayuan Gu, Karl Pertsch, Oier Mees, Homer Rich Walke, Chuyuan Fu, Ishikaa Lunawat, Isabel Sieh, Sean Kirmani, Sergey Levine, Jiajun Wu, Chelsea Finn, Hao Su, Quan Vuong, Ted Xiao
- **Main Affiliations**: UC San Diego, Stanford University, UC Berkeley, Google Deepmind
- **Tags**: `Simulation to Reality`

#### Abstract

The field of robotics has made significant advances towards generalist robot manipulation policies. However, real-world evaluation of such policies is not scalable and faces reproducibility challenges, which are likely to worsen as policies broaden the spectrum of tasks they can perform. We identify control and visual disparities between real and simulated environments as key challenges for reliable simulated evaluation and propose approaches for mitigating these gaps without needing to craft full-fidelity digital twins of real-world environments. We then employ these approaches to create SIMPLER, a collection of simulated environments for manipulation policy evaluation on common real robot setups. Through paired sim-and-real evaluations of manipulation policies, we demonstrate strong correlation between policy performance in SIMPLER environments and in the real world. Additionally, we find that SIMPLER evaluations accurately reflect real-world policy behavior modes such as sensitivity to various distribution shifts. We open-source all SIMPLER environments along with our workflow for creating new environments at this https URL to facilitate research on general-purpose manipulation policies and simulated evaluation frameworks.

[Paper Link](https://arxiv.org/abs/2405.05941)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_15-47.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## Probing Multimodal LLMs as World Models for Driving

- **Authors**: Shiva Sreeram, Tsun-Hsuan Wang, Alaa Maalouf, Guy Rosman, Sertac Karaman, Daniela Rus
- **Main Affiliations**: MIT
- **Tags**: `Large Language Models`

#### Abstract

We provide a sober look at the application of Multimodal Large Language Models (MLLMs) within the domain of autonomous driving and challenge/verify some common assumptions, focusing on their ability to reason and interpret dynamic driving scenarios through sequences of images/frames in a closed-loop control environment. Despite the significant advancements in MLLMs like GPT-4V, their performance in complex, dynamic driving environments remains largely untested and presents a wide area of exploration. We conduct a comprehensive experimental study to evaluate the capability of various MLLMs as world models for driving from the perspective of a fixed in-car camera. Our findings reveal that, while these models proficiently interpret individual images, they struggle significantly with synthesizing coherent narratives or logical sequences across frames depicting dynamic behavior. The experiments demonstrate considerable inaccuracies in predicting (i) basic vehicle dynamics (forward/backward, acceleration/deceleration, turning right or left), (ii) interactions with other road actors (e.g., identifying speeding cars or heavy traffic), (iii) trajectory planning, and (iv) open-set dynamic scene reasoning, suggesting biases in the models' training data. To enable this experimental study we introduce a specialized simulator, DriveSim, designed to generate diverse driving scenarios, providing a platform for evaluating MLLMs in the realms of driving. Additionally, we contribute the full open-source code and a new dataset, "Eval-LLM-Drive", for evaluating MLLMs in driving. Our results highlight a critical gap in the current capabilities of state-of-the-art MLLMs, underscoring the need for enhanced foundation models to improve their applicability in real-world dynamic environments.

[Paper Link](https://arxiv.org/abs/2405.05956)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-20_15-44.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-07

### DexSkills: Skill Segmentation Using Haptic Data for Learning Autonomous Long-Horizon Robotic Manipulation Tasks

- **Authors**: Xiaofeng Mao, Gabriele Giudici, Claudio Coppola, Kaspar Althoefer, Ildar Farkhatdinov, Zhibin Li, Lorenzo Jamone
- **Main Affiliations**: University of Edinburgh, ARQ (the Centre for Advanced Robotics @ Queen Mary)
- **Tags**: `teleoperation`

#### Abstract

Effective execution of long-horizon tasks with dexterous robotic hands remains a significant challenge in real-world problems. While learning from human demonstrations have shown encouraging results, they require extensive data collection for training. Hence, decomposing long-horizon tasks into reusable primitive skills is a more efficient approach. To achieve so, we developed DexSkills, a novel supervised learning framework that addresses long-horizon dexterous manipulation tasks using primitive skills. DexSkills is trained to recognize and replicate a select set of skills using human demonstration data, which can then segment a demonstrated long-horizon dexterous manipulation task into a sequence of primitive skills to achieve one-shot execution by the robot directly. Significantly, DexSkills operates solely on proprioceptive and tactile data, i.e., haptic data. Our real-world robotic experiments show that DexSkills can accurately segment skills, thereby enabling autonomous robot execution of a diverse range of tasks.

[Paper Link](https://arxiv.org/abs/2405.03476)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-09_17-11.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-05-06

### Learning Robust Autonomous Navigation and Locomotion for Wheeled-Legged Robots

- **Authors**: Joonho Lee, Marko Bjelonic, Alexander Reske, Lorenz Wellhausen, Takahiro Miki, Marco Hutter
- **Main Affiliations**: Robotic Systems Lab-ETH Zurich
- **Tags**: `Wheeled-Legged Robots`

#### Abstract

Autonomous wheeled-legged robots have the potential to transform logistics systems, improving operational efficiency and adaptability in urban environments. Navigating urban environments, however, poses unique challenges for robots, necessitating innovative solutions for locomotion and navigation. These challenges include the need for adaptive locomotion across varied terrains and the ability to navigate efficiently around complex dynamic obstacles. This work introduces a fully integrated system comprising adaptive locomotion control, mobility-aware local navigation planning, and large-scale path planning within the city. Using model-free reinforcement learning (RL) techniques and privileged learning, we develop a versatile locomotion controller. This controller achieves efficient and robust locomotion over various rough terrains, facilitated by smooth transitions between walking and driving modes. It is tightly integrated with a learned navigation controller through a hierarchical RL framework, enabling effective navigation through challenging terrain and various obstacles at high speed. Our controllers are integrated into a large-scale urban navigation system and validated by autonomous, kilometer-scale navigation missions conducted in Zurich, Switzerland, and Seville, Spain. These missions demonstrate the system's robustness and adaptability, underscoring the importance of integrated control systems in achieving seamless navigation in complex environments. Our findings support the feasibility of wheeled-legged robots and hierarchical RL for autonomous navigation, with implications for last-mile delivery and beyond.

[Paper Link](https://arxiv.org/abs/2405.01792)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-09_16-57.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-30

### Dexterous Grasp Transformer

- **Authors**: Guo-Hao Xu, Yi-Lin Wei, Dian Zheng, Xiao-Ming Wu, Wei-Shi Zheng
- **Main Affiliations**: Sun Yat-sen University
- **Tags**: `Dexterous Grasp`

#### Abstract

In this work, we propose a novel discriminative framework for dexterous grasp generation, named Dexterous Grasp TRansformer (DGTR), capable of predicting a diverse set of feasible grasp poses by processing the object point cloud with only one forward pass. We formulate dexterous grasp generation as a set prediction task and design a transformer-based grasping model for it. However, we identify that this set prediction paradigm encounters several optimization challenges in the field of dexterous grasping and results in restricted performance. To address these issues, we propose progressive strategies for both the training and testing phases. First, the dynamic-static matching training (DSMT) strategy is presented to enhance the optimization stability during the training phase. Second, we introduce the adversarial-balanced test-time adaptation (AB-TTA) with a pair of adversarial losses to improve grasping quality during the testing phase. Experimental results on the DexGraspNet dataset demonstrate the capability of DGTR to predict dexterous grasp poses with both high quality and diversity. Notably, while keeping high quality, the diversity of grasp poses predicted by DGTR significantly outperforms previous works in multiple metrics without any data pre-processing. Codes are available at this https URL .

[Paper Link](https://arxiv.org/abs/2404.18135)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-03_16-56.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Quadruped robot traversing 3D complex environments with limited perception

- **Authors**: Yi Cheng, Hang Liu, Guoping Pan, Linqi Ye, Houde Liu, Bin Liang
- **Main Affiliations**: Tsinghua University
- **Tags**: `Simulation to Reality`

#### Abstract

Traversing 3-D complex environments has always been a significant challenge for legged locomotion. Existing methods typically rely on external sensors such as vision and lidar to preemptively react to obstacles by acquiring environmental information. However, in scenarios like nighttime or dense forests, external sensors often fail to function properly, necessitating robots to rely on proprioceptive sensors to perceive diverse obstacles in the environment and respond promptly. This task is undeniably challenging. Our research finds that methods based on collision detection can enhance a robot's perception of environmental obstacles. In this work, we propose an end-to-end learning-based quadruped robot motion controller that relies solely on proprioceptive sensing. This controller can accurately detect, localize, and agilely respond to collisions in unknown and complex 3D environments, thereby improving the robot's traversability in complex environments. We demonstrate in both simulation and real-world experiments that our method enables quadruped robots to successfully traverse challenging obstacles in various complex environments.

[Paper Link](https://arxiv.org/abs/2404.18225)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-03_16-52.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-29

### Part-Guided 3D RL for Sim2Real Articulated Object Manipulation

- **Authors**: Pengwei Xie, Rui Chen, Siang Chen, Yuzhe Qin, Fanbo Xiang, Tianyu Sun, Jing Xu, Guijin Wang, Hao Su
- **Main Affiliations**: Tsinghua University, Shanghai AI Laboratory, University of California, San Diego
- **Tags**: `Simulation to Reality`

#### Abstract

Manipulating unseen articulated objects through visual feedback is a critical but challenging task for real robots. Existing learning-based solutions mainly focus on visual affordance learning or other pre-trained visual models to guide manipulation policies, which face challenges for novel instances in real-world scenarios. In this paper, we propose a novel part-guided 3D RL framework, which can learn to manipulate articulated objects without demonstrations. We combine the strengths of 2D segmentation and 3D RL to improve the efficiency of RL policy training. To improve the stability of the policy on real robots, we design a Frame-consistent Uncertainty-aware Sampling (FUS) strategy to get a condensed and hierarchical 3D representation. In addition, a single versatile RL policy can be trained on multiple articulated object manipulation tasks simultaneously in simulation and shows great generalizability to novel categories and instances. Experimental results demonstrate the effectiveness of our framework in both simulation and real-world settings. Our code is available at this https URL.

[Paper Link](https://arxiv.org/abs/2404.17302)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-03_16-31.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Ag2Manip: Learning Novel Manipulation Skills with Agent-Agnostic Visual and Action Representations

- **Authors**: Puhao Li, Tengyu Liu, Yuyang Li, Muzhi Han, Haoran Geng, Shu Wang, Yixin Zhu, Song-Chun Zhu, Siyuan Huang
- **Main Affiliations**: Beijing Institute for General Artificial Intelligence, Tsinghua University, Peking University, University of California, Los Angeles
- **Tags**: `Agent-Agnostic Visual Representation`

#### Abstract

Autonomous robotic systems capable of learning novel manipulation tasks are poised to transform industries from manufacturing to service automation. However, modern methods (e.g., VIP and R3M) still face significant hurdles, notably the domain gap among robotic embodiments and the sparsity of successful task executions within specific action spaces, resulting in misaligned and ambiguous task representations. We introduce Ag2Manip (Agent-Agnostic representations for Manipulation), a framework aimed at surmounting these challenges through two key innovations: a novel agent-agnostic visual representation derived from human manipulation videos, with the specifics of embodiments obscured to enhance generalizability; and an agent-agnostic action representation abstracting a robot's kinematics to a universal agent proxy, emphasizing crucial interactions between end-effector and object. Ag2Manip's empirical validation across simulated benchmarks like FrankaKitchen, ManiSkill, and PartManip shows a 325% increase in performance, achieved without domain-specific demonstrations. Ablation studies underline the essential contributions of the visual and action representations to this success. Extending our evaluations to the real world, Ag2Manip significantly improves imitation learning success rates from 50% to 77.5%, demonstrating its effectiveness and generalizability across both simulated and physical environments.

[Paper Link](https://arxiv.org/abs/2404.17521)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-05-03_16-25.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-26

### Leveraging Pretrained Latent Representations for Few-Shot Imitation Learning on a Dexterous Robotic Hand

- **Authors**: Davide Liconti, Yasunori Toshimitsu, Robert Katzschmann
- **Main Affiliations**: ETH
- **Tags**: `Behavioral Cloning`

#### Abstract

In the context of imitation learning applied to dexterous robotic hands, the high complexity of the systems makes learning complex manipulation tasks challenging. However, the numerous datasets depicting human hands in various different tasks could provide us with better knowledge regarding human hand motion. We propose a method to leverage multiple large-scale task-agnostic datasets to obtain latent representations that effectively encode motion subtrajectories that we included in a transformer-based behavior cloning method. Our results demonstrate that employing latent representations yields enhanced performance compared to conventional behavior cloning methods, particularly regarding resilience to errors and noise in perception and proprioception. Furthermore, the proposed approach solely relies on human demonstrations, eliminating the need for teleoperation and, therefore, accelerating the data acquisition process. Accurate inverse kinematics for fingertip retargeting ensures precise transfer from human hand data to the robot, facilitating effective learning and deployment of manipulation policies. Finally, the trained policies have been successfully transferred to a real-world 23Dof robotic system.

[Paper Link](https://arxiv.org/abs/2404.16483)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-28_11-49.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Learning Visuotactile Skills with Two Multifingered Hands

- **Authors**: Toru Lin, Yu Zhang, Qiyang Li, Haozhi Qi, Brent Yi, Sergey Levine, Jitendra Malik
- **Main Affiliations**: University of California, Berkeley
- **Tags**: `visuotactile`

#### Abstract

Aiming to replicate human-like dexterity, perceptual experiences, and motion patterns, we explore learning from human demonstrations using a bimanual system with multifingered hands and visuotactile data. Two significant challenges exist: the lack of an affordable and accessible teleoperation system suitable for a dual-arm setup with multifingered hands, and the scarcity of multifingered hand hardware equipped with touch sensing. To tackle the first challenge, we develop HATO, a low-cost hands-arms teleoperation system that leverages off-the-shelf electronics, complemented with a software suite that enables efficient data collection; the comprehensive software suite also supports multimodal data processing, scalable policy learning, and smooth policy deployment. To tackle the latter challenge, we introduce a novel hardware adaptation by repurposing two prosthetic hands equipped with touch sensors for research. Using visuotactile data collected from our system, we learn skills to complete long-horizon, high-precision tasks which are difficult to achieve without multifingered dexterity and touch feedback. Furthermore, we empirically investigate the effects of dataset size, sensing modality, and visual input preprocessing on policy learning. Our results mark a promising step forward in bimanual multifingered manipulation from visuotactile data. Videos, code, and datasets can be found at this https URL .

[Paper Link](https://arxiv.org/abs/2404.16823)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-28_11-36.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-17

### Scaling Instructable Agents Across Many Simulated Worlds

- **Authors**: SIMA Team, Maria Abi Raad, Arun Ahuja, Catarina Barros, Frederic Besse, Andrew Bolt, Adrian Bolton, Bethanie Brownfield, Gavin Buttimore, Max Cant, Sarah Chakera, Stephanie C. Y. Chan, Jeff Clune, Adrian Collister, Vikki Copeman, Alex Cullum, Ishita Dasgupta, Dario de Cesare, Julia Di Trapani, Yani Donchev, Emma Dunleavy, Martin Engelcke, Ryan Faulkner, Frankie Garcia, Charles Gbadamosi, Zhitao Gong, Lucy Gonzales, Karol Gregor, Arne Olav Hallingstad, Tim Harley, Sam Haves, Felix Hill, Ed Hirst, Drew A. Hudson, Steph Hughes-Fitt, Danilo J. Rezende, Mimi Jasarevic, Laura Kampis, Rosemary Ke, Thomas Keck, Junkyung Kim, Oscar Knagg, Kavya Kopparapu, Andrew Lampinen, Shane Legg, Alexander Lerchner, Marjorie Limont, Yulan Liu, Maria Loks-Thompson, Joseph Marino, Kathryn Martin Cussons, Loic Matthey, Siobhan Mcloughlin, Piermaria Mendolicchio, Hamza Merzic, Anna Mitenkova, Alexandre Moufarek, Valeria Oliveira, Yanko Oliveira, Hannah Openshaw, Renke Pan, Aneesh Pappu, Alex Platonov, Ollie Purkiss, David Reichert, John Reid, Pierre Harvey Richemond, Tyson Roberts, Giles Ruscoe, Jaume Sanchez Elias, Tasha Sandars, Daniel P. Sawyer, Tim Scholtes, Guy Simmons, Daniel Slater, Hubert Soyer, Heiko Strathmann, Peter Stys, Allison C. Tam, Denis Teplyashin, Tayfun Terzi, Davide Vercelli, Bojan Vujatovic, Marcus Wainwright, Jane X. Wang, Zhengdong Wang, Daan Wierstra, Duncan Williams, Nathaniel Wong, Sarah York, Nick Young
- **Main Affiliations**: Google DeepMind
- **Tags**: `dataset`

#### Abstract

Building embodied AI systems that can follow arbitrary language instructions in any 3D environment is a key challenge for creating general AI. Accomplishing this goal requires learning to ground language in perception and embodied actions, in order to accomplish complex tasks. The Scalable, Instructable, Multiworld Agent (SIMA) project tackles this by training agents to follow free-form instructions across a diverse range of virtual 3D environments, including curated research environments as well as open-ended, commercial video games. Our goal is to develop an instructable agent that can accomplish anything a human can do in any simulated 3D environment. Our approach focuses on language-driven generality while imposing minimal assumptions. Our agents interact with environments in real-time using a generic, human-like interface: the inputs are image observations and language instructions and the outputs are keyboard-and-mouse actions. This general approach is challenging, but it allows agents to ground language across many visually complex and semantically rich environments while also allowing us to readily run agents in new environments. In this paper we describe our motivation and goal, the initial progress we have made, and promising preliminary results on several diverse research environments and a variety of commercial video games.

[Paper Link](https://arxiv.org/abs/2404.10179)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-17_21-52.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Closed-Loop Open-Vocabulary Mobile Manipulation with GPT-4V

- **Authors**: Peiyuan Zhi, Zhiyuan Zhang, Muzhi Han, Zeyu Zhang, Zhitian Li, Ziyuan Jiao, Baoxiong Jia, Siyuan Huang
- **Main Affiliations**: State Key Laboratory of General Artificial Intelligence-Beijing Institute for General Artificial Intelligence (BIGAI), Department of Automation-Tsinghua University, University of California Los Angeles
- **Tags**: `Large Language Models`

#### Abstract

Autonomous robot navigation and manipulation in open environments require reasoning and replanning with closed-loop feedback. We present COME-robot, the first closed-loop framework utilizing the GPT-4V vision-language foundation model for open-ended reasoning and adaptive planning in real-world scenarios. We meticulously construct a library of action primitives for robot exploration, navigation, and manipulation, serving as callable execution modules for GPT-4V in task planning. On top of these modules, GPT-4V serves as the brain that can accomplish multimodal reasoning, generate action policy with code, verify the task progress, and provide feedback for replanning. Such design enables COME-robot to (i) actively perceive the environments, (ii) perform situated reasoning, and (iii) recover from failures. Through comprehensive experiments involving 8 challenging real-world tabletop and manipulation tasks, COME-robot demonstrates a significant improvement in task success rate (~25%) compared to state-of-the-art baseline methods. We further conduct comprehensive analyses to elucidate how COME-robot's design facilitates failure recovery, free-form instruction following, and long-horizon task planning.

[Paper Link](https://arxiv.org/abs/2404.10220)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-17_21-47.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-16

### PhyScene: Physically Interactable 3D Scene Synthesis for Embodied AI

- **Authors**: Yandan Yang, Baoxiong Jia, Peiyuan Zhi, Siyuan Huang
- **Main Affiliations**: State Key Laboratory of General Artificial Intelligence,Beijing Institute for General Artificial Intelligence (BIGAI)
- **Tags**: `dataset`

#### Abstract

With recent developments in Embodied Artificial Intelligence (EAI) research, there has been a growing demand for high-quality, large-scale interactive scene generation. While prior methods in scene synthesis have prioritized the naturalness and realism of the generated scenes, the physical plausibility and interactivity of scenes have been largely left unexplored. To address this disparity, we introduce PhyScene, a novel method dedicated to generating interactive 3D scenes characterized by realistic layouts, articulated objects, and rich physical interactivity tailored for embodied agents. Based on a conditional diffusion model for capturing scene layouts, we devise novel physics- and interactivity-based guidance mechanisms that integrate constraints from object collision, room layout, and object reachability. Through extensive experiments, we demonstrate that PhyScene effectively leverages these guidance functions for physically interactable scene synthesis, outperforming existing state-of-the-art scene synthesis methods by a large margin. Our findings suggest that the scenes generated by PhyScene hold considerable potential for facilitating diverse skill acquisition among agents within interactive environments, thereby catalyzing further advancements in embodied AI research. Project website: this http URL.

[Paper Link](https://arxiv.org/abs/2404.09465)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-17_21-32.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-12

### QuasiSim: Parameterized Quasi-Physical Simulators for Dexterous Manipulations Transfer

- **Authors**: Xueyi Liu, Kangbo Lyu, Jieqiong Zhang, Tao Du, Li Yi
- **Main Affiliations**: Tsinghua University, Shanghai AI Laboratory, Shanghai Qi Zhi Institute
- **Tags**: `Simulation to Reality`

#### Abstract

We explore the dexterous manipulation transfer problem by designing simulators. The task wishes to transfer human manipulations to dexterous robot hand simulations and is inherently difficult due to its intricate, highly-constrained, and discontinuous dynamics and the need to control a dexterous hand with a DoF to accurately replicate human manipulations. Previous approaches that optimize in high-fidelity black-box simulators or a modified one with relaxed constraints only demonstrate limited capabilities or are restricted by insufficient simulation fidelity. We introduce parameterized quasi-physical simulators and a physics curriculum to overcome these limitations. The key ideas are 1) balancing between fidelity and optimizability of the simulation via a curriculum of parameterized simulators, and 2) solving the problem in each of the simulators from the curriculum, with properties ranging from high task optimizability to high fidelity. We successfully enable a dexterous hand to track complex and diverse manipulations in high-fidelity simulated environments, boosting the success rate by 11\%+ from the best-performed baseline. The project website is available at this https URL.

[Paper Link](https://arxiv.org/abs/2404.07988)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-12_11-19.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-11

### GOAT-Bench: A Benchmark for Multi-Modal Lifelong Navigation

- **Authors**: Mukul Khanna, Ram Ramrakhya, Gunjan Chhablani, Sriram Yenamandra, Theophile Gervet, Matthew Chang, Zsolt Kira, Devendra Singh Chaplot, Dhruv Batra, Roozbeh Mottaghi
- **Main Affiliations**: Georgia Institute of Technology, Carnegie Mellon University, University of Illinois Urbana-Champaign, Mistral AI, University of Washington
- **Tags**: `Large Language Models`

#### Abstract

The Embodied AI community has made significant strides in visual navigation tasks, exploring targets from 3D coordinates, objects, language descriptions, and images. However, these navigation models often handle only a single input modality as the target. With the progress achieved so far, it is time to move towards universal navigation models capable of handling various goal types, enabling more effective user interaction with robots. To facilitate this goal, we propose GOAT-Bench, a benchmark for the universal navigation task referred to as GO to AnyThing (GOAT). In this task, the agent is directed to navigate to a sequence of targets specified by the category name, language description, or image in an open-vocabulary fashion. We benchmark monolithic RL and modular methods on the GOAT task, analyzing their performance across modalities, the role of explicit and implicit scene memories, their robustness to noise in goal specifications, and the impact of memory in lifelong scenarios.

[Paper Link](https://arxiv.org/abs/2404.06609)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-11_16-29.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### GenCHiP: Generating Robot Policy Code for High-Precision and Contact-Rich Manipulation Tasks

- **Authors**: Kaylee Burns, Ajinkya Jain, Keegan Go, Fei Xia, Michael Stark, Stefan Schaal, Karol Hausman
- **Main Affiliations**: [Google] Intrinsic, Stanford University, Google DeepMind
- **Tags**: `Large Language Models`

#### Abstract

Large Language Models (LLMs) have been successful at generating robot policy code, but so far these results have been limited to high-level tasks that do not require precise movement. It is an open question how well such approaches work for tasks that require reasoning over contact forces and working within tight success tolerances. We find that, with the right action space, LLMs are capable of successfully generating policies for a variety of contact-rich and high-precision manipulation tasks, even under noisy conditions, such as perceptual errors or grasping inaccuracies. Specifically, we reparameterize the action space to include compliance with constraints on the interaction forces and stiffnesses involved in reaching a target pose. We validate this approach on subtasks derived from the Functional Manipulation Benchmark (FMB) and NIST Task Board Benchmarks. Exposing this action space alongside methods for estimating object poses improves policy generation with an LLM by greater than 3x and 4x when compared to non-compliant action spaces

[Paper Link](https://arxiv.org/abs/2404.06645)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-11_16-21.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Wild Visual Navigation: Fast Traversability Learning via Pre-Trained Models and Online Self-Supervision

- **Authors**: Matías Mattamala, Jonas Frey, Piotr Libera, Nived Chebrolu, Georg Martius, Cesar Cadena, Marco Hutter, Maurice Fallon
- **Main Affiliations**: University of Oxford, Robotic Systems Lab-ETH Zurich
- **Tags**: `Navigation`

#### Abstract

Natural environments such as forests and grasslands are challenging for robotic navigation because of the false perception of rigid obstacles from high grass, twigs, or bushes. In this work, we present Wild Visual Navigation (WVN), an online self-supervised learning system for visual traversability estimation. The system is able to continuously adapt from a short human demonstration in the field, only using onboard sensing and computing. One of the key ideas to achieve this is the use of high-dimensional features from pre-trained self-supervised models, which implicitly encode semantic information that massively simplifies the learning task. Further, the development of an online scheme for supervision generator enables concurrent training and inference of the learned model in the wild. We demonstrate our approach through diverse real-world deployments in forests, parks, and grasslands. Our system is able to bootstrap the traversable terrain segmentation in less than 5 min of in-field training time, enabling the robot to navigate in complex, previously unseen outdoor terrains. Code: this https URL - Project page:this https URL

[Paper Link](https://arxiv.org/abs/2404.07110)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-11_16-03.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-09

### Long-horizon Locomotion and Manipulation on a Quadrupedal Robot with Large Language Models

- **Authors**: Yutao Ouyang, Jinhan Li, Yunfei Li, Zhongyu Li, Chao Yu, Koushil Sreenath, Yi Wu
- **Main Affiliations**: Shanghai Qizhi Institute, Tsinghua University, University of California, Berkeley
- **Tags**: `Large Language Models`

#### Abstract

We present a large language model (LLM) based system to empower quadrupedal robots with problem-solving abilities for long-horizon tasks beyond short-term motions. Long-horizon tasks for quadrupeds are challenging since they require both a high-level understanding of the semantics of the problem for task planning and a broad range of locomotion and manipulation skills to interact with the environment. Our system builds a high-level reasoning layer with large language models, which generates hybrid discrete-continuous plans as robot code from task descriptions. It comprises multiple LLM agents: a semantic planner for sketching a plan, a parameter calculator for predicting arguments in the plan, and a code generator to convert the plan into executable robot code. At the low level, we adopt reinforcement learning to train a set of motion planning and control skills to unleash the flexibility of quadrupeds for rich environment interactions. Our system is tested on long-horizon tasks that are infeasible to complete with one single skill. Simulation and real-world experiments show that it successfully figures out multi-step strategies and demonstrates non-trivial behaviors, including building tools or notifying a human for help.

[Paper Link](https://arxiv.org/abs/2404.05291)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-09_22-05.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Humanoid-Gym: Reinforcement Learning for Humanoid Robot with Zero-Shot Sim2Real Transfer

- **Authors**: Xinyang Gu, Yen-Jen Wang, Jianyu Chen
- **Main Affiliations**: Shanghai Qizhi Institute, RobotEra, IIIS, Tsinghua University
- **Tags**: `Simulation to Reality`

#### Abstract

Humanoid-Gym is an easy-to-use reinforcement learning (RL) framework based on Nvidia Isaac Gym, designed to train locomotion skills for humanoid robots, emphasizing zero-shot transfer from simulation to the real-world environment. Humanoid-Gym also integrates a sim-to-sim framework from Isaac Gym to Mujoco that allows users to verify the trained policies in different physical simulations to ensure the robustness and generalization of the policies. This framework is verified by RobotEra's XBot-S (1.2-meter tall humanoid robot) and XBot-L (1.65-meter tall humanoid robot) in a real-world environment with zero-shot sim-to-real transfer. The project website and source code can be found at: this https URL.

[Paper Link](https://arxiv.org/abs/2404.05695)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-09_21-00.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-05

### Self-supervised 6-DoF Robot Grasping by Demonstration via Augmented Reality Teleoperation System

- **Authors**: Xiwen Dengxiong, Xueting Wang, Shi Bai, Yunbo Zhang
- **Main Affiliations**: Rochester Institute of Technology
- **Tags**: `AR demonstrations`

#### Abstract

Most existing 6-DoF robot grasping solutions depend on strong supervision on grasp pose to ensure satisfactory performance, which could be laborious and impractical when the robot works in some restricted area. To this end, we propose a self-supervised 6-DoF grasp pose detection framework via an Augmented Reality (AR) teleoperation system that can efficiently learn human demonstrations and provide 6-DoF grasp poses without grasp pose annotations. Specifically, the system collects the human demonstration from the AR environment and contrastively learns the grasping strategy from the demonstration. For the real-world experiment, the proposed system leads to satisfactory grasping abilities and learning to grasp unknown objects within three demonstrations.

[Paper Link](https://arxiv.org/abs/2404.03067)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_14-08.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Embodied Neuromorphic Artificial Intelligence for Robotics: Perspectives, Challenges, and Research Development Stack

- **Authors**: Rachmad Vidya Wicaksana Putra, Alberto Marchisio, Fakhreddine Zayer, Jorge Dias, Muhammad Shafique
- **Main Affiliations**: New York University
- **Tags**: `Survey`

#### Abstract

Robotic technologies have been an indispensable part for improving human productivity since they have been helping humans in completing diverse, complex, and intensive tasks in a fast yet accurate and efficient way. Therefore, robotic technologies have been deployed in a wide range of applications, ranging from personal to industrial use-cases. However, current robotic technologies and their computing paradigm still lack embodied intelligence to efficiently interact with operational environments, respond with correct/expected actions, and adapt to changes in the environments. Toward this, recent advances in neuromorphic computing with Spiking Neural Networks (SNN) have demonstrated the potential to enable the embodied intelligence for robotics through bio-plausible computing paradigm that mimics how the biological brain works, known as "neuromorphic artificial intelligence (AI)". However, the field of neuromorphic AI-based robotics is still at an early stage, therefore its development and deployment for solving real-world problems expose new challenges in different design aspects, such as accuracy, adaptability, efficiency, reliability, and security. To address these challenges, this paper will discuss how we can enable embodied neuromorphic AI for robotic systems through our perspectives: (P1) Embodied intelligence based on effective learning rule, training mechanism, and adaptability; (P2) Cross-layer optimizations for energy-efficient neuromorphic computing; (P3) Representative and fair benchmarks; (P4) Low-cost reliability and safety enhancements; (P5) Security and privacy for neuromorphic computing; and (P6) A synergistic development for energy-efficient and robust neuromorphic-based robotics. Furthermore, this paper identifies research challenges and opportunities, as well as elaborates our vision for future research development toward embodied neuromorphic AI for robotics.

[Paper Link](https://arxiv.org/abs/2404.03325)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_14-00.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Robot Safety Monitoring using Programmable Light Curtains

- **Authors**: Karnik Ram, Shobhit Aggarwal, Robert Tamburo, Siddharth Ancha, Srinivasa Narasimhan
- **Main Affiliations**: Carnegie Mellon University, Technical University of Munich, MIT
- **Tags**: `Programmable Light Curtains`

#### Abstract

As factories continue to evolve into collaborative spaces with multiple robots working together with human supervisors in the loop, ensuring safety for all actors involved becomes critical. Currently, laser-based light curtain sensors are widely used in factories for safety monitoring. While these conventional safety sensors meet high accuracy standards, they are difficult to reconfigure and can only monitor a fixed user-defined region of space. Furthermore, they are typically expensive. Instead, we leverage a controllable depth sensor, programmable light curtains (PLC), to develop an inexpensive and flexible real-time safety monitoring system for collaborative robot workspaces. Our system projects virtual dynamic safety envelopes that tightly envelop the moving robot at all times and detect any objects that intrude the envelope. Furthermore, we develop an instrumentation algorithm that optimally places (multiple) PLCs in a workspace to maximize the visibility coverage of robots. Our work enables fence-less human-robot collaboration, while scaling to monitor multiple robots with few sensors. We analyze our system in a real manufacturing testbed with four robot arms and demonstrate its capabilities as a fast, accurate, and inexpensive safety monitoring solution.

[Paper Link](https://arxiv.org/abs/2404.03556)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_13-58.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Embodied AI with Two Arms: Zero-shot Learning, Safety and Modularity

- **Authors**: Jake Varley, Sumeet Singh, Deepali Jain, Krzysztof Choromanski, Andy Zeng, Somnath Basu Roy Chowdhury, Avinava Dubey, Vikas Sindhwani
- **Main Affiliations**: Google DeepMind, Google Research
- **Tags**: `Large Language Models`

#### Abstract

We present an embodied AI system which receives open-ended natural language instructions from a human, and controls two arms to collaboratively accomplish potentially long-horizon tasks over a large workspace. Our system is modular: it deploys state of the art Large Language Models for task planning,Vision-Language models for semantic perception, and Point Cloud transformers for grasping. With semantic and physical safety in mind, these modules are interfaced with a real-time trajectory optimizer and a compliant tracking controller to enable human-robot proximity. We demonstrate performance for the following tasks: bi-arm sorting, bottle opening, and trash disposal tasks. These are done zero-shot where the models used have not been trained with any real world data from this bi-arm robot, scenes or workspace.Composing both learning- and non-learning-based components in a modular fashion with interpretable inputs and outputs allows the user to easily debug points of failures and fragilities. One may also in-place swap modules to improve the robustness of the overall platform, for instance with imitation-learned policies.

[Paper Link](https://arxiv.org/abs/2404.03570)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_13-52.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_13-54.png" alt="Embodied AI with Two Arms: Zero-shot Learning, Safety and Modularity" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Anticipate & Collab: Data-driven Task Anticipation and Knowledge-driven Planning for Human-robot Collaboration

- **Authors**: Shivam Singh, Karthik Swaminathan, Raghav Arora, Ramandeep Singh, Ahana Datta, Dipanjan Das, Snehasis Banerjee, Mohan Sridharan, Madhava Krishna
- **Main Affiliations**: Robotics Research Center, IIIT Hyderabad, India
- **Tags**: `Human-Robot Collaboration`, `Large Language Models`

#### Abstract

An agent assisting humans in daily living activities can collaborate more effectively by anticipating upcoming tasks. Data-driven methods represent the state of the art in task anticipation, planning, and related problems, but these methods are resource-hungry and opaque. Our prior work introduced a proof of concept framework that used an LLM to anticipate 3 high-level tasks that served as goals for a classical planning system that computed a sequence of low-level actions for the agent to achieve these goals. This paper describes DaTAPlan, our framework that significantly extends our prior work toward human-robot collaboration. Specifically, DaTAPlan planner computes actions for an agent and a human to collaboratively and jointly achieve the tasks anticipated by the LLM, and the agent automatically adapts to unexpected changes in human action outcomes and preferences. We evaluate DaTAPlan capabilities in a realistic simulation environment, demonstrating accurate task anticipation, effective human-robot collaboration, and the ability to adapt to unexpected changes. Project website: this https URL

[Paper Link](https://arxiv.org/abs/2404.03587)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_13-48_1.png" alt="Anticipate & Collab: Data-driven Task Anticipation and Knowledge-driven Planning for Human-robot Collaboration" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_13-48.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### PreAfford: Universal Affordance-Based Pre-Grasping for Diverse Objects and Environments

- **Authors**: Kairui Ding, Boyuan Chen, Ruihai Wu, Yuyang Li, Zongzheng Zhang, Huan-ang Gao, Siqi Li, Yixin Zhu, Guyue Zhou, Hao Dong, Hao Zhao
- **Main Affiliations**: Tsinghua University, Peking University, Zhejiang University
- **Tags**: `Affordance`

#### Abstract

Robotic manipulation of ungraspable objects with two-finger grippers presents significant challenges due to the paucity of graspable features, while traditional pre-grasping techniques, which rely on repositioning objects and leveraging external aids like table edges, lack the adaptability across object categories and scenes. Addressing this, we introduce PreAfford, a novel pre-grasping planning framework that utilizes a point-level affordance representation and a relay training approach to enhance adaptability across a broad range of environments and object types, including those previously unseen. Demonstrated on the ShapeNet-v2 dataset, PreAfford significantly improves grasping success rates by 69% and validates its practicality through real-world experiments. This work offers a robust and adaptable solution for manipulating ungraspable objects.

[Paper Link](https://arxiv.org/abs/2404.03634)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-05_13-32.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-04

### SliceIt! -- A Dual Simulator Framework for Learning Robot Food Slicing

- **Authors**: Cristian C. Beltran-Hernandez, Nicolas Erbetti, Masashi Hamaya
- **Main Affiliations**: OMRON SINIC X Corporation
- **Tags**: `Simulation to Reality`

#### Abstract

Cooking robots can enhance the home experience by reducing the burden of daily chores. However, these robots must perform their tasks dexterously and safely in shared human environments, especially when handling dangerous tools such as kitchen knives. This study focuses on enabling a robot to autonomously and safely learn food-cutting tasks. More specifically, our goal is to enable a collaborative robot or industrial robot arm to perform food-slicing tasks by adapting to varying material properties using compliance control. Our approach involves using Reinforcement Learning (RL) to train a robot to compliantly manipulate a knife, by reducing the contact forces exerted by the food items and by the cutting board. However, training the robot in the real world can be inefficient, and dangerous, and result in a lot of food waste. Therefore, we proposed SliceIt!, a framework for safely and efficiently learning robot food-slicing tasks in simulation. Following a real2sim2real approach, our framework consists of collecting a few real food slicing data, calibrating our dual simulation environment (a high-fidelity cutting simulator and a robotic simulator), learning compliant control policies on the calibrated simulation environment, and finally, deploying the policies on the real robot.

[Paper Link](https://arxiv.org/abs/2404.02569)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-04_17-52.png" alt="image" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### A Survey of Optimization-based Task and Motion Planning: From Classical To Learning Approaches

- **Authors**: Zhigen Zhao, Shuo Chen, Yan Ding, Ziyi Zhou, Shiqi Zhang, Danfei Xu, Ye Zhao
- **Main Affiliations**: Georgia Institute of Technology
- **Tags**: `Survey`, `TAMP`

#### Abstract

Task and Motion Planning (TAMP) integrates high-level task planning and low-level motion planning to equip robots with the autonomy to effectively reason over long-horizon, dynamic tasks. Optimization-based TAMP focuses on hybrid optimization approaches that define goal conditions via objective functions and are capable of handling open-ended goals, robotic dynamics, and physical interaction between the robot and the environment. Therefore, optimization-based TAMP is particularly suited to solve highly complex, contact-rich locomotion and manipulation problems. This survey provides a comprehensive review on optimization-based TAMP, covering (i) planning domain representations, including action description languages and temporal logic, (ii) individual solution strategies for components of TAMP, including AI planning and trajectory optimization (TO), and (iii) the dynamic interplay between logic-based task planning and model-based TO. A particular focus of this survey is to highlight the algorithm structures to efficiently solve TAMP, especially hierarchical and distributed approaches. Additionally, the survey emphasizes the synergy between the classical methods and contemporary learning-based innovations such as large language models. Furthermore, the future research directions for TAMP is discussed in this survey, highlighting both algorithmic and application-specific challenges.

[Paper Link](https://arxiv.org/abs/2404.02817)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-04_17-42.png" alt="image" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-04_17-42_1.png" alt="image" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Learning Quadrupedal Locomotion via Differentiable Simulation

- **Authors**: Clemens Schwarke, Victor Klemm, Jesus Tordesillas, Jean-Pierre Sleiman, Marco Hutter
- **Main Affiliations**: Robotic Systems Lab-ETH Zurich
- **Tags**: `Simulation`

#### Abstract

The emergence of differentiable simulators enabling analytic gradient computation has motivated a new wave of learning algorithms that hold the potential to significantly increase sample efficiency over traditional Reinforcement Learning (RL) methods. While recent research has demonstrated performance gains in scenarios with comparatively smooth dynamics and, thus, smooth optimization landscapes, research on leveraging differentiable simulators for contact-rich scenarios, such as legged locomotion, is scarce. This may be attributed to the discontinuous nature of contact, which introduces several challenges to optimizing with analytic gradients. The purpose of this paper is to determine if analytic gradients can be beneficial even in the face of contact. Our investigation focuses on the effects of different soft and hard contact models on the learning process, examining optimization challenges through the lens of contact simulation. We demonstrate the viability of employing analytic gradients to learn physically plausible locomotion skills with a quadrupedal robot using Short-Horizon Actor-Critic (SHAC), a learning algorithm leveraging analytic gradients, and draw a comparison to a state-of-the-art RL algorithm, Proximal Policy Optimization (PPO), to understand the benefits of analytic gradients.

[Paper Link](https://arxiv.org/abs/2404.02887)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-04_17-00.png" alt="image" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-03

### Generalizing 6-DoF Grasp Detection via Domain Prior Knowledge

- **Authors**: Haoxiang Ma, Modi Shi, Boyang Gao, Di Huang
- **Main Affiliations**: Beihang University, Harbin Institute of Technology, Geometry Robotics
- **Tags**: `6-DoF`

#### Abstract

We focus on the generalization ability of the 6-DoF grasp detection method in this paper. While learning-based grasp detection methods can predict grasp poses for unseen objects using the grasp distribution learned from the training set, they often exhibit a significant performance drop when encountering objects with diverse shapes and structures. To enhance the grasp detection methods' generalization ability, we incorporate domain prior knowledge of robotic grasping, enabling better adaptation to objects with significant shape and structure differences. More specifically, we employ the physical constraint regularization during the training phase to guide the model towards predicting grasps that comply with the physical rule on grasping. For the unstable grasp poses predicted on novel objects, we design a contact-score joint optimization using the projection contact map to refine these poses in cluttered scenarios. Extensive experiments conducted on the GraspNet-1billion benchmark demonstrate a substantial performance gain on the novel object set and the real-world grasping experiments also demonstrate the effectiveness of our generalizing 6-DoF grasp detection method.

[Paper Link](https://arxiv.org/abs/2404.01727)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-08_17-45.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

## 2024-04-01

### Snap-it, Tap-it, Splat-it: Tactile-Informed 3D Gaussian Splatting for Reconstructing Challenging Surfaces

- **Authors**: Mauro Comi, Alessio Tonioni, Max Yang, Jonathan Tremblay, Valts Blukis, Yijiong Lin, Nathan F. Lepora, Laurence Aitchison
- **Main Affiliations**: University of Bristol, Google Zurich, NVIDIA
- **Tags**: `tactile`, `Gaussian Splatting`

#### Abstract

Touch and vision go hand in hand, mutually enhancing our ability to understand the world. From a research perspective, the problem of mixing touch and vision is underexplored and presents interesting challenges. To this end, we propose Tactile-Informed 3DGS, a novel approach that incorporates touch data (local depth maps) with multi-view vision data to achieve surface reconstruction and novel view synthesis. Our method optimises 3D Gaussian primitives to accurately model the object's geometry at points of contact. By creating a framework that decreases the transmittance at touch locations, we achieve a refined surface reconstruction, ensuring a uniformly smooth depth map. Touch is particularly useful when considering non-Lambertian objects (e.g. shiny or reflective surfaces) since contemporary methods tend to fail to reconstruct with fidelity specular highlights. By combining vision and tactile sensing, we achieve more accurate geometry reconstructions with fewer images than prior methods. We conduct evaluation on objects with glossy and reflective surfaces and demonstrate the effectiveness of our approach, offering significant improvements in reconstruction quality.

[Paper Link](https://arxiv.org/abs/2403.20275)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-08_17-31.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---

### Learning Visual Quadrupedal Loco-Manipulation from Demonstrations

- **Authors**: Zhengmao He, Kun Lei, Yanjie Ze, Koushil Sreenath, Zhongyu Li, Huazhe Xu
- **Main Affiliations**: Shanghai Qizhi Institute, Hong Kong University of Science and Technology, University of California, Berkeley, IIIS, Tsinghua University
- **Tags**: `Behavioral Cloning`, `Reinforcement Learning`

#### Abstract

Quadruped robots are progressively being integrated into human environments. Despite the growing locomotion capabilities of quadrupedal robots, their interaction with objects in realistic scenes is still limited. While additional robotic arms on quadrupedal robots enable manipulating objects, they are sometimes redundant given that a quadruped robot is essentially a mobile unit equipped with four limbs, each possessing 3 degrees of freedom (DoFs). Hence, we aim to empower a quadruped robot to execute real-world manipulation tasks using only its legs. We decompose the loco-manipulation process into a low-level reinforcement learning (RL)-based controller and a high-level Behavior Cloning (BC)-based planner. By parameterizing the manipulation trajectory, we synchronize the efforts of the upper and lower layers, thereby leveraging the advantages of both RL and BC. Our approach is validated through simulations and real-world experiments, demonstrating the robot's ability to perform tasks that demand mobility and high precision, such as lifting a basket from the ground while moving, closing a dishwasher, pressing a button, and pushing a door. Project website: this https URL

[Paper Link](https://arxiv.org/abs/2403.20328)

[Website Link](https://zhengmaohe.github.io/leg-manip)

<div style={{ display: 'flex', justifyContent: 'center' }}>
<div style={{ textAlign: 'center', marginRight: '10px' }}>
<img src="/img/daily/2024-04-08_17-20.png" alt="img" style={{ width: 'auto', maxHeight: '400px' }} />
</div>
</div>

---