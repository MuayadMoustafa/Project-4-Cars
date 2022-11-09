```python
import pandas as pd 
```


```python
df = pd.read_excel("C:/Users/Mua/Downloads/cars.xlsx")
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>STRING</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>CAT</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>18.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>130.0</td>
      <td>3504.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Buick Skylark 320</td>
      <td>15.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>3693.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Plymouth Satellite</td>
      <td>18.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>3436.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>4</th>
      <td>AMC Rebel SST</td>
      <td>16.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>150.0</td>
      <td>3433.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>402</th>
      <td>Ford Mustang GL</td>
      <td>27.0</td>
      <td>4</td>
      <td>140.0</td>
      <td>86.0</td>
      <td>2790.0</td>
      <td>15.6</td>
      <td>82</td>
      <td>US</td>
    </tr>
    <tr>
      <th>403</th>
      <td>Volkswagen Pickup</td>
      <td>44.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>52.0</td>
      <td>2130.0</td>
      <td>24.6</td>
      <td>82</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>404</th>
      <td>Dodge Rampage</td>
      <td>32.0</td>
      <td>4</td>
      <td>135.0</td>
      <td>84.0</td>
      <td>2295.0</td>
      <td>11.6</td>
      <td>82</td>
      <td>US</td>
    </tr>
    <tr>
      <th>405</th>
      <td>Ford Ranger</td>
      <td>28.0</td>
      <td>4</td>
      <td>120.0</td>
      <td>79.0</td>
      <td>2625.0</td>
      <td>18.6</td>
      <td>82</td>
      <td>US</td>
    </tr>
    <tr>
      <th>406</th>
      <td>Chevy S-10</td>
      <td>31.0</td>
      <td>4</td>
      <td>119.0</td>
      <td>82.0</td>
      <td>2720.0</td>
      <td>19.4</td>
      <td>82</td>
      <td>US</td>
    </tr>
  </tbody>
</table>
<p>407 rows × 9 columns</p>
</div>




```python
df.head(51)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>STRING</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>CAT</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>18.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>130.0</td>
      <td>3504.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Buick Skylark 320</td>
      <td>15.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>3693.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Plymouth Satellite</td>
      <td>18.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>3436.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>4</th>
      <td>AMC Rebel SST</td>
      <td>16.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>150.0</td>
      <td>3433.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Ford Torino</td>
      <td>17.0</td>
      <td>8</td>
      <td>302.0</td>
      <td>140.0</td>
      <td>3449.0</td>
      <td>10.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Ford Galaxie 500</td>
      <td>15.0</td>
      <td>8</td>
      <td>429.0</td>
      <td>198.0</td>
      <td>4341.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Chevrolet Impala</td>
      <td>14.0</td>
      <td>8</td>
      <td>454.0</td>
      <td>220.0</td>
      <td>4354.0</td>
      <td>9.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Plymouth Fury iii</td>
      <td>14.0</td>
      <td>8</td>
      <td>440.0</td>
      <td>215.0</td>
      <td>4312.0</td>
      <td>8.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Pontiac Catalina</td>
      <td>14.0</td>
      <td>8</td>
      <td>455.0</td>
      <td>225.0</td>
      <td>4425.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>10</th>
      <td>AMC Ambassador DPL</td>
      <td>15.0</td>
      <td>8</td>
      <td>390.0</td>
      <td>190.0</td>
      <td>3850.0</td>
      <td>8.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Citroen DS-21 Pallas</td>
      <td>0</td>
      <td>4</td>
      <td>133.0</td>
      <td>115.0</td>
      <td>3090.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Chevrolet Chevelle Concours (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>4142.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Ford Torino (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>351.0</td>
      <td>153.0</td>
      <td>4034.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Plymouth Satellite (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>383.0</td>
      <td>175.0</td>
      <td>4166.0</td>
      <td>10.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>15</th>
      <td>AMC Rebel SST (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>360.0</td>
      <td>175.0</td>
      <td>3850.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Dodge Challenger SE</td>
      <td>15.0</td>
      <td>8</td>
      <td>383.0</td>
      <td>170.0</td>
      <td>3563.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Plymouth 'Cuda 340</td>
      <td>14.0</td>
      <td>8</td>
      <td>340.0</td>
      <td>160.0</td>
      <td>3609.0</td>
      <td>8.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Ford Mustang Boss 302</td>
      <td>0</td>
      <td>8</td>
      <td>302.0</td>
      <td>140.0</td>
      <td>3353.0</td>
      <td>8.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Chevrolet Monte Carlo</td>
      <td>15.0</td>
      <td>8</td>
      <td>400.0</td>
      <td>150.0</td>
      <td>3761.0</td>
      <td>9.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Buick Estate Wagon (sw)</td>
      <td>14.0</td>
      <td>8</td>
      <td>455.0</td>
      <td>225.0</td>
      <td>3086.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Toyota Corolla Mark ii</td>
      <td>24.0</td>
      <td>4</td>
      <td>113.0</td>
      <td>95.0</td>
      <td>2372.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Plymouth Duster</td>
      <td>22.0</td>
      <td>6</td>
      <td>198.0</td>
      <td>95.0</td>
      <td>2833.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>23</th>
      <td>AMC Hornet</td>
      <td>18.0</td>
      <td>6</td>
      <td>199.0</td>
      <td>97.0</td>
      <td>2774.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Ford Maverick</td>
      <td>21.0</td>
      <td>6</td>
      <td>200.0</td>
      <td>85.0</td>
      <td>2587.0</td>
      <td>16.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Datsun PL510</td>
      <td>27.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>88.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>70</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Volkswagen 1131 Deluxe Sedan</td>
      <td>26.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>46.0</td>
      <td>1835.0</td>
      <td>20.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Peugeot 504</td>
      <td>25.0</td>
      <td>4</td>
      <td>110.0</td>
      <td>87.0</td>
      <td>2672.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Audi 100 LS</td>
      <td>24.0</td>
      <td>4</td>
      <td>107.0</td>
      <td>90.0</td>
      <td>2430.0</td>
      <td>14.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Saab 99e</td>
      <td>25.0</td>
      <td>4</td>
      <td>104.0</td>
      <td>95.0</td>
      <td>2375.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>30</th>
      <td>BMW 2002</td>
      <td>26.0</td>
      <td>4</td>
      <td>121.0</td>
      <td>113.0</td>
      <td>2234.0</td>
      <td>12.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>31</th>
      <td>AMC Gremlin</td>
      <td>21.0</td>
      <td>6</td>
      <td>199.0</td>
      <td>90.0</td>
      <td>2648.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Ford F250</td>
      <td>10.0</td>
      <td>8</td>
      <td>360.0</td>
      <td>215.0</td>
      <td>4615.0</td>
      <td>14.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>33</th>
      <td>Chevy C20</td>
      <td>10.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>200.0</td>
      <td>4376.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Dodge D200</td>
      <td>11.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>210.0</td>
      <td>4382.0</td>
      <td>13.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>35</th>
      <td>Hi 1200D</td>
      <td>9.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>193.0</td>
      <td>4732.0</td>
      <td>18.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>36</th>
      <td>Datsun PL510</td>
      <td>27.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>88.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>71</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>37</th>
      <td>Chevrolet Vega 2300</td>
      <td>28.0</td>
      <td>4</td>
      <td>140.0</td>
      <td>90.0</td>
      <td>2264.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>38</th>
      <td>Toyota Corolla</td>
      <td>25.0</td>
      <td>4</td>
      <td>113.0</td>
      <td>95.0</td>
      <td>2228.0</td>
      <td>14.0</td>
      <td>71</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>39</th>
      <td>Ford Pinto</td>
      <td>25.0</td>
      <td>4</td>
      <td>98.0</td>
      <td>0</td>
      <td>2046.0</td>
      <td>19.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>40</th>
      <td>Volkswagen Super Beetle 117</td>
      <td>0</td>
      <td>4</td>
      <td>97.0</td>
      <td>48.0</td>
      <td>1978.0</td>
      <td>20.0</td>
      <td>71</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>41</th>
      <td>AMC Gremlin</td>
      <td>19.0</td>
      <td>6</td>
      <td>232.0</td>
      <td>100.0</td>
      <td>2634.0</td>
      <td>13.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>42</th>
      <td>Plymouth Satellite Custom</td>
      <td>16.0</td>
      <td>6</td>
      <td>225.0</td>
      <td>105.0</td>
      <td>3439.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>43</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>17.0</td>
      <td>6</td>
      <td>250.0</td>
      <td>100.0</td>
      <td>3329.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>44</th>
      <td>Ford Torino 500</td>
      <td>19.0</td>
      <td>6</td>
      <td>250.0</td>
      <td>88.0</td>
      <td>3302.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>45</th>
      <td>AMC Matador</td>
      <td>18.0</td>
      <td>6</td>
      <td>232.0</td>
      <td>100.0</td>
      <td>3288.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Chevrolet Impala</td>
      <td>14.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>4209.0</td>
      <td>12.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>47</th>
      <td>Pontiac Catalina Brougham</td>
      <td>14.0</td>
      <td>8</td>
      <td>400.0</td>
      <td>175.0</td>
      <td>4464.0</td>
      <td>11.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>48</th>
      <td>Ford Galaxie 500</td>
      <td>14.0</td>
      <td>8</td>
      <td>351.0</td>
      <td>153.0</td>
      <td>4154.0</td>
      <td>13.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>49</th>
      <td>Plymouth Fury iii</td>
      <td>14.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>4096.0</td>
      <td>13.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Dodge Monaco (sw)</td>
      <td>12.0</td>
      <td>8</td>
      <td>383.0</td>
      <td>180.0</td>
      <td>4955.0</td>
      <td>11.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff = df.head(51)
dff
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>STRING</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>CAT</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>18.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>130.0</td>
      <td>3504.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Buick Skylark 320</td>
      <td>15.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>3693.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Plymouth Satellite</td>
      <td>18.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>3436.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>4</th>
      <td>AMC Rebel SST</td>
      <td>16.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>150.0</td>
      <td>3433.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Ford Torino</td>
      <td>17.0</td>
      <td>8</td>
      <td>302.0</td>
      <td>140.0</td>
      <td>3449.0</td>
      <td>10.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Ford Galaxie 500</td>
      <td>15.0</td>
      <td>8</td>
      <td>429.0</td>
      <td>198.0</td>
      <td>4341.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Chevrolet Impala</td>
      <td>14.0</td>
      <td>8</td>
      <td>454.0</td>
      <td>220.0</td>
      <td>4354.0</td>
      <td>9.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Plymouth Fury iii</td>
      <td>14.0</td>
      <td>8</td>
      <td>440.0</td>
      <td>215.0</td>
      <td>4312.0</td>
      <td>8.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Pontiac Catalina</td>
      <td>14.0</td>
      <td>8</td>
      <td>455.0</td>
      <td>225.0</td>
      <td>4425.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>10</th>
      <td>AMC Ambassador DPL</td>
      <td>15.0</td>
      <td>8</td>
      <td>390.0</td>
      <td>190.0</td>
      <td>3850.0</td>
      <td>8.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Citroen DS-21 Pallas</td>
      <td>0</td>
      <td>4</td>
      <td>133.0</td>
      <td>115.0</td>
      <td>3090.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Chevrolet Chevelle Concours (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>4142.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Ford Torino (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>351.0</td>
      <td>153.0</td>
      <td>4034.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Plymouth Satellite (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>383.0</td>
      <td>175.0</td>
      <td>4166.0</td>
      <td>10.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>15</th>
      <td>AMC Rebel SST (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>360.0</td>
      <td>175.0</td>
      <td>3850.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Dodge Challenger SE</td>
      <td>15.0</td>
      <td>8</td>
      <td>383.0</td>
      <td>170.0</td>
      <td>3563.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Plymouth 'Cuda 340</td>
      <td>14.0</td>
      <td>8</td>
      <td>340.0</td>
      <td>160.0</td>
      <td>3609.0</td>
      <td>8.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Ford Mustang Boss 302</td>
      <td>0</td>
      <td>8</td>
      <td>302.0</td>
      <td>140.0</td>
      <td>3353.0</td>
      <td>8.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Chevrolet Monte Carlo</td>
      <td>15.0</td>
      <td>8</td>
      <td>400.0</td>
      <td>150.0</td>
      <td>3761.0</td>
      <td>9.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Buick Estate Wagon (sw)</td>
      <td>14.0</td>
      <td>8</td>
      <td>455.0</td>
      <td>225.0</td>
      <td>3086.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Toyota Corolla Mark ii</td>
      <td>24.0</td>
      <td>4</td>
      <td>113.0</td>
      <td>95.0</td>
      <td>2372.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Plymouth Duster</td>
      <td>22.0</td>
      <td>6</td>
      <td>198.0</td>
      <td>95.0</td>
      <td>2833.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>23</th>
      <td>AMC Hornet</td>
      <td>18.0</td>
      <td>6</td>
      <td>199.0</td>
      <td>97.0</td>
      <td>2774.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Ford Maverick</td>
      <td>21.0</td>
      <td>6</td>
      <td>200.0</td>
      <td>85.0</td>
      <td>2587.0</td>
      <td>16.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Datsun PL510</td>
      <td>27.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>88.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>70</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Volkswagen 1131 Deluxe Sedan</td>
      <td>26.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>46.0</td>
      <td>1835.0</td>
      <td>20.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Peugeot 504</td>
      <td>25.0</td>
      <td>4</td>
      <td>110.0</td>
      <td>87.0</td>
      <td>2672.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Audi 100 LS</td>
      <td>24.0</td>
      <td>4</td>
      <td>107.0</td>
      <td>90.0</td>
      <td>2430.0</td>
      <td>14.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Saab 99e</td>
      <td>25.0</td>
      <td>4</td>
      <td>104.0</td>
      <td>95.0</td>
      <td>2375.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>30</th>
      <td>BMW 2002</td>
      <td>26.0</td>
      <td>4</td>
      <td>121.0</td>
      <td>113.0</td>
      <td>2234.0</td>
      <td>12.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>31</th>
      <td>AMC Gremlin</td>
      <td>21.0</td>
      <td>6</td>
      <td>199.0</td>
      <td>90.0</td>
      <td>2648.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Ford F250</td>
      <td>10.0</td>
      <td>8</td>
      <td>360.0</td>
      <td>215.0</td>
      <td>4615.0</td>
      <td>14.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>33</th>
      <td>Chevy C20</td>
      <td>10.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>200.0</td>
      <td>4376.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Dodge D200</td>
      <td>11.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>210.0</td>
      <td>4382.0</td>
      <td>13.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>35</th>
      <td>Hi 1200D</td>
      <td>9.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>193.0</td>
      <td>4732.0</td>
      <td>18.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>36</th>
      <td>Datsun PL510</td>
      <td>27.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>88.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>71</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>37</th>
      <td>Chevrolet Vega 2300</td>
      <td>28.0</td>
      <td>4</td>
      <td>140.0</td>
      <td>90.0</td>
      <td>2264.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>38</th>
      <td>Toyota Corolla</td>
      <td>25.0</td>
      <td>4</td>
      <td>113.0</td>
      <td>95.0</td>
      <td>2228.0</td>
      <td>14.0</td>
      <td>71</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>39</th>
      <td>Ford Pinto</td>
      <td>25.0</td>
      <td>4</td>
      <td>98.0</td>
      <td>0</td>
      <td>2046.0</td>
      <td>19.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>40</th>
      <td>Volkswagen Super Beetle 117</td>
      <td>0</td>
      <td>4</td>
      <td>97.0</td>
      <td>48.0</td>
      <td>1978.0</td>
      <td>20.0</td>
      <td>71</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>41</th>
      <td>AMC Gremlin</td>
      <td>19.0</td>
      <td>6</td>
      <td>232.0</td>
      <td>100.0</td>
      <td>2634.0</td>
      <td>13.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>42</th>
      <td>Plymouth Satellite Custom</td>
      <td>16.0</td>
      <td>6</td>
      <td>225.0</td>
      <td>105.0</td>
      <td>3439.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>43</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>17.0</td>
      <td>6</td>
      <td>250.0</td>
      <td>100.0</td>
      <td>3329.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>44</th>
      <td>Ford Torino 500</td>
      <td>19.0</td>
      <td>6</td>
      <td>250.0</td>
      <td>88.0</td>
      <td>3302.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>45</th>
      <td>AMC Matador</td>
      <td>18.0</td>
      <td>6</td>
      <td>232.0</td>
      <td>100.0</td>
      <td>3288.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Chevrolet Impala</td>
      <td>14.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>4209.0</td>
      <td>12.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>47</th>
      <td>Pontiac Catalina Brougham</td>
      <td>14.0</td>
      <td>8</td>
      <td>400.0</td>
      <td>175.0</td>
      <td>4464.0</td>
      <td>11.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>48</th>
      <td>Ford Galaxie 500</td>
      <td>14.0</td>
      <td>8</td>
      <td>351.0</td>
      <td>153.0</td>
      <td>4154.0</td>
      <td>13.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>49</th>
      <td>Plymouth Fury iii</td>
      <td>14.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>4096.0</td>
      <td>13.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Dodge Monaco (sw)</td>
      <td>12.0</td>
      <td>8</td>
      <td>383.0</td>
      <td>180.0</td>
      <td>4955.0</td>
      <td>11.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff.describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>51</td>
      <td>51.0</td>
      <td>51</td>
      <td>51.0</td>
      <td>51.0</td>
      <td>51.0</td>
      <td>51.0</td>
      <td>51</td>
      <td>51</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>45</td>
      <td>19.0</td>
      <td>4</td>
      <td>31.0</td>
      <td>31.0</td>
      <td>49.0</td>
      <td>23.0</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>top</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>14.0</td>
      <td>8</td>
      <td>97.0</td>
      <td>95.0</td>
      <td>2130.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>2</td>
      <td>9.0</td>
      <td>28</td>
      <td>4.0</td>
      <td>4.0</td>
      <td>2.0</td>
      <td>7.0</td>
      <td>35</td>
      <td>39</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff.mode()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>AMC Gremlin</td>
      <td>14.0</td>
      <td>8</td>
      <td>97.0</td>
      <td>95.0</td>
      <td>2130.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>150.0</td>
      <td>3850.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Chevrolet Impala</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Datsun PL510</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Ford Galaxie 500</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Plymouth Fury iii</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.describe()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>407</td>
      <td>407.0</td>
      <td>407</td>
      <td>407.0</td>
      <td>407.0</td>
      <td>407.0</td>
      <td>407.0</td>
      <td>407</td>
      <td>407</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>309</td>
      <td>131.0</td>
      <td>6</td>
      <td>84.0</td>
      <td>95.0</td>
      <td>357.0</td>
      <td>97.0</td>
      <td>14</td>
      <td>4</td>
    </tr>
    <tr>
      <th>top</th>
      <td>Toyota Corolla</td>
      <td>13.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>150.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>73</td>
      <td>US</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>9</td>
      <td>20.0</td>
      <td>207</td>
      <td>22.0</td>
      <td>22.0</td>
      <td>4.0</td>
      <td>23.0</td>
      <td>40</td>
      <td>254</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff[["MPG","Acceleration"]]
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>MPG</th>
      <th>Acceleration</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
    </tr>
    <tr>
      <th>1</th>
      <td>18.0</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>15.0</td>
      <td>11.5</td>
    </tr>
    <tr>
      <th>3</th>
      <td>18.0</td>
      <td>11.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>16.0</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>17.0</td>
      <td>10.5</td>
    </tr>
    <tr>
      <th>6</th>
      <td>15.0</td>
      <td>10.0</td>
    </tr>
    <tr>
      <th>7</th>
      <td>14.0</td>
      <td>9.0</td>
    </tr>
    <tr>
      <th>8</th>
      <td>14.0</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>9</th>
      <td>14.0</td>
      <td>10.0</td>
    </tr>
    <tr>
      <th>10</th>
      <td>15.0</td>
      <td>8.5</td>
    </tr>
    <tr>
      <th>11</th>
      <td>0</td>
      <td>17.5</td>
    </tr>
    <tr>
      <th>12</th>
      <td>0</td>
      <td>11.5</td>
    </tr>
    <tr>
      <th>13</th>
      <td>0</td>
      <td>11.0</td>
    </tr>
    <tr>
      <th>14</th>
      <td>0</td>
      <td>10.5</td>
    </tr>
    <tr>
      <th>15</th>
      <td>0</td>
      <td>11.0</td>
    </tr>
    <tr>
      <th>16</th>
      <td>15.0</td>
      <td>10.0</td>
    </tr>
    <tr>
      <th>17</th>
      <td>14.0</td>
      <td>8.0</td>
    </tr>
    <tr>
      <th>18</th>
      <td>0</td>
      <td>8.0</td>
    </tr>
    <tr>
      <th>19</th>
      <td>15.0</td>
      <td>9.5</td>
    </tr>
    <tr>
      <th>20</th>
      <td>14.0</td>
      <td>10.0</td>
    </tr>
    <tr>
      <th>21</th>
      <td>24.0</td>
      <td>15.0</td>
    </tr>
    <tr>
      <th>22</th>
      <td>22.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>23</th>
      <td>18.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>24</th>
      <td>21.0</td>
      <td>16.0</td>
    </tr>
    <tr>
      <th>25</th>
      <td>27.0</td>
      <td>14.5</td>
    </tr>
    <tr>
      <th>26</th>
      <td>26.0</td>
      <td>20.5</td>
    </tr>
    <tr>
      <th>27</th>
      <td>25.0</td>
      <td>17.5</td>
    </tr>
    <tr>
      <th>28</th>
      <td>24.0</td>
      <td>14.5</td>
    </tr>
    <tr>
      <th>29</th>
      <td>25.0</td>
      <td>17.5</td>
    </tr>
    <tr>
      <th>30</th>
      <td>26.0</td>
      <td>12.5</td>
    </tr>
    <tr>
      <th>31</th>
      <td>21.0</td>
      <td>15.0</td>
    </tr>
    <tr>
      <th>32</th>
      <td>10.0</td>
      <td>14.0</td>
    </tr>
    <tr>
      <th>33</th>
      <td>10.0</td>
      <td>15.0</td>
    </tr>
    <tr>
      <th>34</th>
      <td>11.0</td>
      <td>13.5</td>
    </tr>
    <tr>
      <th>35</th>
      <td>9.0</td>
      <td>18.5</td>
    </tr>
    <tr>
      <th>36</th>
      <td>27.0</td>
      <td>14.5</td>
    </tr>
    <tr>
      <th>37</th>
      <td>28.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>38</th>
      <td>25.0</td>
      <td>14.0</td>
    </tr>
    <tr>
      <th>39</th>
      <td>25.0</td>
      <td>19.0</td>
    </tr>
    <tr>
      <th>40</th>
      <td>0</td>
      <td>20.0</td>
    </tr>
    <tr>
      <th>41</th>
      <td>19.0</td>
      <td>13.0</td>
    </tr>
    <tr>
      <th>42</th>
      <td>16.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>43</th>
      <td>17.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>44</th>
      <td>19.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>45</th>
      <td>18.0</td>
      <td>15.5</td>
    </tr>
    <tr>
      <th>46</th>
      <td>14.0</td>
      <td>12.0</td>
    </tr>
    <tr>
      <th>47</th>
      <td>14.0</td>
      <td>11.5</td>
    </tr>
    <tr>
      <th>48</th>
      <td>14.0</td>
      <td>13.5</td>
    </tr>
    <tr>
      <th>49</th>
      <td>14.0</td>
      <td>13.0</td>
    </tr>
    <tr>
      <th>50</th>
      <td>12.0</td>
      <td>11.5</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.count()
```




    Car             407
    MPG             407
    Cylinders       407
    Displacement    407
    Horsepower      407
    Weight          407
    Acceleration    407
    Model           407
    Origin          407
    dtype: int64




```python
dff.count()
```




    Car             51
    MPG             51
    Cylinders       51
    Displacement    51
    Horsepower      51
    Weight          51
    Acceleration    51
    Model           51
    Origin          51
    dtype: int64




```python
dff["Model"].mean
```




    <bound method NDFrame._add_numeric_operations.<locals>.mean of 0     INT
    1      70
    2      70
    3      70
    4      70
    5      70
    6      70
    7      70
    8      70
    9      70
    10     70
    11     70
    12     70
    13     70
    14     70
    15     70
    16     70
    17     70
    18     70
    19     70
    20     70
    21     70
    22     70
    23     70
    24     70
    25     70
    26     70
    27     70
    28     70
    29     70
    30     70
    31     70
    32     70
    33     70
    34     70
    35     70
    36     71
    37     71
    38     71
    39     71
    40     71
    41     71
    42     71
    43     71
    44     71
    45     71
    46     71
    47     71
    48     71
    49     71
    50     71
    Name: Model, dtype: object>




```python
dff
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Car</th>
      <th>MPG</th>
      <th>Cylinders</th>
      <th>Displacement</th>
      <th>Horsepower</th>
      <th>Weight</th>
      <th>Acceleration</th>
      <th>Model</th>
      <th>Origin</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>STRING</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>DOUBLE</td>
      <td>INT</td>
      <td>CAT</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>18.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>130.0</td>
      <td>3504.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Buick Skylark 320</td>
      <td>15.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>3693.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Plymouth Satellite</td>
      <td>18.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>3436.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>4</th>
      <td>AMC Rebel SST</td>
      <td>16.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>150.0</td>
      <td>3433.0</td>
      <td>12.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Ford Torino</td>
      <td>17.0</td>
      <td>8</td>
      <td>302.0</td>
      <td>140.0</td>
      <td>3449.0</td>
      <td>10.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Ford Galaxie 500</td>
      <td>15.0</td>
      <td>8</td>
      <td>429.0</td>
      <td>198.0</td>
      <td>4341.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Chevrolet Impala</td>
      <td>14.0</td>
      <td>8</td>
      <td>454.0</td>
      <td>220.0</td>
      <td>4354.0</td>
      <td>9.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Plymouth Fury iii</td>
      <td>14.0</td>
      <td>8</td>
      <td>440.0</td>
      <td>215.0</td>
      <td>4312.0</td>
      <td>8.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Pontiac Catalina</td>
      <td>14.0</td>
      <td>8</td>
      <td>455.0</td>
      <td>225.0</td>
      <td>4425.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>10</th>
      <td>AMC Ambassador DPL</td>
      <td>15.0</td>
      <td>8</td>
      <td>390.0</td>
      <td>190.0</td>
      <td>3850.0</td>
      <td>8.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Citroen DS-21 Pallas</td>
      <td>0</td>
      <td>4</td>
      <td>133.0</td>
      <td>115.0</td>
      <td>3090.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Chevrolet Chevelle Concours (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>4142.0</td>
      <td>11.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Ford Torino (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>351.0</td>
      <td>153.0</td>
      <td>4034.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Plymouth Satellite (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>383.0</td>
      <td>175.0</td>
      <td>4166.0</td>
      <td>10.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>15</th>
      <td>AMC Rebel SST (sw)</td>
      <td>0</td>
      <td>8</td>
      <td>360.0</td>
      <td>175.0</td>
      <td>3850.0</td>
      <td>11.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Dodge Challenger SE</td>
      <td>15.0</td>
      <td>8</td>
      <td>383.0</td>
      <td>170.0</td>
      <td>3563.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Plymouth 'Cuda 340</td>
      <td>14.0</td>
      <td>8</td>
      <td>340.0</td>
      <td>160.0</td>
      <td>3609.0</td>
      <td>8.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Ford Mustang Boss 302</td>
      <td>0</td>
      <td>8</td>
      <td>302.0</td>
      <td>140.0</td>
      <td>3353.0</td>
      <td>8.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Chevrolet Monte Carlo</td>
      <td>15.0</td>
      <td>8</td>
      <td>400.0</td>
      <td>150.0</td>
      <td>3761.0</td>
      <td>9.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Buick Estate Wagon (sw)</td>
      <td>14.0</td>
      <td>8</td>
      <td>455.0</td>
      <td>225.0</td>
      <td>3086.0</td>
      <td>10.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Toyota Corolla Mark ii</td>
      <td>24.0</td>
      <td>4</td>
      <td>113.0</td>
      <td>95.0</td>
      <td>2372.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Plymouth Duster</td>
      <td>22.0</td>
      <td>6</td>
      <td>198.0</td>
      <td>95.0</td>
      <td>2833.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>23</th>
      <td>AMC Hornet</td>
      <td>18.0</td>
      <td>6</td>
      <td>199.0</td>
      <td>97.0</td>
      <td>2774.0</td>
      <td>15.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Ford Maverick</td>
      <td>21.0</td>
      <td>6</td>
      <td>200.0</td>
      <td>85.0</td>
      <td>2587.0</td>
      <td>16.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Datsun PL510</td>
      <td>27.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>88.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>70</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Volkswagen 1131 Deluxe Sedan</td>
      <td>26.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>46.0</td>
      <td>1835.0</td>
      <td>20.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Peugeot 504</td>
      <td>25.0</td>
      <td>4</td>
      <td>110.0</td>
      <td>87.0</td>
      <td>2672.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Audi 100 LS</td>
      <td>24.0</td>
      <td>4</td>
      <td>107.0</td>
      <td>90.0</td>
      <td>2430.0</td>
      <td>14.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Saab 99e</td>
      <td>25.0</td>
      <td>4</td>
      <td>104.0</td>
      <td>95.0</td>
      <td>2375.0</td>
      <td>17.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>30</th>
      <td>BMW 2002</td>
      <td>26.0</td>
      <td>4</td>
      <td>121.0</td>
      <td>113.0</td>
      <td>2234.0</td>
      <td>12.5</td>
      <td>70</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>31</th>
      <td>AMC Gremlin</td>
      <td>21.0</td>
      <td>6</td>
      <td>199.0</td>
      <td>90.0</td>
      <td>2648.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Ford F250</td>
      <td>10.0</td>
      <td>8</td>
      <td>360.0</td>
      <td>215.0</td>
      <td>4615.0</td>
      <td>14.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>33</th>
      <td>Chevy C20</td>
      <td>10.0</td>
      <td>8</td>
      <td>307.0</td>
      <td>200.0</td>
      <td>4376.0</td>
      <td>15.0</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Dodge D200</td>
      <td>11.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>210.0</td>
      <td>4382.0</td>
      <td>13.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>35</th>
      <td>Hi 1200D</td>
      <td>9.0</td>
      <td>8</td>
      <td>304.0</td>
      <td>193.0</td>
      <td>4732.0</td>
      <td>18.5</td>
      <td>70</td>
      <td>US</td>
    </tr>
    <tr>
      <th>36</th>
      <td>Datsun PL510</td>
      <td>27.0</td>
      <td>4</td>
      <td>97.0</td>
      <td>88.0</td>
      <td>2130.0</td>
      <td>14.5</td>
      <td>71</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>37</th>
      <td>Chevrolet Vega 2300</td>
      <td>28.0</td>
      <td>4</td>
      <td>140.0</td>
      <td>90.0</td>
      <td>2264.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>38</th>
      <td>Toyota Corolla</td>
      <td>25.0</td>
      <td>4</td>
      <td>113.0</td>
      <td>95.0</td>
      <td>2228.0</td>
      <td>14.0</td>
      <td>71</td>
      <td>Japan</td>
    </tr>
    <tr>
      <th>39</th>
      <td>Ford Pinto</td>
      <td>25.0</td>
      <td>4</td>
      <td>98.0</td>
      <td>0</td>
      <td>2046.0</td>
      <td>19.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>40</th>
      <td>Volkswagen Super Beetle 117</td>
      <td>0</td>
      <td>4</td>
      <td>97.0</td>
      <td>48.0</td>
      <td>1978.0</td>
      <td>20.0</td>
      <td>71</td>
      <td>Europe</td>
    </tr>
    <tr>
      <th>41</th>
      <td>AMC Gremlin</td>
      <td>19.0</td>
      <td>6</td>
      <td>232.0</td>
      <td>100.0</td>
      <td>2634.0</td>
      <td>13.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>42</th>
      <td>Plymouth Satellite Custom</td>
      <td>16.0</td>
      <td>6</td>
      <td>225.0</td>
      <td>105.0</td>
      <td>3439.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>43</th>
      <td>Chevrolet Chevelle Malibu</td>
      <td>17.0</td>
      <td>6</td>
      <td>250.0</td>
      <td>100.0</td>
      <td>3329.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>44</th>
      <td>Ford Torino 500</td>
      <td>19.0</td>
      <td>6</td>
      <td>250.0</td>
      <td>88.0</td>
      <td>3302.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>45</th>
      <td>AMC Matador</td>
      <td>18.0</td>
      <td>6</td>
      <td>232.0</td>
      <td>100.0</td>
      <td>3288.0</td>
      <td>15.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Chevrolet Impala</td>
      <td>14.0</td>
      <td>8</td>
      <td>350.0</td>
      <td>165.0</td>
      <td>4209.0</td>
      <td>12.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>47</th>
      <td>Pontiac Catalina Brougham</td>
      <td>14.0</td>
      <td>8</td>
      <td>400.0</td>
      <td>175.0</td>
      <td>4464.0</td>
      <td>11.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>48</th>
      <td>Ford Galaxie 500</td>
      <td>14.0</td>
      <td>8</td>
      <td>351.0</td>
      <td>153.0</td>
      <td>4154.0</td>
      <td>13.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>49</th>
      <td>Plymouth Fury iii</td>
      <td>14.0</td>
      <td>8</td>
      <td>318.0</td>
      <td>150.0</td>
      <td>4096.0</td>
      <td>13.0</td>
      <td>71</td>
      <td>US</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Dodge Monaco (sw)</td>
      <td>12.0</td>
      <td>8</td>
      <td>383.0</td>
      <td>180.0</td>
      <td>4955.0</td>
      <td>11.5</td>
      <td>71</td>
      <td>US</td>
    </tr>
  </tbody>
</table>
</div>




```python
dff["Car"]
```




    0                               STRING
    1            Chevrolet Chevelle Malibu
    2                    Buick Skylark 320
    3                   Plymouth Satellite
    4                        AMC Rebel SST
    5                          Ford Torino
    6                     Ford Galaxie 500
    7                     Chevrolet Impala
    8                    Plymouth Fury iii
    9                     Pontiac Catalina
    10                  AMC Ambassador DPL
    11                Citroen DS-21 Pallas
    12    Chevrolet Chevelle Concours (sw)
    13                    Ford Torino (sw)
    14             Plymouth Satellite (sw)
    15                  AMC Rebel SST (sw)
    16                 Dodge Challenger SE
    17                  Plymouth 'Cuda 340
    18               Ford Mustang Boss 302
    19               Chevrolet Monte Carlo
    20             Buick Estate Wagon (sw)
    21              Toyota Corolla Mark ii
    22                     Plymouth Duster
    23                          AMC Hornet
    24                       Ford Maverick
    25                        Datsun PL510
    26        Volkswagen 1131 Deluxe Sedan
    27                         Peugeot 504
    28                         Audi 100 LS
    29                            Saab 99e
    30                            BMW 2002
    31                         AMC Gremlin
    32                           Ford F250
    33                           Chevy C20
    34                          Dodge D200
    35                            Hi 1200D
    36                        Datsun PL510
    37                 Chevrolet Vega 2300
    38                      Toyota Corolla
    39                          Ford Pinto
    40         Volkswagen Super Beetle 117
    41                         AMC Gremlin
    42           Plymouth Satellite Custom
    43           Chevrolet Chevelle Malibu
    44                     Ford Torino 500
    45                         AMC Matador
    46                    Chevrolet Impala
    47           Pontiac Catalina Brougham
    48                    Ford Galaxie 500
    49                   Plymouth Fury iii
    50                   Dodge Monaco (sw)
    Name: Car, dtype: object




```python

```
