# SmartBike IoT Monitoring and Control System

The **SmartBike IoT Monitoring System** is a final-year project that transforms an electric motorcycle into a connected smart vehicle. The platform collects approved battery and vehicle telemetry, tracks the bike's location, sends data to cloud services, and presents useful information through a rider mobile application and fleet administration dashboard.

The project is being developed in collaboration with **Valiant Corporation**, with industry support for hardware, facilities, cloud resources, and technical guidance.

## Objectives

- Acquire and decode approved BMS and vehicle telemetry.
- Monitor battery state of charge, pack voltage/current, cell voltages, temperatures, and faults.
- Track the bike using GPS and cellular/telematics connectivity.
- Provide live status, location, alerts, diagnostics, service guidance, and savings information.
- Build cloud storage, REST/communication services, device management, and fleet monitoring.
- Add safe remote-control functions where technically and operationally permitted.
- Investigate AI/ML features for battery fault prediction, cell-voltage anomaly detection, and remaining-range estimation.
- Explain detected faults in clear English and Urdu.

## System Architecture

```text
Approved vehicle interfaces / sensors
                |
        ESP32 controller
                |
       GPS + cellular module
                |
       Cloud backend and APIs
          /                 \
 AI/ML diagnostics     Fleet dashboard
          |
     Rider mobile app
```

The system is organized into these layers:

1. **Embedded layer** - microcontroller firmware and approved vehicle interfaces.
2. **Connectivity layer** - GPS and cellular/telematics communication.
3. **Cloud layer** - telemetry ingestion, storage, APIs, authentication, and alerts.
4. **AI/ML layer** - predictive diagnostics and range estimation, subject to sufficient real-world data.
5. **Application layer** - rider mobile application and fleet/admin dashboard.

## Features

### Rider application

- Live bike and battery dashboard
- GPS location and location history
- Battery and vehicle diagnostics
- Fault and warning alerts
- Service guidance
- Energy/fuel savings information
- English/Urdu fault explanations
- Approved remote-control functions, when available and safe

### Fleet and administration dashboard

- Connected-bike monitoring
- Live locations
- Battery and vehicle health
- Telemetry trends and analytics
- Fault and service alerts
- Device and fleet records

### AI/ML capabilities

- Battery fault prediction
- Individual cell-voltage anomaly detection
- Remaining-range estimation
- Rider habit and ride-behavior analysis
- Natural-language explanations for technical faults

AI/ML functionality will be validated only where the quantity and quality of collected telemetry are sufficient.

## Current Progress

- Microcontroller-based SmartBike control and communication prototype developed.
- Available BMS/vehicle communication interface investigated and documented, including frame IDs, signal layouts, and fault information.
- Live battery telemetry verified during prototype testing.
- GPS coordinates acquired and verified using a GPS module.
- Initial mobile/web dashboard concept prepared.
- Initial system architecture, feature set, hardware plan, and AI/ML requirements defined.

## Planned Work

1. Integrate the industry-supported tracking/cellular telemetry module.
2. Establish reliable cloud communication and telemetry storage.
3. Complete the mobile application with dashboard, maps, alerts, diagnostics, and service features.
4. Integrate approved motor-controller telemetry and safe remote-control functions.
5. Build the cloud backend, database, APIs, and fleet dashboard.
6. Collect and prepare real ride and telemetry datasets.
7. Develop and validate AI/ML diagnostic and range-estimation models.
8. Complete end-to-end testing, safety validation, documentation, and demonstration.

## Hardware

| Component | Purpose |
| --- | --- |
| ESP32 development board | Main embedded controller |
| MCP2515 vehicle communication interface modules | BMS and motor-controller communication |
| Cellular/telematics module | Cloud connectivity and tracking |
| Neo-6M GPS module or equivalent | Location acquisition |
| Approved BMS and vehicle interfaces | Battery and vehicle telemetry |
| Approved sensors | Battery, temperature, and related measurements |
| Wires, connectors, breadboard, or prototype PCB | Hardware integration |

The estimated basic hardware cost is **Rs. 6,500**. Additional tracking modules, test benches, custom PCB fabrication, cloud hosting, and related resources are expected to be supported through the industry collaboration, subject to approval and availability.

## Software and Technologies

- Embedded firmware development environment
- Vehicle communication interface and telemetry protocols
- REST and communication services
- Cloud backend and database
- Mobile application framework
- Web dashboard technologies
- Python and machine-learning tools
- Mapping and notification services
- Git and GitHub

Specific technology choices may be adjusted during implementation based on hardware availability, integration requirements, and validation results.

## Project Timeline

| Phase | Deliverable | Status |
| --- | --- | --- |
| 1 | BMS/vehicle interface acquisition, verification, and documentation | Completed |
| 2 | Telematics, GPS, and cloud telemetry pipeline | In progress |
| 3 | Mobile application and rider dashboard | Planned |
| 4 | Full integration, motor diagnostics, remote-control prototype, and fleet dashboard | Planned |
| 5 | AI/ML diagnostics and fault-explanation layer | Planned |
| 6 | Testing, validation, documentation, and final demonstration | Planned |

The schedule follows the official SSUET FYP milestones and may change based on hardware availability, industry testing access, and telemetry-data availability.

## Scope and Safety

This project is an academic prototype for approved interfaces and supervised testing. Production deployment, large-scale fleet installation, formal safety certification, and modifications to safety-critical vehicle systems are outside the project scope unless separately approved.

Vehicle-level integration and remote control must remain subject to industry/supervisor guidance, approved interfaces, controlled testing, and applicable safety requirements.

## Team

| Member | Role |
| --- | --- |
| Zaid Ahmed Siddiqui | Team lead |
| Abdul Nasir | Team member |
| Kanzah Zeeshan | Team member |
| Sonia Salman | Team member |

**Supervisor:** Miss Dr. Najma Ismat  
**Industry advisor:** Syed Qamar Ali, CEO, Valiant Corporation

## Alignment

The project applies embedded systems, vehicle communications, IoT networking, cloud computing, databases, mobile development, software engineering, and artificial intelligence to electric mobility. It supports:

- **SDG 7:** Affordable and Clean Energy
- **SDG 9:** Industry, Innovation and Infrastructure
- **SDG 11:** Sustainable Cities and Communities
- **SDG 13:** Climate Action

## Expected Deliverables

- Working microcontroller-based SmartBike IoT prototype
- Rider mobile application prototype
- Cloud backend with telemetry storage and APIs
- Fleet/admin monitoring dashboard
- Validated AI/ML prototypes where data permits
- English/Urdu fault explanation module
- Technical architecture, testing, and project documentation
- Final demonstration for SSUET and the industry partner
