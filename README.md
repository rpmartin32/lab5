# Computer Vision in Remote Sensing Air Pollution


We all use transportation methods in our everyday lives, and although they are incredibly valuable to us, they do carry hidden externalities. One of them being air pollution and this is even more impactful in large urban areas with huge numbers of people commuting every day. To measure potential exposure to this air pollution, originally simple methods were used. By calculating distance from persons to the roadways we could reasonably estimate one’s exposure to air pollution from vehicles. However, with the advent of GIS, our analyses could become more robust and allowing us to more accurately account for traffic density based on time of day as well, amongst other things. It has come to light though, that they may fail to accurately estimate exposure to vehicle emissions specifically, like nitrous oxide and carbon dioxides. 

![traffic-how-close-are-we-to-flying-cars](https://user-images.githubusercontent.com/127624785/233824689-d866c496-06da-40a1-9fe2-3ce31d19ff07.gif)


Scientists have started using machine learning and computer artificial intelligence to assess vehicle specific air pollution more accurately. One study claims that their Python coded machine learning process ConvLSTM (Convolutional Long Short-Term Memory) has a MRE (Mean Relative Error) of 38.9%. This may not sound impressive at first glance, but compared to the 63.2% using the previous Convolutional Neural Network (CNN) model this is a big step forward (Desai, Tayarani, & Gao, 2022). Without going into too much detail about the mathematical steps involved, we can at least visually compare old methods with this new machine learning technique. 

In the image below, the CNN results are on the top and the new ConvLSTM results are on the bottom. We can clearly see much less error indicated in red.

![1-s2 0-S1361920922003315-gr4](https://user-images.githubusercontent.com/127624785/233824503-efece80b-0f04-43bd-b161-b33081dcfec7.jpg)

	
Machine learning is not just useful for air pollution on a local scale, but also at a national or even global scale as well. The EPA, NASA, the Smithsonian Astrophysical Observatory (SOA), and the National Oceanic and Atmospheric Administration (NOAA) collaborated on a satellite named the Tropospheric Emissions: Monitoring of Pollution or TEMPO. TEMPO will have the ability to observe pollutants like nitrogen dioxide, sulfur dioxide and formaldehyde at much higher temporal and spatial resolutions than traditional weather based satellites (U.S. Epa, 2022). It will also allow scientists to better observe how pollutants evolve over hours, days, and even weeks as they interact with changing weather phenomena. 
[](url)
![tempo_1](https://user-images.githubusercontent.com/127624785/233824459-edaecc38-1bd6-4719-be49-5f272be2a631.png)

  
Another way to measure air pollution is through the random forest technique. This technique creates a ‘forest’ of decision trees and uses them to make predictions based on the input features. So a simple forest might have 3 inputs and each input splits into 2 smaller branches, which each branch into 2 more branches which gives us a total of 8 possible choices to choose from for each input.

![Random_forest_diagram_complete](https://user-images.githubusercontent.com/127624785/233825008-c4770763-d8c1-4474-a938-6e31b6a5e4ef.png)

During a study in Poland, it was found that during warmer periods, a random forest produces a better fit than in colder periods. However, this is likely not a universal fit and would differ depending on the climate factors in the study area. In random forest modeling, it was determined that when measuring for nitrogen oxides, the variable with the most importance is traffic flow unsurprisingly since these are expelled from internal combustion engines. When measuring for fine particulate matter (PM2.5), meteorological conditions are most important, particularly wind and temperature because these particles are so small and easily carried through wind flow (Kaminska, 2018). 

![1-s2 0-S030147971830327X-fx1_lrg](https://user-images.githubusercontent.com/127624785/233824816-5d0501a9-cbbd-4fa2-832f-fec0582c509b.jpg)

 
Another method of measuring air pollution is through the development of SVMs or Support Vector Machines. A very simplified explanation of SVMs would be that they divide datasets into two classes that are distinct and unique with a clearly divided separation. However, with data that has a lot of overlap it can be tricky to try and make a clear line of division. During one study in Munich that looked at vehicular air pollution and attempted to predict hourly air pollution, SVM was compared with other classification methods. It found that the SVM would likely work better when working with small amounts of data. A relatively small sample could be enough to build an effective model.  The study also found that ozone can be predicted most accurately, while nitrogen oxides are the hardest to predict. This is likely due to the short lifespan of nitrogen oxides compared to ozone (Humpe, Brehm & Gunzel, 2021).

![tumblr_inline_o9aa8dYRkB1u37g00_540](https://user-images.githubusercontent.com/127624785/233824947-7ffb74bb-52ae-48a8-b917-058222d57179.png)




References:


Desai, S., Tayarani, M., & Gao, H. (2022). Developing Machine learning models for hyperlocal traffic related particulate matter concentration mapping. Transportation Research Part D-transport and Environment, 113, 103505. 

Humpe, A., Brehm, L., & Günzel, H. (2021). Forecasting Air Pollution in Munich: A Comparison of MLR, ANFIS, and SVM. In International Conference on Agents and Artificial Intelligence. https://doi.org/10.5220/0010184905000506

Kamińska, J. (2018). The use of random forests in modelling short-term air pollution effects based on traffic and meteorological conditions: A case study in Wrocław. Journal of Environmental Management, 217, 164–174. https://doi.org/10.1016/j.jenvman.2018.03.094

Support Vector Machines: A Simple Explanation - KDnuggets. (n.d.). KDnuggets. https://www.kdnuggets.com/2016/07/support-vector-machines-simple-explanation.html

TEMPO: A New Era of Air Quality Monitoring from Space | US EPA. (2022, July 6). US EPA. https://www.epa.gov/sciencematters/tempo-new-era-air-quality-monitoring-space
