# Quantifying forest recovery dynamics in the Amazon post selective logging

For my UC Berkeley senior thesis, I analyzed the effects of different selective logging methods on carbon stocks in Paracou, French Guiana using both field methods and ecosystem modelling. 

In this script, I first create an ETL pipeline to to prepare my dataset for data analysis.

There were 4 treatment groups (control, T1, T2, and T3), with 3 plots assigned to each treatment.

Set paths and file names for input and output.

-   **home_path**. The user home path.
-   **main_path**. Main working directory
-   **rdata_path**. Output path for R objects (so we can use it for comparisons.)

Then, I filtered and cleaned my dataset, and created subplots based on 50-meter grid intervals using tree coordinate data within each plot to add more data points within my dataset.

Then, for each indicator of forest recovery, I calculated or estimated the metric, and then plotted the indicator against time. For some, I also visualized other summary metrics.

At the end of the script,

I wrote initial conditions for FATES, a vegetation demography model we used to run simulations on the dataset and get an ecosystem modelling perspective on forest recovery.

