# TLHC
Targeted Lung Health Check Reporting

Scripts: 
update_names_tlhc.Rmd: 
Updates the cancer alliance and project names, and combines data for projects where necessary. This script should be run first. 
Input: 
- metrics flatfile
Output: 2x csv files 
- 1: metrics flatfile with udpated names  e.g. tlhc_midata_flatfile_2023-04-26.csv 
- 2: summary of changes made to names tlhc_midata_flatfile_2023-04-26_qa_check_renamed.csv
QA2223.qmd: 
This script produces tables and plots that can be used to aid QA of data. Produces heatmaps used for delivery group slides 
Inputs: 
- 1: metrics flatfile with udpated names  e.g. tlhc_midata_flatfile_2023-04-26.csv 
- 2: metrics flatfile with udpated names from previous month
- 3: trajectories 
- 4: summary of changes made to names tlhc_midata_flatfile_2023-04-26_qa_check_renamed.csv
- 5: cancer alliance and project names lookup table e.g. TLHC_names_lookup.csv
Outputs: 
-1. excel file with differences this months data vs previous months data for key metrics e.g. Feb23_vs_Jan23.xlsx
- 2. html QA file e.g. QA2223.html 
- 3. plot - cumulative actual values as a percentage of cumulative trajectories up to latest month of data. Used in DG slides e.g. ca_pcdiff_this_month.tiff
- 4. plot - cumulative actual values as a percentage of cumulative trajectories up to latest month of data but for live sites only. Used in DG slides e.g. ca_pcdiff_this_month_live_only.tiff
TLHC R Script - CA Packs 
Script to produce monthly cancer alliance packs 
Inputs: 
1. powerpoint template to use for ca packs: CA_Quarterly_Packs_Template.pptx
2. Trajectories 
3: metrics flatfile with udpated names  e.g. tlhc_midata_flatfile_2023-04-26.csv 
4: Which projects are in which phase e.g. TLHC_Phases.csv
5: Project start dates e.g. "TLHC_start_dates.csv"
6: Date_Dictionary.csv
Outputs: 
Directory containing 1x CA pack powerpoint file for each cancer alliance 
