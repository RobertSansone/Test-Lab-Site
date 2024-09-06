---
layout: default
---
# Breakerspace SEM Tutorial

## Overview

The Breakerspace has two scanning electron microscopes (SEM), a ThermoFisher [Phenom XL](https://www.thermofisher.com/us/en/home/electron-microscopy/products/desktop-scanning-electron-microscopes/phenom-xl.html) and [Phenom Pure](https://www.thermofisher.com/us/en/home/electron-microscopy/products/desktop-scanning-electron-microscopes/phenom-pure.html). 

[SEMs](https://www.thermofisher.com/blog/materials/what-is-sem-scanning-electron-microscopy-explained/) use a focused beam of electrons to image materials at much higher magnification than can be achieved with an optical microscope, with our instruments able to resolve features as small as 100 nm in optimum conditions. 

Our Phenom XL has a large 100x100 mm sample stage, a low vacuum mode for non-conducting samples, can perform [energy dispersive spectroscopy (EDS)](https://www.thermofisher.com/blog/materials/edx-analysis-with-sem-how-does-it-work/), and also has a [tensile stage](https://assets.thermofisher.com/TFS-Assets/MSD/Flyers/desktop-sem-tensile-sample-holder-FL0116.pdf) for in-situ observation of mechanical experiments. The Phenom Pure can observe a single sample on an 18 mm or smaller stub, under either low or high vacuum, and has a cold-stage for observation of frozen samples. Both instruments have [backscatter (BSD) and secondary electron (SED) detectors](https://www.thermofisher.com/blog/materials/sem-signal-types-electrons-and-the-information-they-provide/).

### Index:

* [Standard operating protocol](#sop) - ([startup](#startup), [operation](#operation), [shutdown](#shutdown))
* [Materials and sample prep](#materials)
* [Detailed operating instructions](#details)
* [Data processing and analysis](#data)
* [Common failure modes](#failures)
* [Manufacturer manuals](#manuals)
* [Links](#links)
* [Exercises](#exercises)

<a name="sop"></a>
### Standard operating protocol:

<a name="startup"></a> 
#### Instrument startup:

* Log on to instrument workstation using your MIT Kerberos
* Start the Phenom User Interface software
* Wake the instrument up if needed
	* The first time you log on, and occasionally thereafter, you may need to connect to the instrument in [Settings/Phenom/Status](../assets/img/tutorials/SEM/connect.PNG)

<a name="operation"></a> 
#### Operation:

* Wear nitrile gloves when handling your sample, sample stages, and other sample preparation components
* [Prepare samples](#prep) externally at the sample prep table* [Load](#loading) your sample(s) into the instrument
* Remove your gloves while using the computer
* Perform [characterization](#characterization) relevant to your sample (image capture, measurement/annotation, EDS)
* Wear nitrile gloves
* Unload samples
* Repeat as needed

<a name="shutdown"></a> 
#### Instrument shut down:

* Close the software - press F11 to switch out of fullscreen view
* Log off Windows
* The instrument will put itself in standby

<a name="materials"></a> 
### Compatible materials and sample prep:

* Samples should be free of volatiles (dry), excepting samples to be frozen on the Phenom Pure cold stage
* Samples must be free of loose particles ("flush" with compressed air)
* Samples must be well secured to a sample stub 
* Non-conductive samples can be viewed in low vacuuum mode, or sputter coated
* _Phenom XL_ maximum sample size is 100mm x 100mm x 35mm
* _Phenom Pure_ maximum sample size is a cylinder about 18mm diameter and 12mm tall

##### _If you have any questions about whether a material is appropriate to characterize in the Breakerspace, please ask before bringing it to the lab._

<a name="prep"></a>
#### Sample prep basics:

* Prepare samples externally at the sample prep table
* Firmly attach samples to stub
* Remove loose debris with compressed air

#### Solid sample prep (basic)

* Place a bare sample stub in a sample tray __ADD IMAGES__
* Attach a double-sided carbon pad to the stub
* Attach the sample to the pad
* For an expanded discussion of sample prep techniques, see page 15 of [the manual](https://www.dropbox.com/scl/fi/iyd538gtkj79kg0bc8113/2020-MS-Phenom-XL_User-Manual.pdf?rlkey=0yk985nvgz3lckqnrtxwo7afv&dl=0)

<a name="details"></a> 
### Detailed operating instructions: 

<a name="loading"></a>
#### Sample loading:

* Remove sample stage from the microscope (or drawer for _Phenom Pure_)
* _Phenom XL:_ sample compartment is opened by pressing eject button in the software
* _Phenom Pure:_ sample compartment is manually opened and closed, but must be unlocked with the eject button in the software
* Using stub tweezers, push pin on stub into a hole in the sample stage
* _Phenom Pure:_ black stage sets instrument in high vacuum mode, gray stage sets instrument in low vacuum mode for charge reduction on non-conducting samples
* Set proper sample height
* _Phenom XL:_ set the tallest part of your tallest sample level with the opening of the sample stage, then lower by 6 notches on the dial
* _Phenom Pure:_ the tallest part of the sample should be just lower than the top edge of the sample stage
* Load the sample stage into the instrument
* Close the door and your sample should be visible in the NavCam

<a name="loading"></a>
#### Characterization:

__Customize:__ When your sample is loading, this is a good time to visit [Settings/Customize](../assets/img/tutorials/SEM/customizer.PNG) and change the _Label_ and _Location_ fields to a name and folder that are relevant to your project

__NavCam:__ When you first load a sample into the SEM you see your sample(s) on the [NavCam](../assets/img/tutorials/SEM/navcam.PNG). This is an optical image of the sample stage that can be used for navigation once you are in SEM observation mode. If you will rely on the NavCam image for navigating your sample(s), it is helpful at this stage to make sure the brightness, contrast, and focus are all acceptable in key areas of your sample. If you wish, you can click the camera icon in the NavCam to save the NavCam image to a file.

__LiveSEM view:__ Once you click "Move to SEM" __add image__ you will be in the LiveSEM view. Here you can adjust brightness, contrast, and focus, as well as changing magnification. The recommended UI setup is to leave the scroll wheel set to change magnfication, hold down the right mouse button and move the mouse cursor horizontally to change focus, and to use auto brightness/contrast. A full set of keyboard and mouse shortcuts can be found in [Settings/Phenom/Help](../assets/img/tutorials/SEM/shortcuts.PNG). Detailed operating instructions and a full UI overview can be found starting on page 20 of either the [_XL_](https://www.dropbox.com/scl/fi/iyd538gtkj79kg0bc8113/2020-MS-Phenom-XL_User-Manual.pdf?rlkey=0yk985nvgz3lckqnrtxwo7afv&dl=0) or [_Pure_](https://www.dropbox.com/scl/fi/7ju8ldfdm0p04m6n81men/Phenom-ProX-G6-User-Manual.pdf?rlkey=l6gg1ld4zpmtxgrsxfgw00jpb&dl=0) manual.

__Gallery:__ The gallery will show you all images in the active folder. In addition to reviewing the images, you can add dimensions and notes. If you annotate the images the annotated versions need to be saved as new files.

__Acquisition:__ Press the camera icon on the left side of the screen to acquire an image. Images will be saved in the resolution and with the averaging specified in the Operational Settings/Acquisition menu. Pay attention to acquisition times, and take some test images first. Higher averaging settings swill increase signal to noise, and result in cleaner images, but longer acquisition times. If there are issues related to charging, such as drift, they will be more visible in longer acquisitions, so higher averaging is not always better or needed. 

__EDS:__ [Energy dispersive spectroscopy (EDS)](https://www.thermofisher.com/blog/materials/edx-analysis-with-sem-how-does-it-work/), available on the _Phenom XL_, allows you to perform elemental analysis and save out full reports, included map images, images and data of captured spectrum, and a CSV files with raw data. Recommended settings for EDS are 15kV acceleration voltage and map beam intensity. Click the square to stop data collection before navigating to a different section.

__Live EDS:__ Live EDS mode, (_Phenom XL only_) lets you perform quick elemental analysis on a spot on your sample, without generating any files or documentation. It is useful for quick spot checks. Recommended settings for EDS are 15kV acceleration voltage and map beam intensity. Click the square to stop data collection before navigating to a different section.

_For a more complete description and instructions on how to use any of these features, please see the_ [_XL_](https://www.dropbox.com/scl/fi/iyd538gtkj79kg0bc8113/2020-MS-Phenom-XL_User-Manual.pdf?rlkey=0yk985nvgz3lckqnrtxwo7afv&dl=0) or [_Pure_](https://www.dropbox.com/scl/fi/7ju8ldfdm0p04m6n81men/Phenom-ProX-G6-User-Manual.pdf?rlkey=l6gg1ld4zpmtxgrsxfgw00jpb&dl=0) _manuals._

<a name="unloading"></a>
#### Sample unloading:

* Open the sample compartment
* Remove sample(s)
* _Phenom XL:_ return sample stage to sample compartment, close door
* _Phenom Pure:_ close door, place sample stage in drawer


<a name="failures"></a>
### Common failure modes:

* _Phenom XL:_ If the SEM fails to start press the eject button to open and close the door and reinitialize the sample loading process
* _Phenom XL:_ In either live EDS or EDS, if you do not press the stop button, and attempt to return to observation mode, you will get an error message, and need to return to where you were and press stop **add image/gif**
* Sensitive sample may experience [degredation]](https://www.thermofisher.com/us/en/home/materials-science/learning-center/applications/sample-degradation-scanning-electron-microscope-sem.html), often in the form of cracks on the surface, or the sample may appear to be melting or boiling. Lowering acceleration voltage, beam intensity, and magnification will all help slow the rate of degredation.

<a name="manuals"></a> 
### Manufacturer's manuals:

* software manual
* hardware manual

<a name="links"></a>
### Links:

* good video tutorials, etc.

<a name="exercise"></a> 
### Exercises:

* intro for anyone - eg honey bee on optical
* beginner exercise for course 3 subjects - identify and measure types of grain in metal sample, 
* advanced exercise - deconvolution of compound sample from spectrometer, etc.

