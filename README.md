# Motion Planner
## Overview
This repository implemented some common motion planners used on autonomous vehicles, including
* [Hybrid A* Planner](https://blog.habrador.com/2015/11/explaining-hybrid-star-pathfinding.html)
* [Lattice Planner](https://www.researchgate.net/publication/224156269_Optimal_Trajectory_Generation_for_Dynamic_Street_Scenarios_in_a_Frenet_Frame)
* [EM Planner](https://arxiv.org/abs/1807.08048) (imcompleted)

Also, this repository provides some controllers for path tracking, including
* [Pure Pursuit + PID](https://www.ri.cmu.edu/pub_files/pub3/coulter_r_craig_1992_1/coulter_r_craig_1992_1.pdf)
* [Rear-Wheel Feedback + PID](https://www.ri.cmu.edu/pub_files/2009/2/Automatic_Steering_Methods_for_Autonomous_Automobile_Path_Tracking.pdf)
* [Front-Wheel Feedback / Stanley + PID](http://robots.stanford.edu/papers/thrun.stanley05.pdf)
* [LQR + PID](https://github.com/ApolloAuto/apollo/tree/master/modules/control/controller)
* [Linear MPC](http://www.mpc.berkeley.edu/mpc-course-material)

## Requirement
* Python 3.6 or above
* [SciPy](https://www.scipy.org/)
* [cvxpy](https://github.com/cvxgrp/cvxpy)
* [Reeds-Shepp Curves](https://github.com/zhm-real/ReedsSheppCurves)
* [pycubicspline](https://github.com/AtsushiSakai/pycubicspline)

## Vehicle models
This repository uses two models: simple car model and [car pulling trailers model](http://planning.cs.uiuc.edu/node661.html#77556).

## Hybrid A* Planner
<div align=right>
<table>
  <tr>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/HybridAstarPlanner/gif/hybrid%20Astar-1.gif" alt="1" width="400"/></a></td>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/HybridAstarPlanner/gif/hybrid%20Astar-2.gif" alt="2" width="400"/></a></td>
  </tr>
</table>
<table>
  <tr>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/HybridAstarPlanner/gif/hybrid%20Astar-t1.gif" alt="11" width="400"/></a></td>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/HybridAstarPlanner/gif/hybrid%20Astar-t5.gif" alt="12" width="400"/></a></td>
  </tr>
</table>
<table>
  <tr>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/HybridAstarPlanner/gif/hybrid%20Astar-t3.gif" alt="13" width="400"/></a></td>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/HybridAstarPlanner/gif/hybrid%20Astar-t2.gif" alt="14" width="400"/></a></td>
  </tr>
</table>
</div>

## State Lattice Planner
<div align=right>
<table>
  <tr>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/LatticePlanner/gif/Crusing.gif" alt="1" width="400"/></a></td>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/LatticePlanner/gif/StoppingMode.gif" alt="2" width="400"/></a></td>
  </tr>
</table>
</div>

## Controllers
<div align=right>
<table>
  <tr>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/Control/gif/purepursuit1.gif" alt="1" width="400"/></a></td>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/Control/gif/purepursuit2.gif" alt="2" width="400"/></a></td>
  </tr>
</table>
<table>
  <tr>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/Control/gif/RWF1.gif" alt="1" width="400"/></a></td>
    <td><img src="https://github.com/zhm-real/MotionPlanning/blob/master/Control/gif/RWF2.gif" alt="2" width="400"/></a></td>
  </tr>
</table>
</div>

## Useful Material
* [ApolloAuto/apollo](https://github.com/ApolloAuto/apollo) by Baidu
* [Optimal Trajectory Generation for Dynamic Street Scenarios in a Frenet Frame](https://www.researchgate.net/publication/224156269_Optimal_Trajectory_Generation_for_Dynamic_Street_Scenarios_in_a_Frenet_Frame) by Moritz Werling, etc
* [Baidu Apollo EM Motion Planner](https://arxiv.org/abs/1807.08048) by Baidu
* [Practical Search Techniques in Path Planning for Autonomous Driving](https://ai.stanford.edu/~ddolgov/papers/dolgov_gpp_stair08.pdf) by Stanford
* [Hybrid Path Planner (C++)](https://github.com/karlkurzer/path_planner) by KTH Research Concept Vehicle
* [hybrid-astar-planner (MATLAB)](https://github.com/wanghuohuo0716/hybrid_A_star) by Mengli Liu
* [HybridAStarTrailer (Julia)](https://github.com/AtsushiSakai/HybridAStarTrailer) by AtsushiSakai
