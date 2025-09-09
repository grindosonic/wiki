---
title: "Getting Started"
description: "Quick setup guide for impulse excitation testing"
weight: 10
---

# Getting Started

Everything you need to start measuring material properties with impulse excitation.

## Understanding NDT

### [Non-Destructive Material Testing: An Overview](/docs/getting-started/non-destructive-testing/)
Learn about the broader field of non-destructive testing, including common techniques like ultrasonic, radiographic, and eddy current testing, and how they improve product reliability and quality control.

## Equipment Needed

- **Impulse excitation system** - Main measurement unit
- **Test specimens** - Rectangular bars (50-150mm length)
- **Support system** - Two supports positioned at 0.224L from ends
- **Excitation device** - Small hammer or striker
- **Data acquisition** - Accelerometer and analysis software

## Sample Preparation

### Geometry Requirements
- **Length**: 3-5 times the width
- **Width**: 2-4 times the thickness  
- **Thickness**: As thin as possible while maintaining rigidity
- **Surface finish**: Ra < 1.6 μm

### Typical Sizes
- Small: 50×10×3 mm
- Standard: 100×20×5 mm
- Large: 150×30×8 mm

## Basic Procedure

1. **Measure dimensions** - Length, width, thickness (to ±0.01mm)
2. **Weigh sample** - Determine mass (to ±0.1mg)
3. **Position supports** - Place at 0.224L from each end
4. **Apply impulse** - Strike near center with consistent force
5. **Record vibration** - Capture signal for 1-2 seconds
6. **Analyze frequency** - Identify first flexural and torsional modes
7. **Calculate properties** - Use standard formulas

## Quick Reference

### Key Formulas
- **Young's Modulus**: E = (4π² × ρ × L⁴ × f_f²) / (1.506 × t²)
- **Shear Modulus**: G = (4π² × ρ × L² × f_t²) / 1.0
- **Poisson's Ratio**: ν = (E / 2G) - 1

Where: ρ = density, L = length, t = thickness, f_f = flexural frequency, f_t = torsional frequency

### Support Positioning
- **Flexural mode**: Supports at 0.224L from each end
- **Torsional mode**: Supports at center (for separate measurement)

## Next Steps

- [Equipment Setup](/docs/getting-started/equipment-setup/) - Detailed setup instructions
- [Measurement Procedure](/docs/getting-started/measurement-procedure/) - Step-by-step process
- [Data Analysis](/docs/getting-started/data-analysis/) - Processing and calculations
