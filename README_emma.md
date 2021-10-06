### Overview ###
Data set contains information from the Ames Assessor’s Office used in computing assessed values 
for individual residential properties sold in Ames, IA from 2006 to 2010.
SIZE: 2930 observations, 82 variables


This data set was constructed for the purpose of an end of semester project for 
an undergraduate regression course. The original data (obtained directly from the Ames 
Assessor’s Office) is used for tax assessment purposes but lends itself directly to the
prediction of home selling prices. The type of information contained in the data is similar 
to what a typical home buyer would want to know before making a purchase and students should 
find most variables straightforward and understandable.

### Data Science Problem Statement ###
As a real restate developer company, how do we position ourself better in comparison to our
competitors, to take advantage of this current trend / phenomenon? 
What parts of a house should we allocate our resource to when building new housing for 
the Millennials to maximize our profit?  

### Datasets ###

** Original Datasets **
[`train.csv`]
[`test.csv`]

** Cleaned & Organized Datasets **
(based on the above 2 datasets)
[`train_eda_clean.csv`] Cleaned Train Dataset 
[`test_clean.csv`] Cleaned Test Dataset 1st Draft
[`test_clean2.csv`] Cleaned Test Dataset 2nd Draft
[`test_clean_final.csv`] Final Cleaned Test Dataset
[`df_test_1.csv`] Id Column only from test.csv
[`Kaggle_Sumbmission_df_test3.csv`] Kaggle Submission File (845 predictions)
[`Kaggle_Submission_TSUI.csv`] Final Kaggle Submission File (878 predictions)


### Data Dictionary ###
|Feature|Type|Dataset|Description|
|---|---|---|---|
|id|int|train|Unique identification number of each property|
|pid|int|train|Parcel identification number - can be used with city website for parcel review|
|ms_subclass|int|train|Identifies the type of dwelling involved in the sale|
|ms_zoning|int|train|Identifies the general zoning classification of the sale| 
|lot_frontage|float|train|Linear feet of street connected to property|
|lot_area|int|train|Lot size in square feet|
|street|int|train|Type of raod access to property|
|lot_shape|int|train|General shape of property|
|land_contour|int|Train|Flatness of the property|
|utilities|int|Train|Type of utilities available|
|lot_config|int|Train|Lot configuration|
|land_slope|int|Train|Slope of property|
|neighborhood|int|Train|Physical locations within Ames city limits|
|condition_1|int|Train|Proximity to various conditions|
|condition_2|int|Train|Proximity to various conditions (if more than one is present)|
|bldg_type|int|Train|Type of dwelling|
|house_style|float|Train|Style of dwelling|
|overall_qual|int|Train|Rates the overall material and finish of the house|
|overall_cond|int|Train|Rates the overall condition of the house|
|year_built|int|Train|Original construction date|
|year_remod/add|int|Train|Remodel date|
|roof_style|int|Train|Type of roof|
|roof_matl|int|Train|Roof material|
|exterior_1st|int|Train|Exterior covering on house|
|exterior_2nd|int|Train|Exterior covering on house (if more than one material)|
|mas_vnr_type|float|Train|Masonry veneer type|
|mas_vnr_area|float|Train|Masonry veneer area in square feet|
|exter_qual|int|Train|Evaluates the quality of the amterial on the exterior|
|exter_cond|int|Train|Evaluates the present condition of the amterial on the exterior|
|foundation|int|Train|Type of foundation|
|bsmt_qual|float|Train|Evaluates the height of the basement|
|bsmt_cond|float|Train|Evaluates the general condition of the basement|
|bsmt_exposure|float|Train|Refers to walkout or garden level walls|
|bsmtfin_type_1|float|Train|Rating of basement finished area|
|bsmtfin_sf_1|float|Train|Type 1 finished square feet|
|bsmtfin_type_2|float|Train|Rating of basement finished area (if multiple types)|
|bsmtfin_sf_2|float|Train|Type 2 finished square feet|
|bsmt_unf_sf|float|Train|Unfinished square feet of basement area|
|total_bsmt_sf|float|Train|Total square feet of basement area|
|heating|int|Train|Type of heating|
|heating_qc|int|Train|Heating quality and condition|
|central_air|int|Train|Central air conditioning|
|electrical|int|Train|Electrical system|
|1st_flr_sf|int|Train|First floor square feet|
|2nd_flr_sf|int|Train|Second floor square feet|
|low_qual_fin_sf|int|Train|Low quality finished square feet (all floors)|
|gr_liv_area|int|Train|Above grade (ground) living area square feet|
|bsmt_full_bath|float|Train|Basement full bathrooms|
|bsmt_half_bath|float|Train|Basement half bathrooms|
|full_bath|int|Train|Full baths above grade|
|half_bath|int|Train|Half baths above grade|
|bedroom_abvgr|int|Train|Bedrooms above grade|
|kitchen_abvgr|int|Train|Kitchens above grade|
|kitchen_qual|int|Train|Kitchen quality|
|totrms_abvgrd|int|Train|Total rooms above grade (does not include bathrooms)|
|functional|int|Train|Home functionality|
|fireplaces|int|Train|Number of fireplaces|
|fireplaces_qu|float|Train|Fireplace quality|
|garage_type|float|Train|Garage location|
|garage_yr_blt|float|Train|Year garage was built|
|garage_cars|float|Train|Size of garage in car capacity|
|garage_area|float|Train|Size of garage in square feet|
|garage_qual|float|Train|Garage quality|
|garage_cond|float|Train|Garage condition|
|paved_drive|int|Train|Paved driveway|
|wood_deck_sf|int|Train|Wood deck area in square feet|
|open_porch_sf|int|Train|Open porch area in square feet|
|enclosed_porch|int|Train|Enclosed porch area in square feet|
|3ssn_porch|int|Train|3 season porch areain square feet|
|screen_porch|int|Train|Screen porch area in square feet|
|pool_area|int|Train|Pool Area|
|pool_qc|int|Train|Pool Quality|
|fence|float|Train|Fence Quality|
|misc_val|int|Train|Value of Miscellaneous Feature|
|mo_sold|int|Train|Month Sold (MM)|
|yr_sold|int|Train|Year Sold (YYYY)|
|sale_type|int|Train|Type of Sale|
|salesprice|int|All|Sale Price / Predicted Sale Price|

### Conclusion ###
In order to maximize sale price of our newest project, it’s best to choose a suburb area that we can maximize above ground living area and garage area sizes. In addition, put emphasis on kitchen quality, garage finish, fireplace quality, the numbers of full bathrooms, and the numbers of total rooms above ground. This should put us above our competitors while increasing Sale Price and, thus, our total revenue.

False Combination: Big Yard Size + Small House