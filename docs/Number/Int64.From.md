# Int64.From
Creates a 64-bit integer from the given value.
> _function (optional <code>value</code> as nullable any, optional <code>culture</code> as nullable any, optional <code>roundingMode</code> as nullable any) as nullable any_

# Description 
Returns a 64-bit integer <code>number</code> value from the given <code>value</code>. If the given <code>value</code> is <code>null</code>, <code>Int64.From</code> returns <code>null</code>.  If the given <code>value</code> is <code>number</code> within the range of 64-bit integer without a fractional part, <code>value</code> is returned. If it has fractional part, then the number is rounded with the rounding mode specified. The default rounding mode is <code>RoundingMode.ToEven</code>. If the given <code>value</code> is of any other type, see <code>Number.FromText</code> for converting it to <code>number</code> value, then the previous statement about converting <code>number</code> value to 64-bit integer <code>number</code> value applies. See <code>Number.Round</code> for the available rounding modes.
# Category 
Number.Conversion and formatting
# Examples 
Get the 64-bit integer <code>number</code> value of <code>"4"</code>.
```
Int64.From("4")
```
> 4

***
Get the 64-bit integer <code>number</code> value of <code>"4.5"</code> using <code>RoundingMode.AwayFromZero</code>.
```
Int64.From("4.5", null, RoundingMode.AwayFromZero)
```
> 5

***
