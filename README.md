# Automated Literature Analysis

This repository shows an example of how to perform an automated analysis of peer-reviewed scholar literature using Jupyter notebooks and Scopus' citation database. This analysis detects the number of publications over time, popular authors, popular venues, popular affiliations, and popular "topics" that appear within the documents' abstracts (detected using natural language processing).

# Requirements

The notebook requires access to Scopus: A citation database of peer-reviewed literature from scientific journals, books, and conference proceedings. To utilize the Scopus API, you (or your institute) needs a Scopus Python API `pip3 install scopus==1.6.0` and you must request an Elsevier Developer API key (see [Elsevier Developers](https://dev.elsevier.com/sc_apis.html) for more information).

The required Python packages can be found in requirements.txt. Creating a virtual Python environment is recommended (for example, virtualenv or conda). The notebook has been tested using Python 2.7 and Python 3.6.

Last, you may need to install the library `pip3 install PyYAML`. Using `pip3 list` to check the PyYAML (5.1.1) version.

# Running the Notebook

After installing the dependencies, use `jupyter notebook literature_analysis.ipynb` to launch the notebook. Remaining instructions can be found within the notebook itself.

# Examples

```
query = 'title-abs-key("evolving neural network" AND ("deep learning" OR "object recognition"))' 
```

# Citation

Please cite the literatures below if you use our code.
```
@InProceedings{lan2018directed,
author="Lan, Gongjin
and Jelisavcic, Milan
and Roijers, Diederik M.
and Haasdijk, Evert
and Eiben, A. E.",
editor="Auger, Anne
and Fonseca, Carlos M.
and Louren{\c{c}}o, Nuno
and Machado, Penousal
and Paquete, Lu{\'i}s
and Whitley, Darrell",
title="Directed Locomotion for Modular Robots with Evolvable Morphologies",
booktitle="Parallel Problem Solving from Nature -- PPSN XV",
year="2018",
publisher="Springer International Publishing",
address="Cham",
pages="476--487",
isbn="978-3-319-99253-2"
}

@INPROCEEDINGS{lan2018ICARCV, 
author={Gongjin Lan, Jesús Benito-Picazo, Diederik M. Roijers, Enrique Domínguez, A.E. Eiben}, 
booktitle={2018 15th International Conference on Control, Automation, Robotics and Vision (ICARCV)}, 
title={Real-Time Robot Vision on Low-Performance Computing Hardware}, 
year={2018}, 
volume={}, 
number={}, 
pages={1959-1965}, 
doi={10.1109/ICARCV.2018.8581288}, 
ISSN={}, 
month={Nov},}

@INPROCEEDINGS{lan2017development, 
author={G. Lan and J. Liang and G. Liu and Q. Hao}, 
booktitle={2017 IEEE 31st International Conference on Advanced Information Networking and Applications (AINA)}, 
title={Development of a Smart Floor for Target Localization with Bayesian Binary Sensing}, 
year={2017}, 
volume={}, 
number={}, 
pages={447-453}, 
doi={10.1109/AINA.2017.27}, 
ISSN={1550-445X}, 
month={March},}

@INPROCEEDINGS{lan2016developmentuav, 
author={G. Lan and J. Sun and C. Li and Z. Ou and Z. Luo and J. Liang and Q. Hao}, 
booktitle={2016 IEEE International Conference on Multisensor Fusion and Integration for Intelligent Systems (MFI)}, 
title={Development of UAV based virtual reality systems}, 
year={2016}, 
volume={}, 
number={}, 
pages={481-486}, 
doi={10.1109/MFI.2016.7849534}, 
ISSN={}, 
month={Sept},}

@INPROCEEDINGS{lan2016action, 
author={G. Lan and Y. Bu and J. Liang and Q. Hao}, 
booktitle={2016 IEEE International Conference on Mechatronics and Automation}, 
title={Action synchronization between human and UAV robotic arms for remote operation}, 
year={2016}, 
volume={}, 
number={}, 
pages={2477-2481},  
doi={10.1109/ICMA.2016.7558955}, 
ISSN={2152-744X}, 
month={Aug},}
```

# Acknowledgement
The code originate from [stijnh](https://github.com/stijnh/automated-literature-analysis.git) but we improved. 
