# Continuous Intelligence

This site provides documentation for this project.
Use the navigation to explore module-specific materials.

## How-To Guide

Many instructions are common to all our projects.

See
[⭐ **Workflow: Apply Example**](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to get these projects running on your machine.

## Project Documentation Pages (docs/)

- **Home** - this documentation landing page
- **Project Instructions** - instructions specific to this module
- **Your Files** - how to copy the example and create your version
- **Glossary** - project terms and concepts

## Additional Resources

- [Suggested Datasets](https://denisecase.github.io/pro-analytics-02/reference/datasets/cintel/)

## Custom Project https://github.com/BJean-0905/cintel-02-static-anomalies/blob/main/src/cintel/anomaly_detector_bjean.py

## Dataset includes data from youth clients at a behavioral health organization https://github.com/BJean-0905/cintel-02-static-anomalies/blob/main/data/clinic_data_bjean.csv

## Signals
Age- the age of clients in years
Height- the height of clients in inches
Clinical group- strata used to determine assessment needs

## Experiments
Anomaly Detection- checking for anomalies based on age and height while adding clinical group to clarify assessments utilized for that grouping.
Threshold- min age=3, due to min age for client admissios in behavioral health. max age=18, based on adult age. height min=36, max=72. clinical group had no thresholds associated.

##Results
9 anomalies were detected based on age and height. parameters set in min and max included in these parameters.

##Interpretation
Viewing results by group clinical group helped identify any potential assessments that may be a part of the anomaly detection process in regards to clinical implications. Awareness of min/max data utilized is valuable in setting parameters. For example, any child at 72 inches would be flagged since the height max parameter was set at 72. Additionally, any max age of 18 would be flagged as well since 18 was included in the max parameter. It is useful to add columns that may provide more information for additional context, grouping, sampling or auditing. The anomaly detection was easy to read and understand why the data was included.
