# MAPFD-AL: Maximum Annual Peak Flow Discharge for ALabama State

This study focuses on estimating maximum annual peak flow discharge for Alabama's gauged and ungauged river streams by developing, validating, and applying predictive models using data from U.S. Geological Survey (USGS) gage sites and various catchment and river channel attributes. We obtained peak flow discharge records from 188 USGS gauge sites and a diverse set of predictive parameters to form a dataset. We carried out meticulous preprocessing to ensure its accuracy and reliability. The dataset was divided into training and testing subsets for model development and validation. Multi-Linear Regression (MLR) and eXtreme Gradient Boosting Regression (XGBR) algorithms were employed to develop predictive models. XGBR emerged as the superior model due to its ability to handle nonlinearities and missing data adeptly. We adopted a hybrid approach by combining the two methods to enhance comprehensive coverage and representation of all variables, where XGBR was utilized within the range of training data. At the same time, MLR was used to extrapolate values outside this range. A comprehensive dataset and map displaying estimated maximum annual peak flow discharge values for both gauged and ungauged streams in Alabama was produced (__Figure 1__), which can facilitate better decision-making processes in flood risk and water resource management in Alabama.

![MAPFD-AL](https://github.com/Reizrb/NSF-R2O-NRT_2023/assets/133435701/45f64059-e435-4309-b7eb-e3d506f0ac4d)

__Figure 1.__ Map of estimated values of Maximum Annual Peak Flow Discharge <br> in cubic meter per second for 77,423 river streams (gauged and ungauged) <br> Alabama state 

## Download Dataset

_MAPFD-AL_ is publicly available in.

## Dataset Description

MAPFD-AL dataset includes _"COMID"_, _"REACHCODE"_, _"FTYPE"_, _"TotDASqKM"_, _"StreamOrde"_, _"MAPFD"_, and _"XGBR_or_MLR"_ fields, where the difination of each attributes and their unit of measurement are provided as below:

| Attribute Name | Attribute Description    | Unit of Measurement    |
| :---   | :--- | :--- |
| COMID |   Common identifier of the NHD feature   |  ---   |
| REACHCODE |  Reach Code assigned to feature   |  ---   |
|  FTYPE  |  NHD Feature Type  |  ---  |
|  TotDASqKM  |  Total upstream catchment area from downstream end of flowline   | SqKM  |
| StreamOrde  |  Modified Strahler Stream Order  | count |
|  MAPFD  |  Maximum Annual Peak Flow Discharge  | Cubic meter/Second |
|  XGBR_or_MLR  |  The final model utilized for prediction  | ---   |


