# Power-Supply-Calibration-Automated-System.

## Problem Statement

VARIOSYSTEMS' calibration process uses a Windows application to control power supplies and compare their output with multimeter readings. However, operators must manually connect probes for voltage and current measurements, requiring constant presence and making the process time-consuming. 

<img width="484" alt="image" src="https://github.com/user-attachments/assets/2bc253aa-a0c2-4418-8ebb-a677279644d4" />

Automating or streamlining probe connections based on measurement needs would reduce manual intervention, improving efficiency and saving operator time. A system that automatically connects probes could enhance workflow, minimize human error, and free operators for other tasks. Implementing such automation would optimize calibration, making it more efficient, accurate, and less labor-intensive, ultimately improving productivity and overall process effectiveness.

## Objectives of the Project

This project aims to enhance the efficiency and intelligence of the power supply calibration process at Variosystems by automating manual tasks and minimizing operator involvement. A key focus is the implementation of an intermediate switching unit to manage probe connections automatically, reducing human intervention and improving workflow efficiency. By streamlining these processes, calibration time will be significantly reduced, allowing operators to focus on higher-value tasks and increasing overall throughput.

Automation will not only save time but also enhance accuracy by eliminating human errors in probe connections and measurements. A new Windows application will be developed to intelligently control calibration, integrating with the power supply, multimeter, and switching unit. This software will use smart algorithms to manage test sequences, adjust parameters dynamically, and analyze results in real time.

Comprehensive reporting will be a core feature, providing detailed calibration reports with pass/fail statuses based on predefined criteria. Additionally, RFID technology will be integrated to automate the autofill of operator details in final reports, ensuring traceability and accountability.

By implementing these improvements, the project will transform the calibration process into a highly efficient, automated, and intelligent system, enhancing product quality, reducing operational overhead, and optimizing resource utilization across the production line.

## Implementation of Project	

The solution introduces an innovative intermediate switching unit capable of connecting multimeter and power supply probes through a relay matrix, controlled by a Windows application. This application fully automates the power supply calibration process. Initially, the operator's RFID is scanned, allowing the application to recognize the user. The GUI then displays the probe connection configuration, instructing the user to connect the probes accordingly and press the start button. From this point, the process becomes fully automated, calibrating all channels' voltages and currents by switching the probes automatically. Upon completion, the system generates detailed reports in Excel and PDF formats, which include operator details and comprehensive calibration data. This streamlined approach not only ensures accuracy and efficiency but also significantly reduces manual intervention in the calibration process.

<img width="510" alt="image" src="https://github.com/user-attachments/assets/1369b986-61d8-483f-94ba-fdd220dda7b9" />

This has three main parts,
1)	Relay matrix & Controller Unit.
2)	Windows Application.
3)	Final Reports Generation.

### 1) Intermediate Switching Unit (Relay matrix & Controller Unit)

•	The intermediate switching unit acts as a mediator between the power supply, multimeter, and the computer running the calibration software.
•	It is equipped with automated switching capabilities, allowing it to connect the appropriate probes for voltage and current measurements based on the calibration requirements.
•	This part is also responsible for RFID reading, probe connection detection, and RGB indication functions.

### Prototype of Switching unit  

<img width="150" alt="image" src="https://github.com/user-attachments/assets/3bb744fe-0231-4b2b-973c-6fa604dfa1e1" />

<img width="143" alt="image" src="https://github.com/user-attachments/assets/8e5528a8-97c4-46d6-a8b9-75bfd52794e2" />

<img width="286" alt="image" src="https://github.com/user-attachments/assets/3a3cafa7-a35b-4bc0-b801-0bdd8e812dbf" />

<img width="279" alt="image" src="https://github.com/user-attachments/assets/ee93c230-f1dc-46d7-b0c9-a5dbe0b8fc4b" />


### Final PCBs of Switching unit & Controller

#### Controller

<img width="453" alt="image" src="https://github.com/user-attachments/assets/af15348c-4a89-4508-aafd-7c308b809c65" />
<img width="256" alt="image" src="https://github.com/user-attachments/assets/14ea51fc-f1b0-43ad-ad6b-8abee1bd126d" />

#### Relay Matrix

<img width="290" alt="image" src="https://github.com/user-attachments/assets/c38354a9-8f5d-4915-bc50-678017e73dff" />
<img width="409" alt="image" src="https://github.com/user-attachments/assets/aa82db56-af08-4636-91c2-4498246f95d3" />

#### PCB Stack

<img width="484" alt="image" src="https://github.com/user-attachments/assets/03133955-e8ba-4c33-8f0b-879ed48c11c5" />

### 2) Windows Application

•	A new Windows application is developed to control the entire calibration process.

•	The software interfaces with the power supply, multimeter, and the intermediate switching unit.

•	The operator initiates the calibration process by running the program and specifying calibration parameters.

•	The application communicates with the intermediate switching unit to automate the probe connections, eliminating the need for manual intervention.

•	It controls the power supply to output specific voltages and currents, while the multimeter measures these values.

•	The software compares the power supply output with the multimeter readings and applies tolerance criteria to determine pass or fail for each voltage and current level. After calibration, it automatically generates a PDF and Excel report.

<img width="503" alt="image" src="https://github.com/user-attachments/assets/43bb5fb8-f143-4716-8376-69885cef32aa" />
<img width="507" alt="image" src="https://github.com/user-attachments/assets/1fbb2031-008c-4ec3-9962-baf091363c29" />
<img width="507" alt="image" src="https://github.com/user-attachments/assets/752a561a-0721-4ec7-bb04-07891ae0359e" />

### 3) Report Generation

•	The Windows application generates a detailed calibration report after completing the calibration process. The report includes information on each tested voltage and current level, the actual measurements from the multimeter, the power supply outputs, and whether each test passed or failed based on tolerance criteria.

•	This report provides a clear overview of the calibration results and can be saved or printed for documentation purposes.

•	The operator's name and SAP number are automatically filled in.
These are the autogenerated documents.

[0421TEC4484_KEYSIGHT_E36311A__2024_5_17.xlsx](https://github.com/user-attachments/files/18825457/0421TEC4484_KEYSIGHT_E36311A__2024_5_17.xlsx)

[0421TEC4484_KEYSIGHT_E36311A__2024_5_17.pdf](https://github.com/user-attachments/files/18825460/0421TEC4484_KEYSIGHT_E36311A__2024_5_17.pdf)


### Conclusion of the Project

 By introducing an intermediate switching unit and a dedicated software application, this solution revolutionizes the calibration process, automating tasks that previously demanded significant time and manual effort from operators. This innovative approach not only streamlines operations but also enhances efficiency and accuracy. Operators now simply connect probes according to provided visuals, initiating the process that the software seamlessly executes. The system generates comprehensive reports with detailed graphs, including measurements and pass/fail statuses for each test point. Additionally, the software automatically fills in operator details, ensuring streamlined documentation. This integrated solution not only reduces human error but also optimizes the overall calibration workflow, ultimately elevating quality control standards.
