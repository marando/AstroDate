# AstroDate

#### Julian Day
```php
AstroDate::parse('2015-Jan-1')->jd  // Result: 2457023.5
```

#### Leap Seconds
```php
AstroDate::parse('2015-Jan-1')->leapSec  // Result: 35
AstroDate::parse('2015-Oct-1')->leapSec  // Result: 36
```

#### Conversion to Astronomical Time Standards

##### International Atomic (TAI)
```php
echo AstroDate::parse('2015-Jan-1')->toTAI()
```
```
Output:

2015-Jan-01 00:00:35 TAI
```

##### Terrestrial Dynamic Time (TT or TDT)
```php
echo AstroDate::parse('2015-Jan-1')->toTT()
```
```
Output:

2015-Jan-01 00:01:07.184 TT
```


##### Barycentric Dynamic Time (TDB)
```php
echo AstroDate::parse('2015-Jan-1')->toTDB()
```
```
Output:

2015-Jan-01 00:01:07.186 TDB
```





