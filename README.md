# Water and Sanitation in Indonesia
The dataset is from Community Based Water Supply and Sanitation Program in Indonesia.
The dataset contains 15 columns:
- village_id: village id
- household: number of household in a village. A household can have 1 or more people
- ws_access_h: number of household have water supply access in a village
- no_ws_access_h: number of household do not have water supply access in a village
- population: number of people in a village 
- ws_access_p: number of people have water supply access
- no_ws_access_p: number of people do not have water supply access
- ws_condition: water supply infrastructur condition [working, not working, not built yet]
- water_quality: water quality > qualified, not qualified, not tested yet
- hp_toilet_h: number of household have healthy permanent toilet
- hsp_toilet_h: number of household have healthy semi permanent toilet
- comm_toilet_h: number of household use communal toilet
- no_toilet_h: number of household do not have toilet and defecate carelessly
- ss_condition: sanitary system infrastructur condition [working, not working, not built yet]
- diarrhea_p: number of people have diarrhea

The dataset was manually inputted by a lot of people with various background, so there must be some invalid data.
These are some condition that need to keep, such as:
- ws_access_h + no_ws_access_h must be household
- ws_access_p + no_ws_access_p must be population
- hp_toilet_h + hsp_toilet_h + comm_toilet_h + no_toilet_h must be household
- all value >= 0

If there are some data that don't meet the condition, it is better to drop the row.
