<h1 style="text-align: center;">Climate Change and Its Consequences</h1>

## Introduction

Climate change, in the broadest sense, refers to long term changes in weather and temperature patterns. Throughout almost all of Earth’s history, changes in Earth’s climate are attributed to a variety of natural factors. Some of these factors include changes in solar irradiance caused by the Earth’s orbit, the Sun’s 11 year solar cycle, and volcanic eruptions. These factors contribute to a natural cycle of global warming and cooling which occur in different intensities spanning multiple millenia.

Since the 1800s, however, the Earth has experienced a global warming event which is occurring at an unprecedented rate, far exceeding warming events earlier in the Earth’s history. Between 1901 and 2020, global temperatures rose by 1.98°F (1.1°C), with the 2010s being the warmest decade on record. Nearly universal consensus among scientists points to CO2 emissions caused by the burning of fossil fuels by humans as the primary cause of global warming.

Global increases in temperature will affect the Earth in a myriad of ways. Global sea levels will increase due to the melting of glaciers, Greenland and Antarctica ice sheets, and Arctic sea ice. Heat waves and droughts will occur more frequently and more severely, leading to increasingly intense wildfires and desertification. Consequently, these droughts will increase the amount of water vapor in the atmosphere, leading some areas to experience more intense precipitation and flooding.

It is incredibly important to study and address the effects of global warming, as human suffering will be increasingly widespread. Increasingly severe weather events will not only damage critical infrastructure, but will result in injuries, death, and the spread of disease. Higher temperatures will not only put crops and bodies of freshwater at risk, but will also prevent humans from working outdoors as the wet-bulb temperature will stop our bodies from adequately cooling. Lastly, climate change will hit poor countries more severely since many poor communities rely more on subsistence agriculture, which will result in mass displacement and famine.

This tutorial will cover the data science lifecycle, which will allow us to analyze the data and science regarding climate change and its consequences. There will be five major sections:

1. [Data Collection](#data-collection)
2. [Data Processing](#data-processing)
3. [Exploratory Analysis and Data Visualization](#exploratory-analysis-and-data-visualization)
4. [Model: Analysis, Hypothesis Testing, and Machine Learning](#model-analysis-hypothesis-testing-and-machine-learning)
5. [Interpretation: Insight and Policy Decision](#interpretation-insight-and-policy-decision)


## Data Collection




```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
```

## Data Processing


```python
def remove_monthly_CO2_columns(monthly_co2):
    del monthly_co2['ObjectId']
    del monthly_co2['Country']
    del monthly_co2['ISO2']
    del monthly_co2['ISO3']
    del monthly_co2['Indicator']
    del monthly_co2['Unit']
    del monthly_co2['Source']
    del monthly_co2['CTS_Name']
    del monthly_co2['CTS_Full_Descriptor']
    del monthly_co2['CTS_Code']
    return monthly_co2
```


```python
def extract_monthly_CO2_percents(monthly_co2):
    print("hello")
```


```python
# Monthly CO2 readings
monthly_co2 = pd.read_csv("Atmospheric_CO2_Concentrations.csv")
monthly_co2 = remove_monthly_CO2_columns(monthly_co2)
print(monthly_co2.head(20))
```

           Date   Value
    0   1958M03  315.70
    1   1958M04  317.45
    2   1958M05  317.51
    3   1958M06  317.24
    4   1958M07  315.86
    5   1958M08  314.93
    6   1958M09  313.20
    7   1958M10  312.43
    8   1958M11  313.33
    9   1958M12  314.67
    10  1959M01  315.58
    11  1959M02  316.48
    12  1959M03  316.65
    13  1959M03    0.30
    14  1959M04  317.72
    15  1959M04    0.09
    16  1959M05  318.29
    17  1959M05    0.25
    18  1959M06  318.15
    19  1959M06    0.29
    

## Exploratory Analysis and Data Visualization

## Model: Analysis, Hypothesis Testing, and Machine Learning

## Interpretation: Insight and Policy Decision


```python
# Ice Sheets
```
