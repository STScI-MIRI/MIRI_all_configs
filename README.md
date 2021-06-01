# MIRI_all_configs
 
This repository contains a notebook intended to compile a list of all possible configurations of MIRI and then check for a refence file for each configuration in CRDS in order to address https://jira.stsci.edu/browse/JWSTMIRI-200

The possible configurations are informed by https://innerspace.stsci.edu/pages/viewpage.action?spaceKey=JWST&title=MIRI+Allowed+Configurations

Each section uses for-loops to generate a list of possible configurations for that mode and append them to a master pandas dataframe. These sections need to be updated manually for any changes to the list of possible configurations.

The list is then queried against CRDS using `crds.getrecommendations()` and the output is sorted into '.txt' files by filter type.
