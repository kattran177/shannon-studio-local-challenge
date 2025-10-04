# The Bio-AI Water Guardian: Making the Invisible Visible

## Mapping the Invisible Microplastic Threat in the Shannon

### Summary

The River Shannon is essential to our nation, but people living nearby are really worried about its ecological health. Recent reports confirm that pollution is causing serious damage to the river's biodiversity, especially to important species like the threatened Shannon salmon. This pollution comes from a few places, mainly agricultural runoff and city wastewater.

Local research institutions, like the University of Limerick (UL) and our TUS research hub, are working hard to solve one specific problem: figuring out how to find and measure microplastics in the river. They are using super high-tech methods like Scanning Electron Microscopy (SEM) and Raman/FTIR spectroscopy, and they're even incorporating Machine Learning to help with the analysis.

This lab work is a huge step forward, but we need to move it out into the real world. A genuinely sustainable solution requires scaling this complex analysis beyond the lab. Right now, the data about pollution, regarding its location, its existence, and origin, is too separated, too slow to collect, and often too expensive for local communities and regulators to use effectively.

We need to address this challenge by bringing together the analytical power of our local university research with the global reach of space data and AI. This would let us build an open, transparent, and proactive system for tracking pollution, inspired by the spirit of collaboration found in the NASA Space Apps community.

---

### Background

The River Shannon, which is the longest in Ireland, is currently facing a huge problem with microplastics and nutrient pollution. This contamination seriously threatens keystone species like the Atlantic Salmon. These fish are essential to the river's ecosystem and their health is a clear signal that the river is struggling.

Microplastics are small plastic pieces, less than 5 millimetres in diameter, that are now everywhere. They are considered a pervasive pollutant because they show up in our air, food, and drinking water globally.

For the environment, this is a major issue because microplastics can travel over huge distances and get transferred up through food chains in ecosystems. Even worse, these plastic particles act like tiny sponges, picking up other harmful substances like toxic chemicals and heavy metals. These chemicals often include additives used to make the plastic, and they are known to be toxic to animals and humans.

In terms of human health, we are exposed when we breathe them in or consume contaminated food and drinks. When microplastics are ingested, those toxic chemical compounds can leach out into our bodies. Although researchers are still gathering evidence to fully understand the long-term health risks from exposure at environmental levels, the scientific community agrees that the potential risks to both humans and ecosystems are serious, and we need urgent policy changes to reduce their release.

---

### Objectives

Our main objective is to design and build the foundational software and data framework for a tool we can call the **Bio-AI Water Guardian**. This could become a core resource for the TUS research hub or serve as a starting point for future collaborative hackathons.

This project focuses on four key architectural challenges:

#### 1. Developing a Simulated AI Classification Pipeline

We need to figure out how to design the architecture for a **Machine Learning Classification Model**. This model, maybe a simple Neural Network or a Random Forest, has to be able to take in basic, simplified data, similar to simulated spectral signatures or sensor readings, and instantly categorise the pollution. This means the AI must accurately identify the pollutant, classifying things like the type of microplastic, whether there's high-nitrogen runoff, or if *E. Coli* is present.

#### 2. Integrating NASA Water Quality Proxies

The pollution data from our local sensors needs to be verified and enhanced by global data. We have to show how our AI-detected pollution spots would be improved by using **NASA or ESA satellite imagery**. This involves finding and using publicly available space data, such as images from **Landsat 8/9** or **Sentinel-2** available through NASA Earthdata and the National Centres for Environmental Information- Marine Microplastic Concentrations. The core challenge here is correlating the AI-identified pollution hotspots with things the satellites can see, like **turbidity** (how cloudy the water is) and **chlorophyll levels** (which indicate algae blooms).

#### 3. Prototyping a Real-Time Data Visualisation Interface

We have to build a simple, easy-to-use **web dashboard**. This interface should take the data that the AI has classified and project it onto a dynamic map of the Shannon River Basin. The map needs to be interactive, letting a user filter the data by the type of pollutant and its concentration. It also needs to provide a link back to the originating research data, like the original spectral signature, for transparency.

#### 4. Conceptualising a Source Tracing Model

