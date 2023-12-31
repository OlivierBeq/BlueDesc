[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

# BlueDesc Descriptor Calculator

Original BlueDesc executable from the website of the [University of Tübingen](http://www.ra.cs.uni-tuebingen.de/software/bluedesc/).
*Downloaded on 2020-04-11*

## Original information

BlueDesc Descriptor Calculator (last update: 03-10-08)
Author: Georg Hinselmann
License: GNU GPL

A key step in classical quantitative structure-activity/property relationship (QSAR/QSPR) modeling is the encoding of a chemical compound into a vector of numerical descriptors. Although most of the available chemoinformatic software packages provide routines for the calculation of descriptors they are not easy to use in most cases. This simple command-line tool converts an MDL SD file into ARFF and LIBSVM format for machine learning and data mining purposes using CDK and JOELib2.<br/>
<img src="img/descriptor-mapping.jpg" alt="An chemical compounds provides useful information which can be expressed as descriptors like charge, surfaces or counts" width="500"/>

A ready-to-use (executable JAR), 100% Java tool, which includes JOELib2 (GNU GPL) and the CDK (LGPL), sources and the GNU GPL. It computes 174 descriptors taken from both libraries. Works on 3D structures only. Output is ARFF (WEKA example) and libSVM (example) format.

An overview of the descriptors is given here. 

System requirement: JDK or JRE 1.6.

Syntax: <br/>
```java -jar -Xmx512M ODDescriptors.jar -f (sdf) -l (sdf property y)```

Example: <br/>
```java -jar -Xmx512M ODDescriptors.jar -f anthrax.sdf -l KI```

Note: If you just want to compute the descriptors, type in any property and ignore the WARNING. Note that you won't be able to learn on the resulting WEKA and LIBSVM files, because the target value will be replaced by "?". However, you may open this file in WEKA and WEKA Explorer.

Have fun! Please report bugs to the email adress given below.

Contact<br/>
Georg Hinselmann, Tel.: (07071) 29-77174, georg.hinselmann@uni-tuebingen.de<br/>
Nikolas Fechner, Tel.: (07071) 29-77174, nikolas.fechner@uni-tuebingen.de


