﻿# Byte.From
Creates a 8-bit integer from the given value.
***
function (optional value as nullable any, optional culture as nullable any, optional roundingMode as nullable any) as nullable any
***
# Descrition 
Returns a 8-bit integer <code>number</code> value from the given <code>value</code>. If the given <code>value</code> is <code>null</code>, <code>Byte.From</code> returns <code>null</code>.  If the given <code>value</code> is <code>number</code> within the range of 8-bit integer without a fractional part, <code>value</code> is returned. If it has fractional part, then the number is rounded with the rounding mode specified. The default rounding mode is <code>RoundingMode.ToEven</code>. If the given <code>value</code> is of any other type, see <code>Number.FromText</code> for converting it to <code>number</code> value, then the previous statement about converting <code>number</code> value to 8-bit integer <code>number</code> value applies.See <code>Number.Round</code> for the available rounding modes.
# Category 
Number.Conversion and formatting
# Examples 
Get the 8-bit integer <code>number</code> value of <code>"4"</code>.
```
Byte.From("4")
```
> 4
***
Get the 8-bit integer <code>number</code> value of <code>"4.5"</code> using <code>RoundingMode.AwayFromZero</code>.
```
Byte.From("4.5", null, RoundingMode.AwayFromZero)
```
> 5
***