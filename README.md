# APT - Advanced Prevention Traffic System

<p align="center">
  <img src="https://contrib.rocks/image?repo=Eclipse-SDV-Hackathon-Chapter-Two-APT/APT" alt="Contributors" />
</p>

---
## 💪 Challenge : sunken-kitchen
---
## 🌟 Project Overview

Road dangers, like bad weather and careless driving, put lives at risk every day. These dangers don’t just harm individuals—they also cause traffic jams and other problems for society.

**APT** is an **Advanced Prevention Traffic System** that aims to:
- Keep nearby vehicles safe from potential hazards.
- Help authorities respond quickly and effectively to accidents.
- Reduce additional damage by using real-time information.

---

## 🚘 Use Cases

### 🔴 Hit & Run
Hit-and-run accidents are a big problem, making up **24% of the 7,454 crashes reported by NHTSA in 2020**. These accidents can cause traffic chaos and slow down emergency responses. APT helps by:
- Sending alerts to nearby vehicles.
- Sharing important details like the accident location and suggested speeds.

### 🌧️ Bad Weather
Severe weather, like rain, fog, or snow, causes **10% of crashes over 10 years**, according to NHTSA. APT helps drivers stay safe by:
- Suggesting actions like turning on fog lights.
- Showing safe driving tips, such as "No Overtaking."

---

## 🛠️ Project Description

### 📊 System Architecture
![img_architecture](https://github.com/user-attachments/assets/cbb8215a-aea0-4aab-a769-1eb45e296342)

### ✨ Key Application(Velocitas)

#### 🚗 Vehicle-to-Vehicle Communication
- Sends real-time data, like crash details, speed, and weather conditions using **mosquitto MQTT**.
- Uses this information to alert nearby cars about potential risks.

#### 👨‍✈️ Driver Notifications
- **Hit & Run Scenario**:  
  ![Hit Run Case](https://github.com/user-attachments/assets/37c3d149-702a-4e34-867a-1a954a7e6134)  
  1. Alerts nearby drivers about the accident.  
  2. Shows the distance to the accident to avoid congestion.  
  3. Recommends safe speeds to handle emergencies.  

- **Bad Weather Scenario**:  
  ![Weather Alert Case](https://github.com/user-attachments/assets/d2a8ec66-f0d2-43b3-a2f9-90d14e0c05ec)  
  1. Suggests turning on fog lights for better visibility.  
  2. Advises drivers to slow down and drive carefully.  
  3. Displays traffic rules, like "No Overtaking."
---

## 🚔 WebApplication for Authorities
![img_web](https://github.com/user-attachments/assets/42a1e2df-d38f-4afa-b1e1-ecec047e0468)

- Collects data from vehicles via **eclipse mosquitto**  to find dangerous areas and get an optimized route to the accident areas.
- Gives clear information, like the best routes, to help emergency teams respond faster.

---

## 🎮 Simulations via **eclipse SUMO**  
![carcrash_simulation](https://github.com/user-attachments/assets/3b140131-4ab6-4459-a4f3-d21b1da36fd5)
- Using SUMO, we visualized the entire flow of the APT system applied in the real world.
- Assume a specific situation : Hit & Run
    - Red Car: Offender / Green Car: Victim / Blue Car: Police
1. Red and green vehicles collide at an intersection
2. Collision message(event) sent
3. Police car (blue) receives message and creates optimal route
4. Police car (blue) tracks the fleeing vehicle(red) in real time.
---


## 🧑‍💻 Team Members
- Soonwoong Kim
- Hanbin Yeo
- Wonjeong Lim
- Eunji Lee
- Seungjoo Kim

---

## 🤝 Contributors
<a href="https://github.com/Eclipse-SDV-Hackathon-Chapter-Two-APT/APT/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Eclipse-SDV-Hackathon-Chapter-Two-APT/APT" alt="Contributors" />
</a>



