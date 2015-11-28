## Types

### 1.1 DateTime *type*
 
All timestamps are formatted as string(25) using the combined date and time format from the ISO 8601 standard. The absence of the timezone designator implies a UTC timestamp.


Example:

    2015-06-29T22:39:09+02:00
    2015-06-29T20:39:09Z
    2015-06-29T20:39:09

    
### 1.2 Decimal *type*

Decimals are formatted as strings following JSON's number format. They are explicitly expressed as strings to make it clear that they should be interpreted as exact decimals and not as floating points or doubles.

Example:

    "0.68"
    "3.1415"

    
### 1.3 DimensionType *enum*

| Value        | Description                                          |
| ------------ | ---------------------------------------------------- |
| energy       | defined in kWh, default division is 1 Wh             |
| flat         | flat fee, no unit                                    |
| max_current  | defined in A (Ampere), Maximum current               |
| min_current  | defined in A (Ampere), Minimum current               |
| parking_time | defined in hours, default division is 1 second       |
| time         | defined in hours, default division is 1 second       |


### 1.4 URL *type*

An URL a string(255) type following the [w3.org spec](http://www.w3.org/Addressing/URL/uri-spec.html).