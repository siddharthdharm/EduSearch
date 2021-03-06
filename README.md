# EduSearch Engine for Information Retrieval in Python3
We aim to provide fast and efficient retrieval of queries related to Computer Science on our Search Engine. We have already pre-processed (indexing) all the websites in the education domain, i.e. '.edu'.
<br>
We have ranked pages in the corpus by considering the inlinks and outlinks.
<br>We have handled dead ends and spider traps.
<br>Also, Topic Specific Page Rank and visualization of page links using igraph has been implemented!

**Installing igraph in ubuntu:**
```
Try step 3 first. If you get an error then follow from step 1. 
1. Install aptitude: sudo apt install aptitude
2. Installing the igraph C library: aptitude install build-essential libxml2-dev libglpk-dev libgmp3-dev libblas-dev liblapack-dev libarpack2-dev python-dev
3. pip3 install python-igraph
```

**Instructions on running the code**
```
1. Open terminal and change to the directory containing the main.py file

2. Open main.py:
	A. Specify the data_file value.
	B. If page numbers in dataset are 0-indexed then set is_page_no_zero_indexed = True otherwise set it to False
	C. Set the value of epsilon for convergence
	D. Set max_iterations for calculating pageranks
	E. Set beta value which will be used to avoid spider traps and dead ends.
	F. set the value of display_network_after_each_iteration to True if you want to show the network structure after each iteration.
	G. Set the value of max_nodes_to_show which will specify how many of the top pages to show in the network structure/
	H. If you have a teleport_set then set the value of this list otherwise let it be the way it is.

3. Type: python3 main.py
```
