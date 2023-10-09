# RaagBase

RaagBase is a Hindustani Music dataset for research in computational musicology.

One of the most authentic sources of Hindustani Sangeet is the compositions published in the book Hindusthani Sangeet Paddhati-Kramik Pustak Malika which comprises of approximately 1900
compositions with notations and raags belonging to North Indian Classical Music penned by Pt. Vishnu Narayan Bhatkhande (1860- 1936). In order to reach a greater number of music students and scholars, the first volume of Kramik Pustak Malika has been translated to Hindi language in 1953 by prominent music scholar Dr. Laxminarayan Garg. We have used the music-sheet compositions from Kramik Pustak Malika and have prepared a dataset RaagBase consisting of 116 samples each of which corresponds to the note frequency distribution of a composition and label each such composition with the corresponding raags given in the book itself.

The second volume of the book series contains a total of 319 compositions belonging to 10 different raags. RaagBase takes these written compositions as a source of musical information to create the database for Hindustani Sangeet to be used in computational musicological research. We have taken 116 compositions of the three highest frequent raags (more than 30 compositions) i.e. raag Bhairav or bh (42), Todi or td (39), and Poorvi or pv (35) respectively, from the entire collection of 319 compositions for the creation of machine learning
and graph models and performing our experimental analysis. Eventually, the entire collection of compositions from all six volumes will be preserved in RaagBase and thereby enriching the dataset by including almost 1900 compositions covering 50 odd raags.

The RaagBase is stored in the file named `Bhatkhande-Dataset.csv`. The dataset is a single comma separated values (CSV) file where the notes of each composition along with the raags are manually stored. Therefore, each sample of the dataset corresponds to a single composition and the notes of each composition span over three octaves or _Saptaks_, namely the middle or _Madhya_, upper or _Taar_, and lower octave or _Mandra_ Saptak.

We also represent RaagBase as graph by exploiting the dominance and absence of notes in a composition provided by the characteristic sequences. We apply several existing robust
graph clustering techniques for identifying similar raag compositions. Experimental results show extremely accurate clusters having high accuracy, thus validating RaagBase. The code for implementing graph clustering techniques is given in `Musical-graph.ipynb` file.
