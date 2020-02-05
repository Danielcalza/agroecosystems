## Agroecology Cover Crop and Agroecosystems Experiment at TREC

### Summary

- Data management and products generated by `TREC-summary.R`
- [Detailed methods at wiki](https://github.com/TREC-Agroecology/agroecosystems/wiki)

### Planting & Harvest Seasons

- `summer`: May 10, 2018 - Aug 15, 2018
- `winter`: Nov 1, 2018 - Jan 11, 2019

- `summer`: May 13, 2019 - July 11, 2019
- `winter`: Nov 6, 2019 - Jan 6, 2020

- 'summer': May , 2020 - July , 2020

### Experimental Design

- 6 treatments (`CropTrt`)
- Cover crops
   - Sunn hemp (`SH`)
      - seeding rate = 30 lbs/acre
   - Sorghum-sudangrass (`SS`)
      - seeding rate = 30 lbs/acre
   - Velvet bean (`VB`)
      - seeding rate = 60 bs/acre
- Mixtures [seeding rate = 1/2 rate for each crop]
   - `SHSS`
   - `SHVB`
   - `SSVB`
- 6x6 Latin square at 4 `Location`
   - Vegetable field
      - `VF`
      - Block 1
      - historically agricultural soil
   - Fruit orchard 
      - `FO`
      - Block 4
      - historically agricultural soil
   - Hardwood Hammock
      - `HH`
      - Block 14
      - Newly prepared agricultural soil
   - Old collection
      - `OC`
      - Block 15
      - Newly prepared agricultural soil
- `PlotName` = `[Site]_[treament]-[row]` (`VF_SHSS-1`)
- `PlotID` integer
   - `VF` `1:36`
   - `FO` `37:72`
   - `HH` `73:108`
   - `OC` `109:144`  

### Data Products

`biomass_soil_[season]_[crop].csv` (`biomass_soil_winter_SH.csv`)
`height_[season]_[crop].csv` (`height_winter_SH.csv`)
- 'Season': time period of plantings (i.e. Summer or Winter)
- `Location`: experimental plot location at TREC [*linking field*]
- `CropTrt`: experimental treatment denoting cover crops in monoculture or mixture [*linking field*]
- 'CropName': experimental treatment of specific crop species in unit
- `SamplingWeek`: week of sampling after planting date
- 'EmergDay50_percent': day of fifty percent emergnce for a species in a unit
- `Height_cm`: canopy height of each crop at a `SamplingWeek` [*reported as a sample average (`avg_`) and standard deviation (`sd_`)*]
- `Chlorophyll_CCI`: chlorophyll index of greeness as measured by an Appogee MC-100 
- 'pH': pH reading of soils as measured by an Oakton pH6+
- `LeavesStems_tha`: an estimate of aboveground biomass for each crop within a treatment at harvest [*reported as a sample average (`avg_`) and standard deviation (`sd_`)*]
- 'Roots_tha': an estimate of belowground biomass for each crop within a treatment at harvest
- 'Weeds_tha': an estimate of weeds biomass for each crop within a treatment at harvest
- `SOM_percent`: soil organic matter as a percent of soil sample before planting
- `TP_mgkg: soil total phosphorous concentration in mg/Kg before planting [*summer only*]
- `GravelDryWgt_g`: gravel dry weight of bulk density sample in grams
- `GravelVol_mL`: gravel volume from bulk density sample in milliliters
- `SoilDryWgt_g`: soil dry weight from bulk density sample in grams
- `SoilVol_cm3`: soil volume from bulk density sample in cubic centimeters (i.e. mL)
- `SoilBD_gcm3`: soil bulk density in grams / cubic centimeters
- `SoilPorosity_percent`: soil porosity from bulk density as a percent of sample volume
- 'PreIgnitionWgt_g': beaker and soil sample weight before muffle furnace 
- 'PostIgnitionWgt_g': beaker and soil sample weight after muffle furnace
- 'AshWgt_g': weight of ash minus beaker after muffle furnace 
- 'LOIorSOM_percent': percentage of soil organic matter by LOI method 
- `NH4_mgL`: ammonium concentration from soil sample in milligrams / Liter
- `NO3_mgL`: nitrate concentration from soil sample in milligrams / Liter
- `NH4_mgKg`: ammonium concentration from soil sample in milligrams / kilogram
- `NO3_mgKg`: nitrate concentration from soil sample in milligrams / kilogram






