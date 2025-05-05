# meam620-project-1-phase-1--modeling-and-control-of-a-quadrotor-solved
**TO GET THIS SOLUTION VISIT:** [MEAM620-Project 1 phase 1- Modeling and Control of a Quadrotor Solved](https://www.ankitcodinghub.com/product/meam620-project-1-modeling-and-control-of-a-quadrotor-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;50553&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;MEAM620-Project 1 phase 1- Modeling and Control of a Quadrotor Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
Introduction

In this project you will put your knowledge of quadrotor dynamics to work by developing algorithms for control. A good controller is the backbone of any quadrotor autonomy stack and thus it is crucial that you understand the theory and implementation in this project. You will be reusing the code throughout this course; during the lab session you will use it to fly a real, physical quadrotor! All code written in this project will be in Python. Refer to the instructions on Piazza for more information about which version to use and getting set up.

Figure 1: The CrazyFlie 2.0 robot that will be used in the lab and exercises. An Euler Z-X-Y transformation takes the inertial frame A to the body-fixed frame B. First a rotation by <em>ψ </em>around the <strong>a<sub>3 </sub></strong>axis is performed, then a roll by <em>φ </em>around the (rotated!) <strong>a<sub>1 </sub></strong>axis, and finally a pitch by <em>θ </em>around the (now twice rotated!) <strong>a<sub>2 </sub></strong>axis. A translation <strong>r </strong>then produces the coordinate system B, coinciding with the center of mass <em>C </em>of the robot, and aligned along the arms.

Modeling

Coordinate Systems and Reference frames

The coordinate systems and free body diagram for the quadrotor are shown in Fig. 1. The inertial frame, A, is defined by the triad <strong>a</strong><sub>1</sub>, <strong>a</strong><sub>2</sub>, and <strong>a</strong><sub>3 </sub>with <strong>a</strong><sub>3 </sub>pointing upward. The body frame, B, is attached to the center of mass of the quadrotor with <strong>b</strong><sub>1 </sub>coinciding with the preferred forward direction and <strong>b</strong><sub>3 </sub>being perpendicular to the plane of the rotors pointing vertically up during perfect hover (see Fig. 1). These vectors are parallel to the principal axes. More formally, the coordinates of a vector <strong>x </strong>that is expressed in A as <strong>x </strong>= <sup>P</sup><em><sub>i </sub></em><sup>A</sup><em>x<sub>i</sub></em><strong>a</strong><em><sub>i </sub></em>and in B as <strong>x </strong>= <sup>P</sup><em><sub>i </sub></em><sup>B</sup><em>x<sub>i</sub></em><strong>b</strong><em><sub>i </sub></em>are transformed into each other by the rotation matrix <sup>A</sup><em>R</em><sub>B </sub>and translation vector <sup>A</sup><strong>T</strong><sub>B</sub>:

A&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A B&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A

<strong>x </strong>=&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <em>R</em><sub>B </sub><strong>x </strong>+ <strong>T</strong><sub>B </sub><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(1)

To express the rotational motion of the moving frame B, it is useful to introduce the angular velocity vector <em>ω </em>that describes how the basis vectors <strong>b</strong><em><sub>i </sub></em>move:

d

<strong>b</strong><em><sub>i </sub></em>= <em>ω </em>× <strong>b<sub>i </sub></strong><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(2)

d<em>t</em>

Note that this equation is coordinate free, meaning <em>ω </em>is not yet expressed explicitly in any particular coordinate system. We will denote the components of angular velocity of the robot in the body frame by <em>p</em>, <em>q</em>, and <em>r</em>:

<em>ω </em>= <em>p</em><strong>b</strong><sub>1 </sub>+ <em>q</em><strong>b</strong><sub>2 </sub>+ <em>r</em><strong>b</strong><sub>3</sub><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(3)

The heading (yaw) angle of the robot plays a special role since we can choose it freely without directly affecting the robot’s dynamics. For this reason we use <em>Z </em>− <em>X </em>− <em>Y </em>Euler angles to describe the transform from A to B: first a yaw rotation by <em>ψ </em>around the <strong>a</strong><sub>3 </sub>axis is performed, then a roll by <em>φ </em>around the (rotated!) <strong>a</strong><sub>1 </sub>axis, and finally a pitch by <em>θ </em>around the (now twice rotated!) <strong>a</strong><sub>2 </sub>axis <a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> From the Euler angles one can compute the rotation matrix as follows:

The angular velocity and Euler angle velocities are related by:

(5)

<h2>2.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Motor Model</h2>
This section describes how we model the motors. Each rotor has an angular speed <em>ω<sub>i </sub></em>and produces a vertical force <em>F<sub>i </sub></em>according to:

<em>F</em><em>i </em>= <em>k</em><em>F </em><em>ω</em><em>i</em>2<em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(6)

Experimentation with a fixed rotor at steady-state shows that <em>k<sub>F </sub></em>≈ 6<em>.</em>11 × 10<sup>−8 N</sup><em>/</em>rpm<sup>2</sup>. The rotors also produce a moment according to

<em>M<sub>i </sub></em>= <em>k<sub>M</sub>ω<sub>i</sub></em><sup>2</sup><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(7)

The constant, <em>k<sub>M</sub></em>, is determined to be about 1<em>.</em>5 × 10<sup>−9 Nm</sup><em>/</em>rpm<sup>2 </sup>by matching the performance of the simulation to the real system.

Data obtain from system identification experiments suggest that the rotor speed is related to the commanded speed by a first-order differential equation <em>ω</em>˙<em>i </em>= <em>k</em><em>m</em>(<em>ω</em><em>i</em>des − <em>ω</em><em>i</em>)<em>.</em>

This motor gain, <em>k<sub>m</sub></em>, is found to be about 20s<sup>−1 </sup>by matching the performance of the simulation to the real system. The desired angular velocities, <em>ω<sub>i</sub></em><sup>des</sup>, are limited to a minimum and maximum value determined through experimentation.

However, as a first approximation, we can assume the motor controllers to be perfect and the time constant <em>k<sub>m </sub></em>associated with the motor response to be arbitrarily small. In other words, we can assume the actual motor velocities <em>ω<sub>i </sub></em>are equal to the commanded motor velocities, <em>ω<sub>i</sub><sup>des</sup></em>. Notes:

<ol>
<li>In simulation, you will be able to directly command torque and thrust. The thrust limit is available as a parameter inside the simulator, although you don’t need it for this project.</li>
<li>In the lab, we will provide the code to translate torque and thrust to motor commands. You will however encounter saturation of your motors and may have to tweak your gains.</li>
</ol>
<h2>2.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Rigid Body Dynamics: Newton’s Equations of Motion for the Center of Mass</h2>
We will describe the motion of the center of mass (CoM) in the inertial (“world”) coordinate frame A. This makes sense because we will want to specify our waypoints (where the robot should fly), trajectories and controller targets (where the robot should be at this moment) in the inertial frame.

Newton’s equation of motion for the robot’s CoM <strong>r </strong>is determined by the robot’s mass <em>m</em>, the gravitational force <strong>F</strong><sub>g </sub>= <em>m</em><strong>g</strong>, and the sum of the motor’s individual forces <strong>F</strong><sub>i</sub>:

<table width="0">
<tbody>
<tr>
<td width="537"><em>m</em>¨<strong>r </strong>= <strong>F</strong><sub>g </sub>+ <sup>X</sup><strong>F</strong><sub>i </sub><em>.</em>

<em>i</em>

In the coordinates of the inertial frame A this reads:
</td>
<td width="135">(8)</td>
</tr>
</tbody>
</table>
<em>&nbsp;.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(9)

where <sup>A</sup><em>R</em><sub>B </sub>is the rotation matrix used in Eq (1) constructed via Eq (4). If the robot is tilted, the above equation will mix the propeller forces into the <em>x </em>and <em>y </em>plane and so generate horizontal acceleration of the robot. In other words, we can accomplish movement in all three directions by manipulating the attitude of the vehicle and its thrust.

Equation (9) further suggests that rather than using the forces <em>F<sub>i </sub></em>as control inputs, we should define our first input <em>u</em><sub>1 </sub>as the sum:

<em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(10)

<h2>2.4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Euler’s Equations of Motion for the Attitude</h2>
Since from Eq (9) we know that attitude control is necessary to generate horizontal motion, in this section we will examine how the motors affect the orientation of the vehicle.

In the inertial frame, the rate at which the robot’s angular momentum <strong>L </strong>= <em>I</em><em>ω </em>changes is determined by the total moment <strong>M </strong>generated by the propellers:

<strong>L</strong><sup>˙ </sup>= <strong>M </strong><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(11)

While this equation looks clean and simple in the inertial frame, it is actually hard to work with because the inertial tensor <em>I </em>changes with the attitude of the robot, and is thus time dependent and non diagonal! For control purposes, this equation is best expressed in the body frame that is aligned with the principal axis, where the inertia tensor <em>I </em>is constant, and diagonal. However, since now the basis vectors <strong>b</strong><em><sub>i </sub></em>are time-dependent, the equation for the time derivative of the angular momentum in the body frame becomes:

<table width="0">
<tbody>
<tr>
<td width="648"><strong>L</strong>˙ = XB<em>L</em>˙ <em>i</em><strong>b</strong><em>i </em>+ XB<em>L</em><em>i</em><strong>b</strong>˙ <em>i </em>= XB<em>L</em>˙ <em>i</em><strong>b</strong><em>i </em>+ X<em>ω </em>× B<em>L</em><em>i</em><strong>b</strong><strong>i </strong>= XB<em>L</em>˙ <em>i</em><strong>b</strong><em>i </em>+ <em>ω </em>× <strong>L </strong><em>.</em>

<em>i&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; i</em>

Combining (11) and (12), and using the fact that <em>I </em>is constant in B yield’s Euler’s Equation:
</td>
<td width="24">(12)</td>
</tr>
<tr>
<td width="648"><em>I</em><sup>B</sup><em>ω</em><strong>˙ </strong>= <sup>B</sup><strong>M </strong>− <sup>B</sup><em>ω </em>× <em>I</em><sup>B</sup><em>ω </em><em>,</em></td>
<td width="24">(13)</td>
</tr>
</tbody>
</table>
where depending on context <em>I </em>means alternatingly a tensor or a matrix expressed in the body frame.

How do the motors come into play? First, by generating a force <em>F<sub>i </sub></em>that is a distance <em>l </em>away from the CoM, each motor can exert a torque that is in the <strong>b</strong><sub>1</sub>, <strong>b</strong><sub>2 </sub>plane. In addition, each rotor produces a moment <em>M<sub>i </sub></em>perpendicular to the plane of rotation of the blade. Rotors 1 and 3 rotate clockwise in the −<strong>b</strong><sub>3 </sub>direction while 2 and 4 rotate counter clockwise in the <strong>b</strong><sub>3 </sub>direction. Since the moment produced on the quadrotor is opposite to the direction of rotation of the blades, <em>M</em><sub>1 </sub>and <em>M</em><sub>3 </sub>act in the <strong>b</strong><sub>3 </sub>direction while <em>M</em><sub>2 </sub>and <em>M</em><sub>4 </sub>act in the −<strong>b</strong><sub>3 </sub>direction. In contrast to this, the forces <em>F<sub>i </sub></em>are all in the positive <strong>b</strong><sub>3 </sub>direction due to the fact that the pitch is reversed on two of the propellers, see Fig

1.

Using this geometric intuition, and expressing the angular velocity in the body frame by <em>p</em>, <em>q</em>, and <em>r </em>as in Eq (3), the Euler equation (13) becomes:

<em>&nbsp;.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(14)

Note that the total net torque along the yaw (<strong>b</strong><sub>3</sub>) axis of the robot is simply the signed sum of the motor’s torques <em>M<sub>i </sub></em>(why does the distance <em>l </em>to the center of the robot play no role?). We can rewrite this as:

<table width="0">
<tbody>
<tr>
<td width="95"></td>
<td width="33"><em>l</em>

0

−<em>γ</em>
</td>
<td width="22">0 <em>l γ</em></td>
<td width="323"><em>&nbsp;.</em></td>
<td width="24">(15)</td>
</tr>
</tbody>
</table>
where is the relationship between lift and drag given by Equations (6-7). Accordingly, we will define our second set of inputs to be the vector of moments <strong>u</strong><sub>2 </sub>given by:

<strong>u</strong><em> .&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(16)

Dropping the reference frame superscripts for brevity, we can now write the equations of motion for center of mass and orientation in compact form:

(17)

<em>&nbsp;,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(18)

where (17) is in inertial coordinates, and (18) is in body coordinates. The inputs <em>u</em><sub>1 </sub>and <strong>u</strong><sub>2 </sub>are related to the motor forces <em>F<sub>i </sub></em>via the linear system of equations formed by (10) and (16). We are thus facing a system governed by two coupled second order differential equations which we will exploit in section 3 to design controllers.

Robot Controllers

Trajectory Generation

Our ultimate goal is to make the robot follow a trajectory. For the time let’s assume we are given a trajectory generator that for any given time <em>t </em>produces a trajectory target <strong>z</strong><sup>des</sup>(<em>t</em>) consisting of target position <strong>r</strong><em><sub>T </sub></em>(<em>t</em>) and target yaw <em>ψ<sub>T </sub></em>(<em>t</em>):

<strong>z</strong><sup>des</sup>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (19)

and its first and second derivatives <strong>z</strong>˙<sup>des </sup>and <strong>z</strong>¨<sup>des</sup>. To hover for example, the trajectory generator would produce a constant <strong>r</strong>(<em>t</em>) = <strong>r</strong><sub>0 </sub>and e.g. a fixed <em>ψ</em>(<em>t</em>) = <em>ψ</em><sub>0</sub>, with all derivatives being zero.

The controller’s job will then be to produce the correct torque <strong>u</strong><sub>2 </sub>and thrust <em>u</em><sub>1 </sub>to bring the robot to the desired state specified by the trajectory generator.

<h2>3.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Linear Backstepping Controller</h2>
For this controller we will make the following assumptions:

<ol>
<li>The robot is near the hover points, meaning the roll angle <em>φ </em>and pitch angle <em>θ </em>are small enough to allow linearization of trigonometric functions, i.e. cos(<em>φ</em>) = 1, sin(<em>φ</em>) = <em>φ</em>, cos(<em>θ</em>) = 1, sin(<em>θ</em>) = <em>θ</em>. This will allow us to linearize the rotation matrix in Eq (17).</li>
<li>The robot’s angular velocity is small enough for the cross product term between angular momentum and velocity in (18) to be negligible. This is usually a good assumption for almost any quadrotor.</li>
<li>The attitude of the quadrotor can be controlled at a much smaller time scale than the position. This “backstepping” approach to controller design allows a decoupling of position and attitude control loops. In practice this is generally warranted since the attitude controller usually runs almost an order of magnitude faster than the position controller.</li>
</ol>
Making the backstepping approximation is equivalent to assuming that <em>R </em>in Eq (17) can be commanded instantaneously. This further implies that it is possible to directly command the acceleration <strong>r</strong><sup>des</sup>. Figure 2 shows how trajectory generator, position, and attitude controller play together.

Figure 2: The position and attitude control loops.

Define the position error in terms of components by:

<em>e</em><em>i </em>= (<em>r</em><em>i </em>− <em>r</em><em>i,T </em>)<em>.</em>

In order to guarantee that this error goes exponentially to zero, we require

(<em>r</em>¨<em>i</em>des − <em>r</em>¨<em>i,T </em>) + <em>k</em><em>d,i</em>(<em>r</em>˙<em>i </em>− <em>r</em>˙<em>i,T </em>) + <em>k</em><em>p,i</em>(<em>r</em><em>i </em>− <em>r</em><em>i,T </em>) = 0 <em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(20)

In Eq (20), <em>r<sub>i,T </sub></em>and its derivatives are given by the trajectory generator, and <em>r<sub>i </sub></em>and <em>r</em>˙<em><sub>i </sub></em>are provided by the state estimation system, allowing for the commanded acceleration <em>r</em>¨<em><sub>i</sub></em><sup>des </sup>to be calculated:

<em>r</em>¨<em>i</em>des = <em>r</em>¨<em>i,T </em>− <em>k</em><em>d,i</em>(<em>r</em>˙<em>i </em>− <em>r</em>˙<em>i,T </em>) − <em>k</em><em>p,i</em>(<em>r</em><em>i </em>− <em>r</em><em>i,T </em>) <em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(21)

Now the attitude of the quadrotor must be controlled such that it will generate ¨<strong>r</strong><sup>des</sup>. For this, the linearized version of (17) is used:

(22a)

(22b)

(22c)

From the third equation we can directly read off the thrust control <em>u</em><sub>1</sub>. The first two equations can be solved for <em>θ</em><sup>des </sup>and <em>φ</em><sup>des</sup>, since <em>ψ</em><sup>des </sup>= <em>ψ<sub>T </sub></em>is given directly by the trajectory generator. Linearizing (18), we get:

<em>&nbsp;,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(23)

and by further exploiting that via Eq (5) Euler angle velocities are to linear approximation equal to angular velocities, it becomes evident that we can directly command the acceleration of the Euler angles:

<em>&nbsp;.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(24)

Thus the “inner loop” attitude control can also be done with a simple PD controller:

<strong>u</strong><em> ,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(25)

where the desired roll and pitch velocities <em>p</em><sup>des </sup>and <em>q</em><sup>des </sup>can be computed from the equations of motion and the specified trajectory [1], but in practice can be set to zero. <a href="#_ftn2" name="_ftnref2"><sup>[2]</sup></a>In summary, the controller then works as follows:

<ol>
<li>Use Eq (21) to compute the commanded acceleration ¨<strong>r</strong><sup>des</sup>.</li>
<li>Use Eq (22c) to compute <em>u</em><sub>1 </sub>and the desired angles <em>θ</em><sup>des </sup>and <em>φ</em><sup>des </sup>from (22a) and (22b).</li>
<li>Use Eq (25) to compute <strong>u</strong><sub>2</sub>.</li>
</ol>
<h2>3.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; A Geometric Nonlinear Controller</h2>
Nonlinear controllers are generally built based on geometric intuition, i.e. the quadrotor’s <strong>b</strong><sub>3 </sub>axis is tilted to point in the desired direction, and thrust is applied. Such controllers are suitable for very aggressive maneuvers and will allow for faster flight and sharper turns, in particular in the simulator. Note that we have considerable freedom to choose a control algorithm so long as it results in a stable system.

The following section is based on the controller developed in [1], which in turn is a simplified version of the controller in [2]. For a thorough treatment and stability analysis please refer to [2].

It turns out that the basic layout of the controller remains as shown in Figure 2, i.e. there is an attitude and a position controller, although we no longer make the backstepping assumption.

We start out from the PD controller in Eq (21), but now write it in more compact vector form:

¨<strong>r</strong><sup>des </sup>= ¨<strong>r</strong><em><sub>T </sub></em>− <em>K<sub>d</sub></em>(<strong>r</strong>˙ − <strong>r</strong>˙<em><sub>T </sub></em>) − <em>K<sub>p</sub></em>(<strong>r </strong>− <strong>r</strong><em><sub>T </sub></em>) <em>,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(26)

where <em>K<sub>d </sub></em>and <em>K<sub>p </sub></em>are diagonal, positive definite gain matrices.

We are again faced with the question how to compute the inputs <em>u</em><sub>1</sub>, <strong>u</strong><sub>2 </sub>to generate <strong>¨r</strong><sup>des</sup>. We first determine the input <em>u</em><sub>1</sub>. By rearranging Eq (17) one obtains:

<em>&nbsp;.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(27)

Note that the lhs of (27) is just the total commanded force <strong>F</strong><sup>des </sup>(including gravity):

<strong>F</strong>des = <em>m</em>¨<strong>r</strong>des <em>&nbsp;.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(28)

On the right hand side is <em>u</em><sub>1</sub>, multiplied with the quadrotor’s axis <strong>b</strong><sub>3 </sub>= <em>R</em>[0<em>,</em>0<em>,</em>1]<em><sup>T </sup></em>, expressed in the inertial frame. We obtain the input <em>u</em><sub>1 </sub>by projecting <strong>F</strong><sup>des </sup>onto <strong>b</strong><sub>3</sub>:

<strong>F</strong><sup>des </sup><em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(29)

To compute <strong>u</strong><sub>2</sub>, we observe that a quadrotor can only produce thrust along its <strong>b</strong><sub>3 </sub>axis. It makes sense to align <strong>b</strong><sub>3 </sub>with <strong>F</strong><sup>des</sup>, and align <strong>b</strong><sub>1 </sub>to match the desired yaw <em>ψ<sub>T </sub></em>. Please refer to Fig. 3. In the following steps we find a triad

Figure 3: Geometry based attitude control. First <strong>b</strong><sub>3</sub><sup>des </sup>is aligned along <strong>F</strong><sup>des</sup>. Then <strong>b</strong><sub>2</sub><sup>des </sup>is chosen to be <em>perpendicular </em>to the plane spanned by the desired yaw heading vector <strong>a</strong><em><sub>ψ </sub></em>and <strong>b</strong><sub>3</sub><sup>des</sup>. This ensures that <strong>b</strong><sub>1</sub><sup>des </sup>and <strong>b</strong><sub>3</sub><sup>des </sup>are <em>in </em>the plane containing <strong>a</strong><em><sub>ψ</sub></em>.

<em>R</em><sup>des </sup>= [<strong>b</strong><sub>1</sub><sup>des</sup><em>,</em><strong>b</strong><sub>2</sub><sup>des</sup><em>,</em><strong>b</strong><sub>3</sub><sup>des</sup>] that has the proper alignment, then proceed to develop a control input <strong>u</strong><sub>2 </sub>that produces the corresponding torque to drive the attitude towards <em>R</em><sup>des</sup>.

As indidicated, the <strong>b</strong><sub>3</sub><sup>des </sup>axis should be oriented along the desired thrust: <strong>F</strong>des

<sub>des</sub>

<strong>b</strong>3 = ||<strong>F</strong>des|| <em>.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(30)

Next, we want the <strong>b</strong><sub>2</sub><sup>des </sup>axis to be perpendicular to both <strong>b</strong><sub>1</sub><sup>des </sup>and the vector <strong>a</strong><em><sub>ψ </sub></em>that defines the yaw direction in the plane (<strong>a</strong><sub>1</sub>, <strong>a</strong><sub>2</sub>) plane:

<strong>a</strong><em> .&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(31)

This can be accomplished by forming the cross product between <strong>b</strong><sub>3</sub><sup>des </sup>and <strong>a</strong><em><sub>ψ</sub></em>:

des&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3des × <strong>a</strong>

<strong>b</strong><sub>2</sub>(32)

<table width="0">
<tbody>
<tr>
<td width="625"><em>R</em>des = [<strong>b</strong><sub>2</sub>des × <strong>b</strong><sub>3</sub>des<em>,</em><strong>b</strong><sub>2</sub>des<em>,</em><strong>b</strong><sub>3</sub>des] <em>.</em>

Next, we need a measure for the error in orientation <em>R</em><sup>des</sup><em><sup>T </sup></em><em>R</em>. The following error vector (see [1])
</td>
<td width="24">(33)</td>
</tr>
<tr>
<td width="625">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <em><sub>R&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </sub></em><sup>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </sup>des<em><sup>T&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </sup></em>− <em>R</em><em>T </em><em>R</em>des)∨

