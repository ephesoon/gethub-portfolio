
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
A data-driven urban climate project focused on analyzing how city structure and green spaces influence heat accumulation. The goal was to support EU climate adaptation strategies by quantifying solar heat absorption in urban environments.

A physics-based spatial analysis of urban heat dynamics in the Overvecht district (Utrecht), quantifying how building geometry, shading, and greenery influence thermal stress.
* Note: The dashboard uses average values (13.6m), which hides extreme buildings (33m–36m). 
Further analysis shows that both tall buildings and unshaded mid-rise buildings contribute significantly to heat risk.
<img width="941" height="421" alt="Capture2" src="https://github.com/user-attachments/assets/982bf66d-0979-4726-b77a-28b50811d037" />
<img width="1024" height="682" alt="Overvecht solar radation distribution to be uploaded for get hup" src="https://github.com/user-attachments/assets/62407002-60e8-4535-bc36-fb3f5ba18a19" />




---

##  Overview
This project models the **Urban Heat Island (UHI)** effect across **5,919 buildings** using GIS and physics-based simulation.

- 🌞 Solar Load: **800 W/m²**
- 🏙️ Buildings: **5,919**
- 🌳 Green Buffer: **20m**
- 🌗 Shadow Angle: **45°**
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
![Uploading 8fa5529f-0593-4f2c-a847-2a9e5599f594.png…]()

##  Conclusion

- 🌳 Nature reduces **24.3%** of heat
- 🏢 Tall buildings remain dominant heat sources
- ⚠️ ~401 MW heat still remains

### Recommendation:
- Trees → exposed buildings
- Reflective materials → tall buildings
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
