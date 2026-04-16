# DidacMaymoThesis

Bachelor thesis of Didac Maymo, supervised by MFZBCN at Tecnocampus in 2022.  
This repository is a copy of the original GitHub repository:  
https://github.com/DidacMaymo/MaymoDidacTesis/tree/main

## Overview

The purpose of this project is to develop a sequence of applications that acquire data from a person’s eye movements using a **Tobii Pro Glasses 3** device while the person performs a writing test with a **Wacom Cintiq** graphic tablet.

There are two main applications in this project:

- **HandAQUS**: records data from both devices during the acquisition session.
- **AlignData**: aligns, synchronizes, and visualizes the acquired data.

The overall goal is to determine where a person is looking at any given moment while writing. This supports the study of neurological disorders such as **Parkinson’s disease** and other conditions involving visuomotor and handwriting alterations.

## Research context

These applications have been used by students and professors from the same university within the framework of a **PECT project**, obtaining samples from approximately **150 real users** in different civic centers.

A full technical description of the framework, acquisition workflow, synchronization logic, exported files, and validation is provided in the associated article:

**HandAQUS: A Multimodal Acquisition and Synchronization Framework for Handwriting and Gaze Signals**.  
The paper describes the contribution as a dual framework composed of **HandAQUS** for simultaneous acquisition and **AlignData** for synchronization and visualization, developed in **C# using the .NET Framework**, and validated in research and clinical-oriented settings. :contentReference[oaicite:0]{index=0}  
It also states that the applications are openly available in this repository. :contentReference[oaicite:1]{index=1}

## Main functionality

The framework supports multimodal acquisition and processing of:

- **Handwriting data** captured from the Wacom tablet
- **Gaze data** captured from Tobii Pro Glasses 3
- **IMU data**
- **Scene video**
- **Session metadata**
- **Synchronized per-task exports**

According to the paper, HandAQUS stores the acquisition session in a structured folder and AlignData then synchronizes both streams using millisecond-level timestamps and exports per-task CSV files for downstream analysis. :contentReference[oaicite:2]{index=2}

## Hardware requirements

- **Tobii Pro Glasses 3**
- **Tobii recording unit**
- **Wacom Cintiq 16** graphic tablet
- **Wacom digital pen**
- **Windows computer**

The paper specifies that the framework was designed as a Windows-based environment integrating Tobii Pro Glasses 3 and Wacom Cintiq 16 for synchronized handwriting and gaze acquisition. :contentReference[oaicite:3]{index=3}

## Software origin and acknowledgements

This project was developed from a previously existing application called **HandAQUS**, which originally permitted acquisition from a Wacom Cintiq graphic tablet. Starting from that point, numerous new requirements were added, especially support for eye-tracking acquisition, synchronization, metadata handling, and visualization.

The base application was originally developed by:

- **@DzanMucha**
- https://github.com/BDALab/HandAQUS_for_Cintiq

The associated paper also acknowledges the original HandAQUS codebase by Jan Mucha. :contentReference[oaicite:4]{index=4}

## Associated publication

If you use this repository, please also cite the associated paper:

**Maymó-Calatayud, D., Monaco, A., Lopez-Xarbau, J., Faundez-Zanuy, M.**  
*HandAQUS: A Multimodal Acquisition and Synchronization Framework for Handwriting and Gaze Signals.*
WIRN'2026 Vietri sul Mare (Salerno, Italy) 9th-13th June'2026

## Notes

This repository is intended to preserve and share the software developed in the context of the bachelor thesis and the subsequent research work associated with the HandAQUS multimodal framework.

## License

This project is distributed under the terms of the license included in the `LICENSE` file.
