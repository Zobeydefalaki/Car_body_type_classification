# Car_body_type_classification
# Car Body Type Classification

This project is a real-world machine vision system deployed in an automotive manufacturing environment.  
It automatically classifies car body types before they are sent to sub-assembly lines, replacing manual operator input.

## Project Context

- **Location in production**: After the paint shop, before sub-assembly
- **Purpose**: Automatically determine car body type to route it to the correct sub-assembly line
- **Previous method**: Manual operator input via control panel
- **Improvement**: Reduced errors, increased speed and consistency

## Features

- Classification of **6 known car body types**
- Detection of **unknown types** (e.g., new models not yet trained)
- Real-time inference and decision-making
- Integration with Siemens PLCs for automatic line routing

## Technologies

- **Programming Language**: Python  
- **Libraries**: OpenCV, TensorFlow, Keras, snap7  
- **Model**: Custom CNN  
- **Automation**: Communication with Siemens PLC using snap7

## Workflow

1. Image captured from fixed industrial camera
2. Preprocessing (resize, ROI extraction, filtering)
3. Inference using trained CNN model
4. Output class sent to PLC via `snap7`
5. PLC decides which sub-assembly line to send the car to

## Classes

- 206 SD
- 207
- Runna
- Samand
- 206 
- test bodies
- Unknown (fallback for untrained/new models)

## Deployment

This system is currently live and operational at **Iran Khodro**, providing automated classification and routing on the production line.

## Author

Industrial Automation & Machine Vision Engineer  
[S Z Falaki] — 10+ years in automotive industry  
LinkedIn / Portfolio: [https://www.linkedin.com/in/zobeideh-falaki-a6b55785]
