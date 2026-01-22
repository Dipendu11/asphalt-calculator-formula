# Asphalt Calculator Formula (JavaScript)

This repository contains the standard mathematical formula used to calculate hot mix asphalt (HMA) tonnage for driveways and construction projects.

## The Formula
The standard density for asphalt is typically **145 lbs/cu ft** (or 2322 kg/m³).

### JavaScript Code Snippet
You can use this function in your own projects:

```javascript
function calculateAsphalt(length, width, depth) {
  // Length and Width in feet, Depth in inches
  const cubicFeet = length * width * (depth / 12);
  const density = 145; // standard density
  const totalWeight = cubicFeet * density;
  const tons = totalWeight / 2000;

  return tons.toFixed(2);
}
