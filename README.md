
# Ephesoon's Portfolio

Welcome to my portfolio! Here you'll find information about my projects, skills, and how to get in touch.

## 🎯 Quick Links
- [About Me](./about.md)
- [My Skills](./skills.md)
- [My Projects](#projects)
- [Contact](./contact.md)

## 📚 Featured Projects

### [Cyclistic Bike-Share Data Analysis](./projects/cyclistic-bike-share/)
In this case study, I analyzed Cyclistic’s bike-share data to understand behavioral differences between casual riders and annual members. Using Python and pandas, I cleaned and processed trip data, calculated ride durations, and grouped usage patterns by rider type, weekday, and bike type.

The analysis showed that casual riders tend to take longer rides, especially on weekends, while annual members mostly use bikes on weekdays with shorter ride durations, indicating commuting behavior. Electric bikes were the most popular choice across both groups.

These insights suggest that casual riders use the service more for leisure, while members rely on it for daily transportation. Based on this, targeted marketing strategies such as promoting membership benefits for weekday riders and offering incentives for casual users could help increase membership conversions.
<img width="1536" height="1024" alt="Capture" src="https://github.com/user-attachments/assets/8d3556a3-7f02-4222-acf8-1caee47754bc" />This dashboard highlights key behavioral differences between casual riders and members. 
It shows that members ride more frequently during weekdays (commuting behavior), while casual riders dominate weekend usage with longer ride durations (leisure behavior). 
This supports targeted marketing strategies to convert casual riders into members.

**Tech Stack:** Python, pandas | **Status:** Completed

---


### [Project 2: Urban Heat Resiliency & Solar Load Modeling](./projects/project-3/)

### [Urban Heat Resiliency Modeling – Overvecht, Utrecht](./projects/urban-heat-resiliency/)
This case study evaluates the urban heat risk for 5,919 buildings in the Overvecht district of Utrecht, Netherlands, to quantify the impact of architectural geometry and greenery on thermal resilience. The process involved a physics-based spatial analysis that calculated total theoretical solar loads while factoring in the "Urban Canyon" effect where heat is trapped between tall structures and the cooling "halos" provided by nature-based mitigation. 

The goal was to support EU climate adaptation strategies by quantifying solar heat absorption in urban environments.

A physics-based spatial analysis of urban heat dynamics in the Overvecht district (Utrecht), quantifying how building geometry, shading, and greenery influence thermal stress.

<img width="639" height="341" alt="pythone map for overvecht" src="https://github.com/user-attachments/assets/c04956da-9f3b-429a-a609-4783214a2a9d" />

<img width="4000" height="2647" alt="Pokecut_1777631448036" src="https://github.com/user-attachments/assets/6d57cc8b-814c-4296-91cf-cd9eb946f767" />





---

##  Overview
This project models the **Urban Heat Island (UHI)** effect across **5,919 buildings** using GIS and physics-based simulation.

- 🌞 Solar Load: **800 W/m²**
- 🏙️ Buildings: **5,919**
- 🌳 Green Buffer: **20m**
- 🌗 Shadow Angle: **45°**

* Note: The dashboard uses average values (13.6m), which hides extreme buildings (33m–36m). 
Further analysis shows that both tall buildings and unshaded mid-rise buildings contribute significantly to heat risk.
<img width="1189" height="590" alt="Capture 3" src="https://github.com/user-attachments/assets/39b8f689-9dac-4eba-9424-9d0fe2799f4e" />

---

##  Key Results

| Metric | Value |
|------|------|
| Total Solar Load | **529,909,196 W (~530 MW)** |
| After Mitigation | **401,257,576 W (~401 MW)** |
| Heat Reduced | **128,651,620 W (24.3%)** |

---

##  Economic Value of Green Infrastructure

- Electricity required to replace trees: **42,883.87 kW**
- Cooling cost savings: **€12,865.16 per hour**

➡️ Urban greenery functions as a **natural power plant for cooling**

---

## 🔍 Key Findings

### 1. Height is the main driver
- Avg height (all): **4.87 m**
- Avg height (high-risk): **13.60 m**
➡️ High-risk buildings are ~**3× taller**

---

### 2. Wall area dominates cooling effects
- Example: **Building 300043630**
  - Wall area: **16,453 m²**
  - Heat: **3.25M W**
  - Still high risk despite shade + greenery

---

### 3. Environmental exposure matters
- Example: **Building 300283598 (12m)**
  - ❌ No shade
  - ❌ No greenery
  - 🔥 Higher heat than taller buildings

---

### 4. Urban canyon effect increases heat
- Tall buildings (>15m) apply **+10% thermal trapping**
- Heat reflects between walls instead of escaping

---

##  Methodology

### Data Pipeline
- OSMnx → building + green space extraction
- Reprojected to **EPSG:28992**
- Cleaned missing values

### Physics Modeling
- Shadow length = height / tan(45°)
- Shadow zones = geometry buffer
- Canyon factor applied for tall buildings

### Spatial Analysis
- Spatial join → detect shading
- Green buffers → evapotranspiration effect
- Fixed join duplication + index issues

### Heat Model
- Base solar load
- Shade → **-50%**
- Green → **-20%**

---


##  Conclusion

The analysis reveals that urban geometry and lack of vegetation are the primary drivers of thermal stress in Overvecht. Key findings include:

Significant Thermal Load: The district faces a total theoretical solar load of 529.91 MW, highlighting the massive scale of energy absorption by the built environment.

Mitigation Success: Existing greenery and shading already provide a 24.3% reduction in heat, saving approximately 128.65 MW of energy.
 
 - 🌳 Nature reduces **24.3%** of heat

The "Height-Risk" Link: High-risk buildings are significantly taller, averaging 13.60m (nearly 3x the district average of 4.87m), which leads to increased surface area for solar absorption.
 
 - 🏢 Tall buildings remain dominant heat sources
 
Economic Impact: Nature-based infrastructure currently saves the equivalent of 43 MW of mechanical cooling every hour, translating to an economic value of €12,865.16 per hour in avoided electricity costs.

- ⚠️ ~401 MW heat still remains

## Recommendations
To further reduce heat risk and improve climate resilience in Utrecht, the following actions are recommended:

- Target the "Top 10": Prioritize the ten most vulnerable buildings identified in the dashboard, specifically those with wall areas exceeding 16,000 m², for immediate retrofitting.

- Expand the Green Buffer: Increase the "Green Buffer Radius" beyond the current 20m in high-risk zones, particularly around Overvecht Centrum, to maximize the cooling "halo" effect.

- Implement Vertical Mitigation: Since wall area dominates heat absorption, focus on vertical greenery and high-albedo (reflective) wall coatings for buildings taller than 12m.

- Address Urban Canyons: For buildings higher than 15m, where the "Canyon Trapping Factor" increases thermal load by 10%, prioritize street-level tree canopies to break the cycle of trapped radiation.

- Nature-First Policy: Integrate nature-based solutions as a primary cooling strategy, as they currently provide a more cost-effective reduction (-20% heat) compared to mechanical alternatives.
 
- Combine **Nature + Engineering solutions**

---

##  Portfolio Value

This project demonstrates:
- GIS + physics integration
- Spatial data engineering
- Climate modeling
- Real-world policy insights

---

### [Project 3: Your Second Project](./projects/project-2/)
A brief description of your second project.

**Tech Stack:** Python, Django, PostgreSQL | **Status:** In Progress

---


### [Project 4: Your Third Project](./projects/project-3/)
A brief description of your third project.

**Tech Stack:** TypeScript, Vue.js, Firebase | **Status:** Completed

---

## 🎓 About
Civil Engineering graduate (Unity University, 2013–2018) with professional experience in construction and engineering roles in Addis Ababa.

**Work Experience:**
- Site Engineer, Rama Construction PLC (June 2019 – May 2021)
- Payment Follow-up, TNT Construction (Aug 2018 – May 2019)

**Courses & Training:**
- Data Analysis (Google, Coursera)
- Python Data Structures (University of Michigan, Coursera)
- Transportation Engineering (Eindhoven University of Technology)
- Calculus Variant A (Eindhoven University of Technology)
- Introduction to Complex Systems (Utrecht University)
- Data Analysis Fundamentals (Udacity)
- Microsoft Power BI (PL-300)
- Advanced Excel, PowerPoint, Data Cleaning

Check out [my full profile](./about.md) to learn more.

## 💻 Skills
Python, Data Analysis, Power BI, Excel, Engineering Fundamentals, Problem Solving, Data Cleaning

[See my complete skill set](./skills.md)

## 📞 Get in Touch
Have a project in mind or want to collaborate? [Let's connect!](./contact.md)

---

*Last updated: April 2026*