<strong>e </strong>=&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; (<em>R&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; R</em>
</td>
<td width="24">(34)</td>
</tr>
</tbody>
</table>
which guarantees that the plane formed by <strong>b</strong><sub>3</sub><sup>des </sup>and the axis <strong>b</strong><sub>1</sub><sup>des </sup>representing the head of the robot contains the <strong>a</strong><em><sub>ψ</sub></em>. Finally, <strong>b</strong><sub>1</sub><sup>des </sup>is obtained by cross product and the desired rotation matrix is:

2

is obtained from the matrices by taking the ∨ operator that maps elements of so(3) to R<sup>3</sup>. This error vector is zero when <em>R</em><sup>des </sup>= <em>R</em>. It is the rotation vector that generates the error in orientation. Consequently, by applying a torque along its direction it can be decreased, suggesting the control input:

<strong>u</strong><sub>2 </sub>= <em>I</em>(−<em>K<sub>R</sub></em><strong>e</strong><em><sub>R </sub></em>− <em>K<sub>ω</sub></em><strong>e</strong><em><sub>ω</sub></em>) <em>,&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(35)

where <strong>e</strong><em><sub>ω </sub></em>= <em>ω </em>− <em>ω</em><sup>des </sup>is the error in angular velocities and <em>K<sub>R </sub></em>and <em>K<sub>ω </sub></em>are diagonal gains matrices. The desired angular velocities <em>ω</em><sup>des </sup>can be computed from the output of the trajectory generator <strong>z</strong><em><sub>T </sub></em>and its derivatives, but setting them to zero will work for the purpose of this project.

To summarize, the steps to implement the controller are:

<ol>
<li>calculate <strong>F</strong><sup>des </sup>from Eq (28), (27), and (26).</li>
<li>compute <em>u</em><sub>1 </sub>from Eq (29)</li>
<li>determine <em>R</em><sup>des </sup>from Eq (33) and the definitions of <strong>b</strong><em><sub>i</sub></em><sup>des</sup>.</li>
<li>find the error orientation error vector <strong>e</strong><em><sub>R </sub></em>from Eq (34) and substitute <em>ω </em>for <strong>e</strong><em><sub>ω</sub></em>.</li>
<li>compute <strong>u</strong><sub>2 </sub>from Eq (35).</li>
</ol>
<h1>4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; System Description</h1>
<h2>4.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Quadrotor Platform</h2>
For this project we will be using the CrazyFlie 2.0 platform made by Bitcraze, shown in Fig. 1. The CrazyFlie has a motor to motor (diagonal) distance of 92mm, and a mass of 30g, including a battery. A microcontroller allows lowlevel control and estimation to be done onboard the robot. An onboard IMU provides feedback of angular velocities and accelerations.

<h2>4.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Software and Integration</h2>
Position control and other high level commands are computed in Python and sent to the robot via the CrazyRadio (2.4GHz). Attitude control is performed onboard using the microcontroller, though you will control it in simulation.

<h2>4.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Inertial Properties</h2>
Since <strong>b</strong><em><sub>i </sub></em>are principal axes, the inertia matrix referenced to the center of mass along the <strong>b</strong><em><sub>i </sub></em>reference triad, <em>I</em>, is a diagonal matrix. In practice, the three moments of inertia can be estimated by weighing individual components of the quadrotor and building a physically accurate model in SolidWorks. The key parameters for the rigid body dynamics for the CrazyFlie platform are as follows:

<ul>
<li>mass: <em>m </em>= 0<em>.</em>030kg;</li>
<li>the distance from the center of mass to the axis of a motor: <em>l </em>= 0<em>.</em>046m; and (c) the components of the inertia dyadic using <strong>b</strong><em><sub>i </sub></em>in kg m<sup>2</sup>:</li>
</ul>
Note that these constants have already been incorporated into the provided Python simulator.

<h1>5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Project Work</h1>
<h2>5.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Code Packet</h2>
We have provided you with a project packet that contains all the code you need to complete this assignment. The flightsim directory contains the quadrotor simulator; you will not need to make any changes to the enclosed files but you may want to poke around to see how it works under the hood. Inside the proj11 directory you will find two folders: code contains files with code stubs for you to complete for this assignment and util contains a test suite for judging the performance of your controller offline.

The file code/sandbox.py will run the simulator with your controller on the trajectory specified within and produce plots of the state of the quadrotor over time useful for performance tuning as well as an animation of the result. Additionally, a test script (util/test.py) and a few test cases specified as util/*.json files will help you judge the performance of you implementation offline and gain familiarity with the testing system (more on this later). Additionally, at the root of the packet is an important file called setup.py. This file specifies the additional python packages necessary to run the simulator and can be used to automatically install those dependencies in your python environment. For more of this see the piazza post on Python and Pycharm.

Before implementing your own functions, you should first try running code/sandbox.py. It should produce a number of plots displaying useful information about the state of the quadrotor over time as well as a short animation showing the quadrotor in action. Because you haven’t implemented your controller yet you will get an error in the console and the animation will show your quadrotor falling out of the sky. This is because the outputs of the update function in se3control.py are all zeros and thus no thrust is generated.

<h2>5.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tasks</h2>
For this project you will complete the implementation of a controller in se3control.py and a waypoint trajectory generator in waypointtraj.py:

<ol>
<li>waypoint traj.py</li>
</ol>
You will first implement a waypoint trajectory class. This class holds a set of desired waypoints for the quadrotor to visit and subsequently must prescribe a state for each instant in time that if followed by the quadrotor will ensure it visits each point. In particular, you will populate the dict flatoutput containing position (x), velocity (xdot), acceleration (xddot), jerk (xdddot), snap (xddddot), yaw angle (yaw), and angular rate (yawdot). For more information see the doc strings for each function in waypointtraj.py.

<ol start="2">
<li>se3 control.py</li>
</ol>
Next you will implement a controller that drives the quadrotor towards the state specified by the waypoint trajectory class. As mentioned before, this controller will be used throughout project 1. The controller is implemented as a class that holds the physical parameters of the robot and produces motor speed commands (cmdmotorspeeds) given the current time and state of the quadrotor as well as the desired state (flatoutput). For more information see the doc strings for each function in se3control.py.

Although in this phase of the project you will only need to output motor speeds, you should also set the corresponding commanded thrust (cmdthrust), moment (cmdmoment), and attitude (cmdq). Although they will be ignored in the simulator, they can be useful for debugging purposes and will be used when you fly in the lab.

Hints:

<ol>
<li>py ships with a hover trajectory generator built in; use it to first implement and tune your controller then move on to filling out waypointtraj.py.</li>
<li>Make sure that your controller can also handle arbitrary yaw targets, and test that it works! Beware of yaw angle wrap-around.</li>
<li>Tune attitude and position gains separately. Which ones should you do first?</li>
</ol>
&nbsp;
