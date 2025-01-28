# WWA_intersection

This code looks for overlaps in time and space of National Weather Service (NWS) watches, warnings, and advisories. This code work with ArcGIS ArcPro’s python library. This requires a license. Please reach out to Erik Nielsen (ernielsen@tamu.edu) if you have any questions.  

When using a lab computer or device for the first time: 
1.	Open ArcGIS Pro, as you must be signed in before running the code. This code is specifically designed for Esri ArcGIS/ArcPy
2.	Authenticate your ArcGIS Pro. 
3.	Close the graphical user interface.
4.	Download the “AlternativeWorkFlows.tbx” toolbox and place it in the directory you are running the main code it. 

Launching the software:
1.	Open the file browser.
2.	Locate the hard drive on the left side of the screen; click on it. 
3.	Scroll down and open the Python File titled “wwa_intersect_generic_python37”.
4.	Open with favorite editing software.

Data Source:
This code pings the Iowa Environmental Mesonet (IEM) GIS watch/warning/advisory archive here: https://mesonet.agron.iastate.edu/request/gis/watchwarn.phtml

More details here: https://mesonet.agron.iastate.edu/info/datasets/vtec.html 


1. Editing the code:
2.	Edit the script to include the desired inputs. Lines/criteria to edit are listed below.
   
Line 20: year

Line 23: overlap period 

Line 24: overlap period (same as line 23)

Line 27: first product in overlap 

-More information about watch/warning abbreviations used in this portion of the code can be found here: https://github.com/akrherz/pyIEM/blob/main/src/pyiem/nws/vtec.py

Line 29: second product in overlap

Line 122: change product 2; select county(C)/polygon(P)*; watch/warning

-Certain watches/warnings are only polygon based, some are county based, some are both. This depends on year.

Line 124: change product 2; select county(C)/polygon(P)*; watch/warning

3.	Click File → Save (CTRL +S).
4.	Run code using favorite editor/method.
5.	The number returned is the number of overlaps that occurred within your given parameters. 
6.	Close the script window.
7.	Locate the folder that corresponds to the year you’re looking at. (It’ll be titled something like “20XX_all”).
8.	Delete all files at the top that don’t have “final” in the title. 

Examples of Warning Abbreviations

*Polygon warnings: TO (Tornado), FF (Flash Flood), EW (Extreme Wind)

*County warnings: SS (Storm Surge), HU (Hurricane), TR (Tropical Storm) 


