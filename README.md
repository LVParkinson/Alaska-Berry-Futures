![grafik](https://github.com/LVParkinson/Alaska-Berry-Futures/assets/15371952/8dc6b71e-ad0f-40db-81b5-777d67ffa082)

### [Alaska Berry Futures](https://sites.google.com/alaska.edu/alaska-berry-futures/home) strives to provide current knowledge about northern berry species, expose gaps in our knowledge and inform Alaskans about how we can plan for changing berry resources. 
Berries in Alaska's Changing Climate Series, as of April 2024:
- Cloudberry (*Rubus chamaemorus*)
- Blueberry (*Vaccinium uliginosum*)
- Lowbush cranberry / lingonberry (*V. vitis-idaea*)

Other Alaska Berry Futures resources include: 
- Zotero library
- This repository

## This repository
This repo contains data analysis files related to some of the figures and statements of the above booklets. Most of the analysis was done with python and pandas in jupyter notebooks (.ipynb files) or within excel files. There are three sections:
- The "All statements..." section describes which file(s) relate to a specific comment.
- The "File Descriptions..." section is rather self explanatory
- Errata to be fixed in future updates   

## All statements referencing "Data underlying graphs and climate statements in the Berries in Alaska’s Changing Climate series"

### Cloudberry
> ...and in some parts of Alaska (Yukon-Kuskokwim Delta, Interior) much of the winter precipitation will switch from snow to rain. - page 6

> Concerns about cloudberry plants are mentioned in at least 12 climate adaptation plans from communities across Alaska and are reported by additional communities in Alaska and Canada. - page 12    

- Katie Spellman (klspellman *at* alaska.edu) reviewed climate adaptation plans from across the state for mentions of berries and berry-related concerns. She and Christa Mulder also ran community listening sessions. For more information, please contact her directly.  

> In Scandinavia and Quebec, the addition of honeybees has been shown to increase pollination and fruit set. - page 13

- This is a mistake and should reference: 40; Naess, S. K. & Chagnon, M. Honeybees are useful as pollinators of the dioecious cloudberry, a high-value northern berry. Acta Agriculturae Scandinavica, Section B - Soil & Plant Science 61, 1–7 (2011). 

### Blueberry
> Precipitation during the growing season is expected to increase across most regions of the state... - page 5    

- See section "Precipitation, pollinator success", below

> Increased rain during the pollination period (May or June) may reduce pollination. - page 8    

- See section "Precipitation, pollinator success", below

> Concerns about bog blueberry plants are mentioned in at least 16 climate adaptation plans from communities across Alaska. - page 13

- Katie Spellman (klspellman *at* alaska.edu) reviewed climate adaptation plans from across the state for mentions of berries and berry-related concerns. She and Christa Mulder also ran community listening sessions. For more information, please contact her directly.  

### Lowbush cranberry    
> At least eleven Alaskan communities mention lowbush cranberry in their climate adaptation plans. Many are particularly concerned with changes in the variability of timing and abundance of harvests. - page 4

- Katie Spellman (klspellman *at* alaska.edu) reviewed climate adaptation plans from across the state for mentions of berries and berry-related concerns. She and Christa Mulder also ran community listening sessions. For more information, please contact her directly. 

> **Figure 6** - page 10    
> While most of Alaska is unlikely to get that hot in June, even with climate warming, the Interior may start to see negative effects from high temperatures if no efforts to reduce greenhouse gas emissions are undertaken and temperatures rise as
predicted (Figure 6). - page 11

- See section "Projected June temperatures", below

> Increased rain during the flowering period (June) may reduce pollination because the insects don’t fly in bad weather. In Interior Alaska precipitation in June is expected to increase by ~50% but in other places it is either not increasing or not by very much. - page 13

- See section "Precipitation, pollinator success", below

> However, this is not a big danger: even historical records from Utqiaġvik, Alaska rarely show temperatures this cold in June or July. - page 14

- While we did some investigation, we did not do any new analysis for this statement. It should instead reference the [Alaska Climate Research Center](https://akclimate.org/data/data-portal/)

## File descriptions 

### Berry harvest by community
`2023.02.08_Alaska vegetation harvest 2013-18.ipynb`

**Found in:**
- Cloudberry, map on page 12
- Blueberry, figure 10
- Lowbush cranberry, figure 2

![grafik](https://github.com/LVParkinson/Alaska-Berry-Futures/assets/15371952/b54dba30-648e-423e-a628-76d06c37536a)


Uses vegetation harvest spreadsheets from the Alaska Department of Fish and Game [Commuity Subsistence Information System](https://www.adfg.alaska.gov/sb/CSIS/). For more detail, see the notebook. 

__

### Freeze thaw, winter icing
`2024.02.23_ABF_FreezeThawDays.ipynb`    

**Found in:**    
- Lingonberry, page 11
  > "**Spring icing:** In a study in Sweden, when winter warming melted snow but then froze again to cover the plants in ice for weeks or months two winters in a row there was a significant decrease in the number of flowers.
This is unlikely to be an issue in Southeast Alaska or the Aleutians, but it may be become a problem in some other parts of the state."

Using [Alaska Climate Research Center](https://akclimate.org/data/data-portal/) historical temperature data to investigate freeze thaw days and snow depth in selected locations across Alaska. For more detail, see the notebook.      
  
__

### Precipitation, pollinator success
` 2023.02.16_AK precipitation.ipynb`    

**Found in:**
- Blueberry, page 5
  > "Precipitation during the growing season is expected to increase across most regions of the state"
- Lowbush cranberry, page 13
  > "Increased rain during the flowering period (June) may reduce pollination because the insects don’t fly in bad weather. In Interior Alaska precipitation in June is expected to increase by ~50% but in other places it is either not increasing or not by very much."


Using SNAP precipitation models to look at predicted changes.      
http://data.snap.uaf.edu/data/Base/Other/Community_charts_tool_database/    
https://catalog.snap.uaf.edu/geonetwork/srv/eng/catalog.search#/metadata/b3b9581e-cccc-440f-bb2f-0fd6754d8d41 

![grafik](https://github.com/LVParkinson/Alaska-Berry-Futures/assets/15371952/7860e75c-1d1d-42f4-a366-185d722dcad4)

__

### Projected June temperatures
`2023.02.16_AK temperature.ipynb`  -- TO DO: clean notebook, add comments, add post-processing   

**Found in**    
- Lowbush cranberry, page 10 and 11
  > While most of Alaska is unlikely to get that hot in June, even with climate warming, the Interior may start to see negative effects from high temperatures if no efforts to reduce greenhouse gas emissions are undertaken and temperatures rise as
predicted (Figure 6).

![grafik](https://github.com/LVParkinson/Alaska-Berry-Futures/assets/15371952/1480eaaf-6434-4645-b9fc-685172d93a00)

__


### Wind speed, pollinator success   
`2023.02.16_AK windspeed.ipynb`    

**Found in:**    
This was a preliminary investigation using SNAP [Historical and Projected Hourly Wind Data for Alaskan Communities, 1980-2099](https://catalog.snap.uaf.edu/geonetwork/srv/eng/catalog.search#/metadata/5bdac624-203c-4a65-bfca-1c3f5bf738db). Results from this analysis were not directly referenced in the booklets. Instead, all references to changes in Alaskan wind conditions reference:
> Redilla K, ST Pearl, PA Bieniek, JE Walsh. 2019. Wind climatology for Alaska: historical and future. Atmospheric and Climate Sciences 9:
683-702. [10.4236/acs.2019.94042](https://doi.org/10.4236/acs.2019.94042).

For more information:
- ACCAP [Alaska Community Wind Data](http://windtool.accap.uaf.edu/)
- SNAP [climate tools](https://uaf-snap.org/climate-tools/) and [Github](https://github.com/ua-snap)



## Errata
A running record of typos or other errors to fix during the next round of updates    

### Cloudberry
- Page 13: the statement "In Scandinavia and Quebec, the addition of honeybees has been shown to increase pollination and fruit set." should reference 40- Naess, et al. 2011


### Blueberry

### Lowbush cranberry
- page 2: add LV Parkinson as a contributor to the graphics and photos
- page 14: the statement "even historical records from Utqiaġvik, Alaska rarely show temperatures this cold in June or July." should reference the [Alaska Climate Research Center](https://akclimate.org/data/data-portal/)


