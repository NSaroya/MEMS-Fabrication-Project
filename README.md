The project was undertaken as a component of ECE 457, focusing on Microfabrication and Devices, within the nanoFAB - Fabrication and Characterization Facility - located in Edmonton.

# Objective
The project aimed to fabricate and test a variety of *micro-electro-mechanical systems* (MEMS) using standard fabrication and characterization techniques. These include simple spring and beam structures, small drives, extended-needle gauges, large drives, resistance gauges, inch-worm gears, smooth movers and many more. The main fabrication techniques used in this lab are photolithography, anisotropic etch of Si using the Bosch process in the RIE system and etching of the SOI layer by VHF etching. 

Among various fabricated structures, the comb drive is a basic building block which is one of the various methods used to actuate MEMS devices. A Comb drive consists of a series of interdigitated teeth. Comb drives actuate by utilizing the electrostatic force generated by the oppositely charged comb teeth in the drive to move one set of teeth relative to the 
other. While comb teeth must overlap to initiate the attraction, a large overlap is undesirable because this will restrict the range of motion of the combs. The anchored spring suspensions provide the restoring force for the movable combs to return to their original positions. Since the device is planar, the springs and the linear motion occur in the same plane.

# Introduction
## MEMS
The origin of the field of MEMS is largely attributed to physicist Richard P. Feynman who presented, in 1959 to the American Physical Society, his visionary speech entitled “There’s plenty of room at the bottom”. Since then, great strides have been made in miniaturisation technologies and techniques that have allowed the fabrication of MEMS to be possible.

MEMS refer to devices that have a characteristic length between 1 µm and 1 mm and integrate electrical and mechanical components. The field of MEMS is known by a variety of other names: micromechanics, microsystems technology (MST), micro-machines, microactuators. The study of MEMS is a rapidly emerging field that plays an important role in the microelectronics industry. MEMS fill a vital niche by creating devices that would be too large and costly or even impossible to make using traditional integrated circuit (IC) electronics: devices such as optical switches and relays.

MEMS are traditionally fabricated onto a substrate or wafer that may also contain the electronics required to interact with the MEMS device. One type of substrate is the *silicon-on-insulator* (SOI) wafer. SOI MEMS are planar devices that consist of three layers: a top Si *device layer*, a middle SiO2 layer, and a bottom silicon base layer. After processing, sections of the Si device layer hover over the silicon base layer, allowing for movement; this is accomplished by removing portions of the SiO2, which we deem a *sacrificial layer*. The SiO2 that has not been removed anchors immobile sections of the device layer to the silicon base layer. One type of MEMS device is a *comb drive*, which uses electrostatic attraction between oppositely charged combs to mechanically actuate the device

## SOI Wafer
Silicon-on-insulator (SOI) wafers consist of three layers: a 20 µm Si device layer, a 2 µm buried-oxide (BOX) SiO2 sacrificial layer, and a ∼500 µm Si handle wafer. The thickness of these layers varies depending on the devices being fabricated. The Si device layer is patterned and etched to create MEMS devices, while parts of the sacrificial SiO2 layer are etched using buffered oxide etch (BOE) to release the MEMS for actuation. The unetched SiO2 anchors the MEMS to the handle wafer, providing electrical isolation for the two silicon layers. Different methods are used to produce SOI wafers, including SIMOX, wafer bonding, Smart Cut, NanoCleave, and ELTRAN, which involve processes like ion implantation and controlled exfoliation. SOI wafers offer advantages such as reduced power consumption, increased speed, and improved manufacturing processes, making them valuable in MEMS and CMOS integrated circuit fabrications.

<div align="center">
  
![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/35e951c0-0927-41cb-99bc-dc1fb96397d0)
</div>

<p align="center">
  <strong>Figure 1:</strong> Silicon-on-insulator wafer layers. From bottom, a handle wafer (base layer), a sacrificial layer in the middle, and the top device layer.
