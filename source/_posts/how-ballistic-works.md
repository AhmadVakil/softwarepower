---
title: Ballistic missiles programming languages and how it works?
date: 2018-07-03T08:27:33.000Z
updated: 2018-07-03T08:27:33.000Z
category:
  - Learning
comments: true
---
**Ballistic missiles programming languages and how it works?**

<p align="center">
  <img width="920" height="600" src="/images/missiles.png" style="border-radius:25px">
</p>

Today with the use of programming, life is easier, and most of the tedious tasks are simplified for us since the computer, or our smart phones helps us in our daily basis life. This simplification can also leave a huge impact on our life on earth which is the use of technology by governments to defend themselves. The most and dangerous technology that is used today by militaries or even terrorism oganizations are ballistic missiles that can target enemies or innocent people far from the launch point. These missiles mostly using C programming languages, C++ and also Ada. These programming languages can be vulnerable if an attacker find an exploit within the system which will end up in controlling the missile by unauthorized people, terrorism organizations or governments. 

Cybersecurity can be used to secure us from cyber attacks. Attackers might try to steal our information inorder to use them for malicious purposes or even find vulnerabilities for an organization and get a prise.

On the other hand, cyber attacks can both secure and insecure our surrounding world. Imagine a terrorist organization that use cyber attacks to take control of military equipments for malicious puposes and on the other side imagine an attacker who tries to stop these malicious activities.

As mentioned, finding and fixing vulnerabilities in military equipments is vital which will also help terrorism organizations to be more secure too if they find the solution on how to fix their current bugs. 

As an example we can think about how a Ballistic missile works and how does it reach its target?

By hacking a missile it is possible to take control of launch time and the target. In order to defend against Ballistic missile, military bases uses satellite technology which consist of an infrared equipped satellite which detect the exact location of the missile and a communication satellite that send/receive data from the infrared satellite to the ground based military with air defence weapon. The interesting part is to estimate exactly the time and the location that the defence rocket reach the ballistic missile in the air which will be calculated using trajectory formula as following.

*****y = h + xtan(α) - gx²/2V₀²cos²(α)*****

****What is the definition of trajectory?****

Trajectory, likewise called a flight way which help us to guess an estimated point. It is the way followed by a moving item with gravity. Typically, the term is used with satellites and moving objects. If an item is fired to a distance target, at that point a parabola is a guess of the direction.

****Example of such:****
- Path of a ping pong ball bouncing while on the air
- Path of a rocket fire to a target while on the air
- Path of a basketball while in the air

<p align="center">
  <img width="920" height="600" src="/images/rocket-launch-2.jpg" style="border-radius:25px">
</p>

****What is the trajectory formula?****
Now we know what is the trajectory, let's dig deeper into the formula:

<p align="center">
  <img width="920" height="600" src="/images/missile-trajectory.png">
</p>

****1- So, motion equations are:****

*****x = Vx * t*****
*****y = h + Vy * t - g * t² / 2*****

****2- We have three Vx, Vy and V₀ form a right triangle, we can write that:****

*****Vx is equal to V₀ * cos(α)*****
*****Vy = V₀ * sin(α)*****

****3- Then, we mix up the equations of motion & velocity components into a single formula:****

*****x = Vx * t => t = x / Vx*****
*****y = h + Vy * t - g * t² / 2 = h + x * Vy / Vx - g * (x / Vx)² / 2*****
*****y = h + x * (V₀ * sin(α)) / (V₀ * cos(α)) - g * (x / V₀ * cos(α))² / 2*****

Sine over cosine is a definition of tangent. So, the final trajectory formula is:

*****y = h + x * tan(α) - g * x² / 2 * V₀² * cos²(α)*****

Following is a video which demonstrate the use of Ballistic missile.

{% youtube 3LPdmxnBkIU %}