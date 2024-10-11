# Distributed_DNA_Multi-Strand_Simulator


This software provides a platform to simulate DNA multi-strands on a distributed model using NFsim simulator. 

NFsim simulator author:
Michael Sneddon http://michaelsneddon.net/nfsim/

Distributed DNA Multi-Strand Simulator software developed by Frankie Spencer,

Project led by Dr. Eugen Czeizler,

    Algorithms and Software in Bio-Engineering (AlgoBio), 
    Dept. of Information Technologies, 
    Åbo Akademi University, 
    Åbo, Finland

Software is free and open source. 


Instructions:
    
Download the software package as zip file using 'Download ZIP' and extract files. This software does not require additional installations of dependencies. 

IMPORTANT: If you have installed python already in your system, It is necessary to remove them in order for software package included python interpreter to work properly. 

Software package has embedded the following free and open source tools:

    -NFsim_v1.11 - http://michaelsneddon.net/nfsim/download/
    -strawberry-perl-5.30.0.1-64bit-portable - https://strawberryperl.com/releases.html
    -python-3.8.7-embed-amd64 - https://www.python.org/downloads/release/python-387/
    --joblib==1.4.0

OS requirement - Windows 7 or later versions

Please fill the “simulation_parameters.json” according to following instructions. 
Then run 'RUN.bat' file. There will be number of command line windows will pop up (number will depend on how many CPU threads are used). 

Note: It may be not possible to use the system during these simulations since they do not run on background. 

--------------------------------------------------------------------------

{

Desired number of CPU threads to be utilized for the simulation, e.g. 8

   "number_of_parallel_threads": 8,

Simulation model time in seconds, e.g. 10

   "simulation_time": 10,

Desired number of test suites to run. Here you can set multiple simulation sets to run, e.g. 10

   "number_of_test_suites": 10,

The input file location on the system. You can find our samples ".species" files at "test_samples"

   "input_species_file": "C:/my_species_file_directory/dx_tile_small-scale_example.species",

Desired directory to collect results. Make sure this directory exists.

   "save_results_directory": "C:/my_save_results_directory/my_test_simulation",

Delete temporary files for saving system space. We recommend set it to "true" unless you decide otherwise.

   "delete_temporary_files": true
 
}