</p>

## Comb drive actuation
The comb drive is one of the basic building blocks of MEMS. It is one of the various methods used to actuate MEMS devices. A comb drive consists of a series of interdigitated teeth. Comb drives actuate by utilizing the electrostatic force generated by the oppositely charged comb teeth in the drive to move one set of teeth relative to the other. While the comb teeth must overlap in order to initiate the attraction, a large overlap is undesirable because this will restrict the range of motion of the combs. One set of the comb teeth are anchored down to the wafer while the other set is mobile and attached
to anchored spring suspensions. The anchored spring suspensions provide the restoring force for the movable combs to return to their original positions. Since the device is planar, the springs and the linear motion occur in the same plane.

<div align="center">
  
![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/5f76562d-7613-41f9-95b4-bac48ebebc45)
</div>

<p align="center">
  <strong>Figure 2:</strong> Comb drive actuation. At right is an SEM image showing a close-up view of the comb drive teeth.
</p>

## Coulombic attraction analysis 
The electrostatic force of the comb drive depends on numerous factors: the voltage applied, the number of comb fingers, the amount of overlap between comb fingers, the size of the gaps separating the fingers, and the thickness (height) of the combs.

The inherent linearity of the electrostatic comb drive structure allows for the application of relatively straightforward first-order, two-dimensional theory to determine an accurate approximation of the induced electrostatic force.
 
<div align="center">
  
![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/b9d6ce03-f18d-448a-af48-6f13a97038f6)
</div>
<p align="center">
  <strong>Figure 3:</strong> Comb drive showing the device dimensions of interest
</p>


## Stiction
The use of sacrificial layers is a common technique in creating MEMS. The removal of the sacrificial layer yields a free-standing structure capable of movement. However, a serious problem can arise during the removal of the sacrificial layer: when the SiO2 layer is less than 10 µm, surface tension becomes a major issue. Stiction is short for static friction and is caused by capillary forces and molecular adhesion that occur during the drying of MEMS. As the liquid in the space between the device layer and the base layer is removed by drying, the surface tension forces pull the device layer down until the layer of liquid is gone. Once the device layer is stuck to the base layer, it cannot be released causing the MEMS device to fail to actuate.

<div align="center">
  
![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/b4e1cab6-0f10-4919-82ab-854925b2e706)
</div>

<p align="center">
  <strong>Figure 4:</strong> A schematic of stiction causing permanent sticking of the released device to the base layer, an undesirable effect that can occur during the release step wherein the sacrificial SiO2 layer is etched away.
</p>

To prevent stiction during wet etching of the sacrificial layer, MEMS devices are kept moist until they are dried using a critical point dryer that utilises liquid CO2 to dry the devices due to its low surface tension. To eliminate any chance of stiction occurring, it is possible to instead etch the sacrificial layer using gaseous hydrofluoric acid (HF). Further explanation of the dry etching of the sacrificial layer done for this project is included in its own section. It is important to note that stiction can occur if the devices come into contact with liquid after the VHF process has been completed, and therefore cannot be cleaned once processing is completed. VHF etching will be performed on your wafers to release the devices in order to prevent risk of stiction.

## Deep reactive ion etch and Bosch process
The *inductively coupled plasma reactive ion etch* (ICPRIE), also known as deep reactive ion etch (DRIE), is used to anisotropically etch the silicon device layer to reach the underlying SiO2 using a method called the Bosch process. Anisotropic etching is a desirable process as it allows deep structures with high aspect ratios to be made. The Bosch process is a patented method of anisotropically etching silicon that utilizes a two-step cycle to etch.

The Bosch process is sensitive to the temperature of the substrate and operates successfully below 35 °C. It is critical to ensure sufficient heat conduction to the substrate to allow cooling. At temperatures above ~50 °C the formation of the protective polymer is inhibited. This causes an isotropic etch across the entire feature surface, destroying the device.

