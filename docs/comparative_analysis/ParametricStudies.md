# Comparative Analysis Using the ParametricAnalysisTool (PAT)

___________________

## Creating a Project
The [ParametricAnalysisTool Quick Start Guide (PDF)](../../img/pdfs/PAT-Quick_Start_Guide_1.4.0.pdf) provides an introduction to the interface and workflow for creating multiple design alternative from a seed model. 

When you first open PAT you will see the screen below. It shows the workflow:

1. Organize and edit measures for project
2. Select measures and create design alternatives
3. Run simulations
4. Create and view reports

![Opening Screen](../../img/pat/opening_screen.png "Opening Screen for PAT")

*Above: This is the opening screen for PAT. It gives you an overview of the workflow.*

You can move through the four verticle tabs on the leftworkflow by working in order from top to bottom.

To Create a project use the menu item File/New Project

![New Project](../../img/pat/file_open.png "New Project")

*Above: The file menu provides new, open, save as, and other functionality.*

![New Project2](../../img/pat/file_open2.png "New Project Dialog")

*Above: The dialog takes you to a window to save your new project.*

<iframe width="640" height="360" src="http://www.youtube.com/embed/3rmElK_OB28?rel=0&start=0&end=107&autoplay=0" frameborder="0" allowfullscreen></iframe>

*Above: The video above shows the creation of a new project and gives a short introduction to the interface.*

___________________

## Loading a Baseline Model

Select your baseline model by hitting the browse button or typing in a path to your baseline OSM (Open Studio Model) file.

![Baseline Model](../../img/pat/baseline.png "Selecting a Baseline Model")

*Above: The dialog takes you to a window to save your new project.*

___________________


## Organize and Edit Measures for Project
To add measures to your project, drag measures from the library to the central panel.

If you want to learn more about measures check out the [About Measures](../measures/AboutMeasures.md) section.  


*Above: The "Set Window to Wall Ratio by Facade Group 1" contains 3 versions of the same measure with different parameter settings. The next section will show how to set measure parameters.*


*Above: Adding measures to your project and editing the parameters*

### Defining Measures
You can edit the measure parameters and names by selecting the measure in the central panel. The measure will be highlighted with orange and the right panel will go to the "Edit" tab.

![Editing](../../img/pat/measure_parameters.png "Editing Measure Parameters")

*Above: Select a measure in the central panel and view the fields available for editing in the "Edit" panel on the right.*

![Warning](../../img/pat/warning.png "Warning")

*Above: A warning icon will be next to the measure if a required field is empty. Go to the "Edit" tab on the right panel and look for the red text.*


### Downloading Measures from the Building Component Library

