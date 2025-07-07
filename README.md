# Effect Of Industrial Zones in Istanbul to Water Consumption and Dam Occupancy Rates
**Analyze whether water consumption in Istanbul and effects of industrial zones in Istanbul to dam occupancy rates.**
Investigate spatial and temporal relationships between:
- Rainfall
- Water consumption
- Dam occupancy
- Industrial district presence

**Dataset Summary / CSV and Shapefiles;**
1. Daily Rainfall and Consumption (2011–2024) – CSB
(Normalized to 2015 – 2023)
2. Daily Dam Occupancy Rates – IBB
(Normalized to 2015 – 2023)
3. District Water Consumption – IBB
(Normalized to 2015 – 2023)
4. Custom-drawn Industrial Zones – OSM + IBB STP Map
5. Barrages in Istanbul Districts (Point Layer)
Final Timeframe: 2015–2023

**Preview of Datasets;**
Daily Rainfall and Consumption
![image](https://github.com/user-attachments/assets/f9a88471-b8bb-4779-a1f2-4f1dc6fe4c21)

Daily Dam Occupancy Rates
![image](https://github.com/user-attachments/assets/edab3820-f686-4441-8f87-65a400d67de7)

District Water Consumption
![image](https://github.com/user-attachments/assets/9506cb7f-d0df-422c-91ff-1daf672319ad)

**Data Preprocessing**
- Daily data aggregated to annual (2015–2023)
- 2023 monthly values summed for yearly comparison
- Industrial shapefile created manually using OSM and official map
- Districts labeled with HASINDUSTRY = 1 or 0
- Tables joined in QGIS

**Industrial Zones in Istanbul with informations**
![image](https://github.com/user-attachments/assets/573ba739-8422-4bee-a128-88891c467875)

**Methodology**
- QGIS spatial analysis (joins, categorized symbology)
- Python used for plotting with Pandas and Matplotlib
- Created annual layers for thematic mapping (2015–2023)
- Comparison plots:
  • Rainfall vs Occupancy
  • Consumption vs Occupancy
  • Industry vs Non-Industry consumption

**Application of Methodology**
- Average values per year computed:
  • Rainfall per dam (Yearly_Dam_Consumption_and_Rain)
  • Occupancy rate (Yearly_Dam_Occupancy_Rates)
  • Total consumption (YEARLYTOTALM3)
- Districts grouped by HASINDUSTRY (1 or 0)
- All visualizations and maps prepared accordingly

**Istanbul Districts' Yearly Consumption - 2015 & 2023 (Other years are included inside of the project package.)**

![image](https://github.com/user-attachments/assets/c9311c55-3ebd-4cfd-a87f-6fd10d51a385)
--------------------------------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/1fd1a61d-a962-43e5-a38b-8d9ab5f0e8fa)



**Disctricts' Consumptions - Industrial vs non-Industrial Zones**
- Industrial districts consume 1.5–2x more water
- Confirms hypothesis that industry increases urban water demand
- Emphasizes importance of spatial industrial planning

![image](https://github.com/user-attachments/assets/ebe60478-80da-45df-815d-4c20ecbacf8f)
![image](https://github.com/user-attachments/assets/58765723-d130-4970-a570-15d230ee5645)


**Consumption vs Occupancy**
- Strong negative correlation observed
- Increased water usage leads to lower dam fill rates

![image](https://github.com/user-attachments/assets/f7c7636c-479f-4cba-91f4-b48f0d930fb0)

**COVID-19 Impact**
- Slight plateau in consumption during 2020–2021
- Due to lockdowns and reduced industrial activity
- Dam occupancy still declined, indicating structural issues

**Rainfall vs Occupancy Rate**
- Rainfall increased over time, but occupancy declined
- Suggests rainfall alone cannot maintain dam levels
- Other pressures (consumption, infrastructure) dominate

![image](https://github.com/user-attachments/assets/33081118-df08-4532-a5aa-ea5a9aafff90)

**Conclusion**  
Rainfall alone is no longer sufficient to maintain Istanbul’s dam levels.  
The primary pressure on water reserves comes from rising consumption, especially in industrial districts where usage is up to 2× higher.  
This confirms that urban water sustainability depends more on consumption control than rainfall amounts.  
Future urban and industrial growth must prioritize regulated, efficient water use, supported by data-driven policies and spatial planning.  










