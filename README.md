# 📊 HR Employee Attrition & Burnout Dashboard

## 🎯 Project Overview
This Power BI dashboard identifies critical organizational triggers driving employee attrition. By analyzing workload, compensation, corporate equity, and workplace environment satisfaction, this tool provides HR leadership with actionable data to improve talent retention.


<img width="885" height="498" alt="HR Page 1" src="https://github.com/user-attachments/assets/b921ca3d-b25b-4208-8684-5715effc238a" />

---

<img width="880" height="494" alt="HR Page 2" src="https://github.com/user-attachments/assets/8bde56d2-3fbb-480a-9dba-909c54e7dd46" />


---

<img width="874" height="492" alt="HR Page 3" src="https://github.com/user-attachments/assets/cc06d57e-1c96-43df-9960-a1f7bf467b9e" />


---
<img width="882" height="498" alt="HR Page 4" src="https://github.com/user-attachments/assets/05b87afa-50f6-46f7-b730-d996e077ffac" />


---

## 💡 Deep-Dive Business Insights & UI/UX Strategy

### 1. Overtime Toxicity by Department & Role
* **The Business Insight:** Overtime acts as a massive retention killer, but its damage is concentrated. Field-based teams, Sales Representatives, and specific technical tracks in Research & Development experience aggressive, near-instant attrition spikes when mandatory overtime is introduced compared to back-office support roles.
* **Visual Presentation:** Modeled using a **100% Stacked Bar Chart** tracking `JobRole` on the Axis, `Attrition Rate` as values, and `Overtime (Yes/No)` as the legend.
* **UI/UX Design Feature:** Leveraged an intentional, limited color palette. Non-overtime bars are kept in a neutral light gray, forcing an executive’s eye to immediately isolate the high-contrast hazard color assigned to the overtime risk zones.

### 2. The Career Stagnation Danger Zone
* **The Business Insight:** Attrition peaks heavily for high-performing employees who have stalled in their trajectory. A distinct bottleneck occurs when individuals go **2+ years without a promotion** but hold significant tenure in their current role. These employees feel stagnant and actively seek external opportunities.
* **Visual Presentation:** Modeled using a **Scatter Plot** displaying `YearsSinceLastPromotion` on the X-axis, `YearsInCurrentRole` on the Y-axis, and using bubble sizes to represent the `Count of Attrition`.
* **UI/UX Design Feature:** Implemented adjacent, interactive **Slicers** for `Department`. This allows HR partners to filter by team instantly, reducing cognitive overload and showing exactly where promotion bottlenecks are happening.

### 3. Intersecting Environmental & Job Satisfaction
* **The Business Insight:** Low job satisfaction is manageable if the corporate environment is supportive, but when both metrics degrade simultaneously, retention drops to near zero. Employees scoring both environmental and job satisfaction at **1 or 2 (Low/Medium)** constitute the highest risk group in the organization.
* **Visual Presentation:** Displayed using a multi-dimensional **Matrix Grid** mapping `JobSatisfaction` against `EnvironmentSatisfaction` evaluating the average `Attrition Rate`.
* **UI/UX Design Feature:** Applied conditional formatting with a smooth, dynamic gradient heatmap. The cells only darken when values cross high-risk percentage thresholds, ensuring readability while highlighting problematic data "hot spots."

---

## 🎨 Core UI/UX Framework Applied
* **Data Binning for Clarity:** Instead of plotting continuous variables line-by-line (e.g., individual miles for `DistanceFromHome`), variables are binned into scannable ranges (e.g., 0-5 miles, 6-10 miles). This smooths out messy curves into clear, clean business trends.
* **Text Narrative Integration:** Positioned borderless, clean **Text Boxes** directly beneath high-risk visuals to blend raw charts with instant contextual insights.
* **No-Clutter Layouts:** Information architecture is distributed across theme-specific tabs rather than crammed onto a single screen, respecting the viewer's cognitive load.