Before you can download measures from BCL, you will need an [API Key follow the instructions in the Getting Started section](../../GettingStarted/#connecting-with-the-building-component-library) to get your key.

From the “Measures” menu and “Find Measures” along the top or the “Find Measures on BCL” button at the bottom of the “Library” you can access the BCL.

The "Sync Project Measures with Library" will updated any older measures in your project to the latest versions.

![Measures Menu](../../img/pat/measures_menu.png "Measures Menu")

*Above: One of the ways to access the BCL measures is through the menu.*


*Above: Browse categories or search for measures to download.*

You can also search and browse measures on the [Building Component Library site.](https://bcl.nrel.gov/)

### Duplicating and Creating New Measures
If you can't find the measure you need you can duplicate a measure and adjust it or you can write a custom measure. Learn more about writing measures in the [Measure Writing Guide](../measures/Measure-Writing-Guide.md)

![Measures Buttons](../../img/pat/measure_buttons.png "Measure Buttons")

*Above: Create your own measures with the features provided on the bottom of the right panel.*

Hit the “New Measure” icon to open a dialog to create your own measure. Write a descriptive title, more detailed descriptions, and select the measure type and taxonomy.


*Above: The dialog for creating your new measure is shown above.*

___________________

## Select Measures and Create Design Alternatives

<iframe width="640" height="360" src="http://www.youtube.com/embed/4g5nJzDoh58?rel=0&start=0&end=116&autoplay=0" frameborder="0" allowfullscreen></iframe>

*Above: This video shows you how to create design alternatives in an OpenStudio ParametricAnalysisTool Project.*

___________________

## Run Simulations
Select the design alternative you want to run. Selected alternatives turn the yellow-orange. Hit the run button to start the simulations.

You must select the design alternatives you want to run before hitting the run buttons. Selected items have an orange highlight.

![Run Simulations in Pat](../../img/pat/run_tab.png "Run Tab")

*Above: Screenshot of the "Run" tab with design alternatives selected.*

<iframe width="640" height="360" src="http://www.youtube.com/embed/4g5nJzDoh58?rel=0&start=117&end=273&autoplay=0" frameborder="0" allowfullscreen></iframe>

*Above: Running your simulations.*

___________________

## Create and View Reports


<iframe width="640" height="360" src="http://www.youtube.com/embed/9WgUhiJ785I?rel=0&start=&end=&autoplay=0" frameborder="0" allowfullscreen></iframe>

*Above: This video shows the simulation results of a parametric analysis and then shows you how to inspect a specific design alternative in the SketchUp Plugin.*

___________________


## Making Changes After an Analysis

___________________


## Running on the Cloud
There are a few things to do before you click the “Turn on Cloud” button, fill out the Cloud Settings dialogs from the Cloud menu,run your baseline model locally, and then make sure you have selected all of the design alternatives that you want to run. Choosing “Select All” will select all jobs that have not already been run locally, or on a previous cloud session. 

Select your baseline model, then run locally before you start the cloud to confirm that it is valid and will run properly. To do this you can deselect all other design alternatives, and then select just the baseline.

![Cloud Settings 1](../../img/pat/cloud_settings_menu.png "Cloud Settings Screen One")

*Above: Get to the Cloud Settings at any time from the "Cloud" menu.*


*Above: Fill out the first screen and agree to terms before continuing to the second screen.*

On the second screen of the “Cloud Settings” dialog, confirm that you have chosen the desired sever, worker, and number of workers. 


*Above: Fill out the first screen and agree to terms before continuing to the second screen.*


<iframe width="640" height="360" src="http://www.youtube.com/embed/0llNfGNe5x0?rel=0&start=&end=&autoplay=0" frameborder="0" allowfullscreen></iframe>

*Above: The video above demonstrates running simulations on the cloud.*


*Above: Open this dialog from the "Cloud" menu.*


The "Turn on the Cloud" button has several states to let you know the status of the cloud.


![Cloud Buttons](../../img/pat/cloud_buttons.png "Cloud Button States")

*Above: The states of the cloud button are shown.*


You can download standard or detailed results from your runs. If you want detailed results click on the download button in the table. You can choose to download all of the results in detail but it may be a large download. 

![Cloud Download](../../img/pat/download_results.png "Cloud Results Downloads")

*Above: The states of the cloud download button are shown.*

While your project is running on the cloud you can choose the design alternative and select “Download Detailed Results for Selected File” button if you want more detailed data on some of the options.


![Cloud AWS](../../img/pat/aws.png "AWS Console")

*Above: Check your status on AWS and terminate sessions if you have problems in PAT.*
While your runs are completing on the cloud and after they are finished you can explore your results with the OpenStudio Cloud Management Console. 


![Cloud OS Console](../../img/pat/os_console1.png "OS Console")

*Above: This pie chart shows the progress of the runs. Select "View Analysis" to explore results.*


![OS Console Analysis](../../img/pat/os_console2.png "OS Console Analysis")

*Above: The red boxes added to the screenshot above shows where you can select charts and download results in different formats:

* List of Measures



![Cloud Download](../../img/pat/download_results_during.png "Cloud Results During")

*Above: Right click on design alternative to get these options. If your model includes calibration reports the calibration button at the top of the results will display those in a table format in the application*