Finally, we need to outline the data inputs required for a component that could trace the pollution back to its origin. This is a complex challenge. To do this, we'd need to bring in external data like **NASA SRTM** or **ASTER Digital Elevation Models** to understand the terrain and water flow. By integrating this with local flow models, we could potentially trace the pollution plume back to the most likely specific source, such as a particular drain or area of agricultural runoff.

---

### Potential Considerations

When building a system like the Bio-AI Water Guardian, there are several major design and technical questions that need to be addressed. These areas are vital for making sure the platform is useful, sustainable, and capable of growing.

#### 1. Integrating Citizen Science and Community Data

The core challenge is figuring out how to successfully bring local communities into the scientific process. We need to explore how to design the system's architecture and protocols so it can easily take data from **low-cost, open-source hardware**. Could the system accept input from simple devices like **Arduino or Raspberry Pi-based spectrophotometers** that local schools or community groups might use? This is essential for ensuring the AI model has enough real-world, decentralised data to learn from.

#### 2. Utilising AI for Policy and Context

How can we use advanced computing to give pollution data historical and regulatory context? We should explore using **Natural Language Processing (NLP)** to automatically scan and analyse documents like local council minutes and environmental reports. This would allow the system to automatically identify areas that already have a known risk, such as reports of **sewage overflow** or recurring **agricultural compliance issues**, helping to prioritise where the system should focus its attention.

#### 3. Designing for Future Cloud Scalability

Looking ahead, the system will need to handle a huge volume of real-time data from sensors across the entire river basin. The question is: how would the **Cloud Computing architecture** need to be designed? We must consider solutions for the data ingestion pipelines and database choices that are not only cost-effective today but also fully capable of scaling up to handle **petabyte-scale information** in the future.

#### 4. Creating a Research Feedback Loop

To make this a true ecosystem, we have to ensure the data flows both ways. How can the platform provide the cleaned, classified, and mapped data back to the researchers at the TUS hub? Giving them this refined information would help them continuously improve and refine their **laboratory-based Machine Learning models**, solidifying the relationship between the academic lab, the cloud system, and the community.

#### 5. Ensuring Transferability and Broad Utility

Finally, we need to think about future growth. Could the core **AI classification model** be trained to detect other important pollutants beyond just microplastics? We should consider the architectural changes needed to allow the system to identify things like **pharmaceutical residues or heavy metals**, which would significantly broaden the use case of the entire platform for future environmental projects.

---
### Difficulty Level

This problem statement is suitable for intermediate to advanced levels, considering it requires the participants to grasp the concept of Machine Learning to confidently tackle this challenge.

### References

1.  [https://www.ul.ie/node/85167](https://www.ul.ie/node/85167)
2.  [https://www.limerickpost.ie/2025/05/31/water-water-everywhere-but-none-for-the-shannon-salmon/](https://www.limerickpost.ie/2025/05/31/water-water-everywhere-but-none-for-the-shannon-salmon/)
3.  [https://www.sciencedirect.com/science/article/pii/S2405844023015669](https://www.sciencedirect.com/science/article/pii/S2405844023015669)
4.  [https://www.bbc.com/future/article/20250723-how-do-the-microplastics-in-our-bodies-affect-our-health](https://www.bbc.com/future/article/20250723-how-do-the-microplastics-in-our-bodies-affect-our-health)
5.  [https://med.stanford.edu/news/insights/2025/01/microplastics-in-body-polluted-tiny-plastic-fragments.html](https://med.stanford.edu/news/insights/2025/01/microplastics-in-body-polluted-tiny-plastic-fragments.html)
6.  [https://www.sciencedirect.com/science/article/pii/S2950305124000214](https://www.sciencedirect.com/science/article/pii/S2950305124000214)
7.  [https://www.eea.europa.eu/en/european-zero-pollution-dashboards/indicators/impacts-of-microplastics-on-health-signal](https://www.eea.europa.eu/en/european-zero-pollution-dashboards/indicators/impacts-of-microplastics-on-health-signal)
8.  [https://www.ncei.noaa.gov/products/microplastics](https://www.ncei.noaa.gov/products/microplastics)
