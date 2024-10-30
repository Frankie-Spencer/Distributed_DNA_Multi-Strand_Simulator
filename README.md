# Distributed DNA Multi-Strand Simulator

The Distributed DNA Multi-Strand Simulator software provides a platform to simulate DNA multi-strands on a distributed model using NFsim simulator. 

* VDNA-Lab software platform developer: Frankie Spencer [1]
* Project leader: Dr. Eugen Czeizler [1]
* NFsim simulator author: Michael Sneddon [2] – http://michaelsneddon.net/nfsim/

[1] Dept. of Information Technologies, Åbo Akademi University, Åbo, Finland\
[2] Yale University, New Haven, CT, United States

## Software Launch Instructions

* Pre-requisites: 
  * The Operating System requirement is **Windows 7 or later versions**. 
  * **7-Zip file archiver** is needed for file extraction. Please install the latest version – https://www.7-zip.org/. 
* Download the software package as a zip file using 'Download ZIP'. 
* Extract the software package files using 7-Zip. 
* Run 'RUN.bat' file. 

Note: It may be not possible to use the system during these simulations since they do not run on background. 

The Distributed DNA Multi-Strand Simulator software is free and open source and does not require additional installations of dependencies. The software package has embedded the following free and open source tools: 

* NFsim_v1.11 – http://michaelsneddon.net/nfsim/download/
* strawberry-perl-5.30.0.1-64bit-portable – https://strawberryperl.com/releases.html
* python-3.8.7-embed-amd64 – https://www.python.org/downloads/release/python-387/
  * joblib==1.4.0

## Setup Simulation Parameters JSON File

{

* Desired number of CPU threads to be utilized for the simulation, e.g. 8

   "number_of_parallel_threads": 8,

* Simulation model time in seconds, e.g. 10

   "simulation_time": 10,

* Desired number of test suites to run. Here you can set multiple simulation sets to run, e.g. 10

   "number_of_test_suites": 10,

* The input file location on the system. You can find our samples ".species" files at "test_samples"

   "input_species_file": "C:/my_species_file_directory/dx_tile_small-scale_example.species",

* Desired directory to collect results. Make sure this directory exists.

   "save_results_directory": "C:/my_save_results_directory/my_test_simulation",

* Delete temporary files for saving system space. We recommend set it to "true" unless you decide otherwise.

   "delete_temporary_files": true
 
}
