---
title: Quick Start Guide
nav_order: 2
---

# Quick Start Guide

This guide will help you get started with implementing Aeromat's performance plastics in your manufacturing processes.

## Prerequisites

Before beginning your project:

- Review material safety data sheets (MSDS)
- Ensure proper tooling availability
- Verify environmental conditions
- Prepare quality control measures

{: .callout.info}
> Having the right tools and environment is crucial for successful implementation.

## Material Selection

Choose the appropriate material based on your application requirements:

1. **Operating Temperature**
   - Consider maximum service temperature
   - Account for thermal cycling
   - Evaluate heat dissipation needs

2. **Mechanical Properties**
   - Tensile strength requirements
   - Impact resistance needs
   - Wear resistance considerations

3. **Chemical Resistance**
   - Exposure to solvents
   - Contact with lubricants
   - Environmental factors

## Design Considerations

When designing parts for manufacturing:

```javascript
// Example of minimum wall thickness calculation
function calculateMinWallThickness(length, material) {
  const thicknessRatios = {
    'PEEK': 0.015,
    'PPS': 0.020,
    'PTFE': 0.025
  };
  
  return length * thicknessRatios[material];
}
```

### Design Guidelines Table

| Feature | Minimum | Maximum | Notes |
|---------|---------|---------|-------|
| Wall Thickness | 1.5mm | 25mm | Depends on material |
| Corner Radius | 0.5mm | - | Internal corners |
| Draft Angle | 0.5° | 3° | For molded parts |
| Hole Diameter | 2mm | - | Self-tapping |

{: .callout.warning}
> Always consider the manufacturing process when determining design features.

## Processing Parameters

### Temperature Control

Monitor and maintain appropriate temperatures:

1. Material Temperature
   - Pre-drying conditions
   - Processing temperature
   - Cooling requirements

2. Tool Temperature
   - Preheating requirements
   - Operating temperature
   - Cooling rate

{: .callout.error}
> Exceeding maximum temperature limits can cause material degradation.

### Machining Guidelines

Basic parameters for common operations:

```python
def calculate_cutting_speed(diameter, rpm):
    """
    Calculate cutting speed in meters per minute
    
    Args:
        diameter (float): Tool diameter in mm
        rpm (int): Spindle speed in RPM
        
    Returns:
        float: Cutting speed in m/min
    """
    return (diameter * math.pi * rpm) / 1000
```

## Quality Control

Implement these quality control measures:

1. **Dimensional Inspection**
   - Use calibrated measuring tools
   - Document critical dimensions
   - Maintain inspection records

2. **Visual Inspection**
   - Check for surface defects
   - Verify color consistency
   - Identify any contamination

3. **Performance Testing**
   - Conduct load tests
   - Verify thermal properties
   - Test chemical resistance

{: .callout.info}
> Regular quality control checks help maintain consistent product quality.

## Next Steps

After completing this quick start guide:

1. Review specific material guides
2. Explore detailed processing parameters
3. Implement quality control procedures
4. Document your process

{: .callout.warning}
> Keep detailed records of all processing parameters and quality control results. 