## Vapour Phase HF etching
For etching, a dry etching technique called Vapor Phase HF etching is quite popular and is employed to isotopically etch the sacrificial SiO2 layer to release the devices. By using a gaseous method instead of a liquid method to remove the sacrificial SiO2 layer, stiction will be prevented.

<div align="center">
  
![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/40a45d81-dca0-443f-b432-68a4c5b85a0c)
</div>

<p align="center">
  <strong>Figure 5:</strong> SEM image of a deep silicon etch using the Bosch process.
</p>

## Process flow overview
The fabrication of devices at the micrometre-scale (or smaller) is made possible by utilizing planar integrated circuit fabrication technology. A two dimensional image is transferred from a mask to the surface of a wafer using lithography and etching. An overview of the process flow for this project is given here:

### Step 1 — Wafer preparation
The SOI wafer is cleaned using piranha solution before processing to remove any foreign materials that might be on the surface.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/b07e5c9f-feac-4d7b-a98d-3703521726c7)

### Step 2 — Lithography: Apply resist
A layer of UV-sensitive material called photoresist is spin-coated onto the surface of the wafer.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/ab222ef2-4ac8-4efa-a3f4-4740289d527c)

### Step 3 — Lithography: Align and expose
A patterned mask (metal pattern on glass) is brought into contact with the photoresist. The photoresist is exposed to UV light, through the mask. Areas covered by metal on the mask are protected, while uncovered areas are exposed to the UV light. The UV light exposure changes the chemical composition of the photoresist in the exposed areas.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/e7552573-d581-48c5-acdf-a0978a4f95a7)

### Step 4 — Lithography: Develop
The wafer is then placed in a developer solution that removes the resist in the regions where it has been exposed to the UV light.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/ece29eb3-7ab9-43f8-b8ce-3f6746427508)

### Step 5 — Etching
The photoresist acts as a protective layer and the uncovered Si device layer is etched away using the ICPRIE until the underlying SiO2
layer is reached. In this manner, you can selectively etch away areas of the silicon to form MEMS devices.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/34070a9d-4e69-4f3a-a562-bf8042f5fae2)

### Step 6 — Resist removal
The remaining photoresist is removed using an oxygen plasma etch, leaving only the SOI with a patterned Si device layer.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/b962024b-6018-49ed-b2a1-bf75c3952cca)

### Step 7 — SiO2 etch and drying
The sacrificial SiO2 BOX layer is removed, or “sacrificed”, by VHF etching in order to release the MEMS so that the devices can actuate. The remaining SiO2 anchors the stationary sections of the individual MEMS device.

![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/739a3143-f763-4e49-ad1e-d1e45f297370)

The finished devices will be characterized and tested using scanning electron microscopy and device probing.

# Results

<div align="center">
  
  ![20231130_141747](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/1ef9626b-060b-4c91-b755-ceb06a127943)

</div>

<p align="center">
  <strong>Figure 6:</strong> Fabricated MEMS Wafer.
</p>

<div align="center">
  
  ![20231130_140758](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/0e1cfe85-9488-4c30-bc7b-9b63b0cf9e86)

</div>

<p align="center">
  <strong>Figure 7:</strong> Hitachi S4800 FESEM used for Imaging.
</p>

<div align="center">
  
  ![20231123_140804](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/bdb894c4-6f40-46cc-8b0c-c823e4a4aeaf)

</div>

<p align="center">
  <strong>Figure 8:</strong> The Wentworth probing station is used to actuate the comb drives by adjusting the voltage and measure the resulting displacement in the devices.
</p>

<div align="center">

  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/28f0217e-a1eb-4eac-a698-c98edc8afceb)

</div>

<p align="center">
  <strong>Figure 9:</strong> Small comb drives.
</p>

<div align="center">

  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/da06d218-8b37-480e-8e4c-4520d736476d)

</div>

