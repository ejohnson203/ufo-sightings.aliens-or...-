# UFO Sightings: Aliens or Nah?

## “The question is not: ‘Are UFOs real?’  People are definitely seeing something. The question is ‘What exactly are they seeing?’”

### [Slide Deck](https://docs.google.com/presentation/d/e/2PACX-1vSQP2O1tZs_WlLXEigUU7uO2XQASWW_L4ezkbtBI_D2iOWUYK3-2SnWgfUYF4ru1-X0WhnQIEtX1AqV/pub?start=false&loop=false&delayms=3000&slide=id.g21477ba79ef_2_190)

Project Idea

Have you ever seen something unexplainable in the sky? Is the human race in imminent danger of an alien invasion? Should you invest in an aluminum foil hat? 

Are UFOs really some form of alien visiting Earth or is that just a myth? The more common theory is that UFOs have mundane explanations. Planes, balloons, clouds,  or celestial objects, like meteors and planets. Government investigations, developed due to concerns about national security, have not yielded any evidence of alien spacecraft. Skeptics point to flaws in videos, errors in sensors, and the unreliability of eye witness testimony. Yet practitioners of UFOlogy argue that there are phenomena for which there is no earthly explanation. 

The National Unidentified Flying Object Reporting Center, or NUFORC, was founded in 1974 by UFO investigator Robert J. Gribble. The Center’s primary function over the past five decades has been to receive, record, and to the greatest degree possible, corroborate and document reports from individuals who have been witness to unusual, possibly UFO-related events. Throughout its history, the Center has processed over 170,000 reports. This project focuses on 80,000 records from 1906-2014.

This project digs into the facts to see if there is any proof that ties reported UFO sightings to extraterrestrial beings.

## Research Questions
#### 1. When do most sightings occur? (Year, month, day, time?)
#### 2. Are there any similarities in shape?
#### 3. Do celestial objects such as meteorites or the Moon play any significance?

## Data Sources

### UFO Sightings Report Data Source
[UFO Sightings](https://www.kaggle.com/datasets/NUFORC/ufo-sightings)

### Meteorite Landings Data Source
[Meteorite Landings](https://www.kaggle.com/datasets/ulrikthygepedersen/meteorite-landings)

### Lunar Phase Data Source
[Lunar Phases](https://www.kaggle.com/datasets/jodiemullins/1900-2022-primary-moon-phases-utc7-timezone)


## Data Cleaning
In Python for UFO Sightings dataset, split datetime column into  year, month, day, hour, and minute.
Used newly created month and hour to generate bins for seasons and time of day, respectively. 
Fill missing values for country using a dictionary for US states and Canadian Provinces.
Fill missing values for state and other countries with GeoPandas using geographical coordinates.
<br>
In Python for Meteorite Landing Data, remove rows with null values for year or geolocation. 
Split geolocation data into coordinate columns to be processed with GeoPandas.

## Compiling Data
In Python for meteorite landings and UFO sightings, used GeoPandas to plot all coordiates on a world maps.
According to NASA, something burning in the atmosphere can be witness from a radius of approximately 1100km away.
Compared both maps to generate a new map with coordinates that are within that radius and occured at the same time.
![image](https://github.com/ejohnson203/Pics/blob/4dcf40b08e7f72ed53f219cd353487c145704638/UFO%202%20Maps.png)


## Research Questions & Findings
### [Slide Deck](https://docs.google.com/presentation/d/e/2PACX-1vSQP2O1tZs_WlLXEigUU7uO2XQASWW_L4ezkbtBI_D2iOWUYK3-2SnWgfUYF4ru1-X0WhnQIEtX1AqV/pub?start=false&loop=false&delayms=3000&slide=id.g21477ba79ef_2_190)

#### 1. When do most sightings occur? (Year, month, day, time?)
Sightings have been reported way more frequently in the more recent decades as technology improves, especially aerial technology. Sightings are way more likely to occur during the warmer months, around holidays where fireworks are used to celebrate, and at night.

#### 2. Are there any similarities in shape?
Some form of light is the most common sighting making up 1 in 3 of all reports.
<br> ![image](https://github.com/ejohnson203/Pics/blob/13fb2fa7819d0f9e0b61f1905b404a01b9c3a059/UFO%20Shape.png)
#### 3. Do celestial objects such as meteorites or the Moon play any significance?
Meteorite landings explains 3% of sightings. If meteorites explain this amount of sightings, the number of other sightings that can be explained by the numerious celestial objects is very likely. 
Sightings are disproportionately more likely to occur during new moon
![image](https://github.com/ejohnson203/Pics/blob/13fb2fa7819d0f9e0b61f1905b404a01b9c3a059/UFO%20Overlay.png)

## Conclusion
There's a fascinating frailty of the human mind called "argument from ignorance." Here’s what I mean... 
Let’s say you see lights flashing in the sky. You've never seen anything like this before and don't understand what it is. You point and say, "It's a UFO!" Remember the "U" stands for "unidentified." But you say, "I don't know what it is; it must be aliens from outer space, visiting us from another planet." The issue here is that if you don't know what something is, your interpretation of it should stop immediately. You don't then say that it must be X or Y or Z. That's argument from ignorance. It's common. It’s not our fault, it’s part in human psychology; it may relate to our burning need to manufacture answers because we feel uncomfortable about being steeped in ignorance.
<br>
UFOs do require investigation, which most often leads to identification, and not as evidence of some extraterrestrial technology. 
