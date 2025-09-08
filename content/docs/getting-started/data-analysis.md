---
title: "Data Analysis"
description: "Processing measurement data and calculating properties"
weight: 13
---

# Data Analysis

## Signal Processing

### FFT Analysis
- **Window function**: Hanning (recommended)
- **FFT size**: 4096-16384 points
- **Frequency resolution**: 0.1-1 Hz typical
- **Overlap**: 50% for averaging

### Peak Identification
- **Flexural mode**: First peak in spectrum
- **Torsional mode**: Second peak (if present)
- **Peak sharpness**: Indicates damping
- **Signal-to-noise**: Should be >10:1

## Property Calculations

### Young's Modulus (E)
```
E = (4π² × ρ × L⁴ × f_f²) / (k_f × t²)
```

Where:
- ρ = density (kg/m³)
- L = length (m)
- f_f = flexural frequency (Hz)
- t = thickness (m)
- k_f = 1.506 (first flexural mode)

### Shear Modulus (G)
```
G = (4π² × ρ × L² × f_t²) / k_t
```

Where:
- f_t = torsional frequency (Hz)
- k_t = 1.0 (first torsional mode)

### Poisson's Ratio (ν)
```
ν = (E / 2G) - 1
```

## Frequency Factors

### Rectangular Bars
- **First flexural**: k_f = 1.506
- **First torsional**: k_t = 1.0
- **Second flexural**: k_f = 2.500

### Cylindrical Bars
- **First flexural**: k_f = 1.571
- **First torsional**: k_t = 1.0

## Uncertainty Analysis

### Sources of Uncertainty
- **Dimensional measurements**: ±0.01mm
- **Mass determination**: ±0.1mg
- **Frequency measurement**: ±0.1Hz
- **Environmental effects**: ±1°C

### Combined Uncertainty
- **Young's modulus**: ±1-2% typical
- **Shear modulus**: ±1-2% typical
- **Poisson's ratio**: ±2-5% typical

## Quality Assessment

### Acceptable Results
- **Property values**: Within expected range
- **Poisson's ratio**: 0.0 to 0.5
- **Consistency**: <1% variation between measurements
- **Peak quality**: Sharp, well-defined peaks

### Validation Methods
- **Reference materials**: Compare with certified values
- **Literature comparison**: Check against published data
- **Cross-validation**: Compare with other methods
- **Statistical analysis**: Multiple measurements

## Common Issues

### Poor Signal Quality
- **Low amplitude**: Increase excitation force
- **Noisy signal**: Improve environmental conditions
- **Missing peaks**: Check excitation location
- **Broad peaks**: High damping material

### Calculation Errors
- **Unrealistic values**: Check formulas and units
- **Negative Poisson's ratio**: Verify mode identification
- **Inconsistent results**: Check measurement procedure
- **Outliers**: Investigate sample condition

## Software Tools

### Commercial Software
- GrindoSonic systems
- IMCE systems
- Custom analysis software
- MATLAB/Python scripts

### Open Source
- Python with SciPy
- MATLAB toolboxes
- R packages
- Custom implementations
