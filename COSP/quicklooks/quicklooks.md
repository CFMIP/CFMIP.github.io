const gitdown = Gitdown(
  '{"gitdown": "variable", "width": "width.value"}'
);

gitdown.setConfig({
  variable: {
    scope: {
      width: {
        value: 200
      }
    }
  }
});

# COSP quicklooks

All figures show monthly means for a single January of a model integration: HadGEM (left) and CAM/ACME (right). Users can contrast similar plots from one of their simulations to confirm that their outputs appear reasonable.

## ISCCP-simulator map of total cloud cover

Calculated from the joint histogram of cloud cover as a function of cloud-top pressure and optical thickness by summing over all pc-tau bins including the bins with tau smaller 0.3 bins. Instead of observations, the quantity is compared to the model's total cloud cover field as computed by the model itself without the use of the ISCCP simulator. This is the field usually called “CLT” in CMIP archives. The comparison plot displays the difference between ISCCP total cloud cover and its model CLT field.  This comparison plot must be made for each model individually.

<p align="center"><img src="./clt_ga6.png" width=width.value><img src="./FISCCP1_COSP-CLDTOT_map.png" width="500"></p>

## ISCCP-simulator globally-averaged pc-tau joint histogram

Global area-weighted average from all points with valid data. Note that per standard practice, only points that are sunlit in the month will have data. Relative to observations, model plots have an extra optical thickness bin for tau less than 0.3.

<p align="center"><img src="./clisccp_ga6.png" width="500"><img src="./clisccp_cesm.png" width="500"></p>

## CloudSat Simulator global map of cloud volume fraction

Sum fractions over all height and reflectivity bins with reflectivity greater than -25 dBZ and divide by the number of height bins.

<p align="center"><img src="./csat_volume_fraction_ga6.png" width="500"><img src="./CFAD_DBZE94_CS_height_map3.png" width="500"></p>

## CloudSat Tropical-averaged Contoured Frequency by Altitude Diagram (CFAD)

Area-weighted average from all tropical points. Tropical points are defined as 30S to 30N. Note that model plots will have additional reflectivity bins for dBZ smaller than -25.

<p align="center"><img src="./cfadDbze94_tropics_ga6.png" width="500"><img src="./cfadDbze94_tropics_cesm.png" width="500"></p>

## MODIS-simulator global map of total cloud cover

Calculate from the joint histogram of cloud cover as a function of cloud-top pressure and optical thickness by summing over all pc-tau bins with tau greater than 0.3 bins. For the model, the sum should only be for bins with tau greater than 0.3. Observational counterpoint is “Cloud_Fraction_Mask_Total_Mean” in CFMIP-OBS dataset.

<p align="center"><img src="./cltmodis_ga6.png" width="500"><img src="./CLMODIS_map2.png" width="500"></p>

## MODIS-simulator globally-averaged pc-tau joint histogram

Global area-weighted average from all points with valid data. Note that per standard practice, only points that are sunlit in the month will have data. Relative to observations, model plots have an extra optical thickness bin for tau less than 0.3.

<p align="center"><img src="./clmodis_ga6.png" width="500"><img src="./clmodis_cesm.png" width="500"></p>

## MODIS-simulator liquid effective radius
<p align="center"><img src="./reffclwmodis_ga6.png" width="500"><img src="./reffclwmodis_ga6.png" width="500"></p>

## MODIS-simulator ice effective radius
<p align="center"><img src="./reffclimodis_ga6.png" width="500"><img src="./REFFCLIMODIS_map2.png" width="500"></p>

## MISR-simulator global map of total cloud cover

Calculate from the joint histogram of cloud cover as a function of cloud-top height and optical thickness by summing over all pc-tau bins with tau > 0.3 bins.

<p align="center"><img src="./cltmisr_ga6.png" width="500"><img src="./CLD_MISR_map2.png" width="500"></p>

## MISR-simulator globally-averaged height-tau joint histogram

Global area-weighted average from all points with valid data. Note that per standard practice, only points that are sunlit in the month will have data. Relative to observations, model plots have an extra optical thickness bin for tau less than 0.3.

<p align="center"><img src="./clMISR_ga6.png" width="500"><img src="./clMISR_cesm.png" width="500"></p>

## CALIPSO-simulator global map of total cloud cover</a>

<p align="center"><img src="./cltcalipso_ga6.png" width="500"><img src="./cltcalipso_ga6.png" width="500"></p>

## CALIPSO-simulator globally-averaged height-scattering ratio histogram (CFAD)

Global area-weighted average from all points.

<p align="center"><img src="./cfadLidarsr532_ga6.png" width="500"><img src="./cfadLidarsr532_cesm.png" width="500"></p>