<p align="center">
  <strong>Figure 10:</strong> Large comb drives.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/7e8bfcc0-4f95-4a23-b984-c1eb6f887839)

</div>

<p align="center">
  <strong>Figure 11:</strong> A tri-padded Archimedean spiral spring MEMS with 6 comb drives (12/12 teeth per comb drive) designed by Mark Salomons.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/5ceb8e05-cce9-4979-a7ff-1f46d8438554)

</div>

<p align="center">
  <strong>Figure 12:</strong> Smooth movers cell.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/d75dc5fb-e84d-4939-ac3d-b8fddcd1a63d)

</div>

<p align="center">
  <strong>Figure 13:</strong> Extended-needle gauges with small drives. The larger square/rectangular pads in the middle are the anchors: one for the hinge of the needle; the other for the scale next to the moving needle.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/614df113-da06-4a52-a786-337fc78501da)

</div>

<p align="center">
  <strong>Figure 14:</strong> Resistance gauges: A comb drive attached to a resistance gauge, and a close-up of the gauge itself.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/73fda806-3ac7-4c5c-ac2d-7fd6e0dd3704)

</div>

<p align="center">
  <strong>Figure 15:</strong> SEM image of tri-padded Archimedean spiral spring MEMS.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/6b867281-0a4b-4da0-a323-759c22b8d73d)

</div>

<p align="center">
  <strong>Figure 16:</strong> Magnified SEM image of tri-padded Archimedean spiral spring MEMS.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/9baa48fa-4c8d-43b8-a044-2298987f8e09)

</div>

<p align="center">
  <strong>Figure 17:</strong> SEM Microscopy Image of Deep etch.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/aa3fa68e-170b-4fca-98e6-25d15d946ed3)

</div>

<p align="center">
  <strong>Figure 18:</strong> Magnified image of SEM Microscopy Image of Deep etch.
</p>

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/67d60086-82d8-4c33-8314-7edea15388e3)

</div>

<p align="center">
  <strong>Figure 19:</strong> SEM Microscopy Image of Sidewall structure.
</p>

# SOI MEMS project mask map

The mask used in this project was redesigned in the summer of 2016 by the course instructors using L-Edit v10.01 software and fabricated using the Heidelberg DWL-200 Laser Pattern Generator in the nanoFAB. . It is optimized to be used on SOI quarter wafers. It contains numerous repetitions of the rectangular die design shown below. Each die contains nine cells, each of which contains numerous comb drive devices, detailed below. To get the most fulfilling experience when interacting with the die, examine the cells one at a time as they are labelled alphabetically: A through F (regular cells), then B1 and B2 (bonus cells). The parameters for each device are described on the following pages.

<div align="center">
  
  ![image](https://github.com/NSaroya/MEMS-Fabrication-Project/assets/156468713/a29c3482-f56a-492f-9fc0-055f44f95972)

</div>

<p align="center">
  <strong>Figure 20:</strong> Layout of the MEMS die.
</p>

# References

[1] J. C. Sit, "ECE 457 lab manual — 2020–2021," Edmonton, 2023.

[2] Stephen A. Campbell, The Science and Engineering of Microelectronic Fabrication, Oxford University Press (2001).

[3] W. Wai-Chi, A.A. Azid, B.Y. Majlis, “Formulation of stiffness constant and effective mass for a folded beam”, Archive of Mechanics 62(5) (2010).

[4] William Chi-Keung Tang, “Electrostatic Comb Drive for Resonant Sensor and Actuator Applications”, Ph.D. Dissertation, University of California, Nov 21 1990.

[5] Mohamed Gad-el-Hak, The MEMS Handbook, CRC Press LLC ( 2002).

[6] Massood Tabib-Azar, Microactuators, Kluwer Academic Publishers (1998).

[7] Hector J. De Los Santos, Introduction to Microelectromechanical Microwave Systems, Artech House (1999).
