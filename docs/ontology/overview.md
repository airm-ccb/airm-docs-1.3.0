# AIRM Ontology


```mermaid
---
title: Strategic Concepts
---
flowchart LR    
  subgraph Traffic
    FLIGHT@{ shape: doc, label: "Flight"}
  end
  subgraph Operations
    ATO@{ shape: doc, label: "Air Traffic<br>Operations"}
  end
  subgraph Stakeholders
    STK@{ shape: doc, label: "Stakeholders"}
  end
  subgraph Infrastructure
    INFRA@{ shape: docs, label: "Aircraft<br>Base infrastructure<br>Airspace infrastructure"}
  end

Traffic -- is enabled by --> Operations
Traffic -- uses --> Infrastructure
Traffic -- is performed by --> Stakeholders
Stakeholders -- own --> Infrastructure
Operations -- are performed by --> Stakeholders
Operations -- are constrained by --> Infrastructure
```

## Traffic

| AIRM Subject | Ontology | Description |
| :- | :- | :-------------------------- |
| `Flight` | [Flight](ontology/flight.md) | Information about a specific flight. |
| `Flight` | [Flight Event](ontology/flightevent.md) | Information about actions, tasks or facts relevant to a specific flight which occur at an instant.|
| `Flight` | [Flight Identifier](ontology/flightidentifier.md) | Information about identifiers of a flight. |
| `Flight` | [Flight Phase](ontology/flightphase.md) | Information about period-in-time occurrences during a Flight. |
| `Flight` | [Movement](ontology/movement.md) | Information about movement of an aircraft both in the air and on the ground including position, time, and at least via calculation, speed and acceleration. |

## Operations

| AIRM Subject | Ontology | Description |
| :- | :- | :-------------------------- |
| `Air Traffic Operations` | [Aerodrome Operations](ontology/aerodromeoperations.md) | Information about planning, execution and analysis of airport airside activities, including, but not limited to, how the aerodrome operators provide the needed ground infrastructure and precise surface guidance to improve safety and maximize aerodrome capacity in all weather conditions. |
| `Air Traffic Operations` | [Airport Slot Management](ontology/airportslotmanagement.md) | Information on IATA managed airport slots as far as is required as baseline for network management processes. |
| `Air Traffic Operations` | [Deicing](ontology/deicing.md) | De-icing operation on an aircraft that may consist of removal of snow, ice or frost from the aircraft (de-icing), and/or also application of chemicals that remain on a surface and continue to delay the reformation of ice up (anti-icing). |
| `Air Traffic Operations` | [Turnaround](ontology/turnaround.md) | The arrival, unloading, and preparation for the return journey of an aircraft. |
| `Air Traffic Operations` | [Airspace User Operations](ontology/airspaceuseroperations.md) | Information about the ATM-related aspect of flight operations. |
| `Air Traffic Operations` | [ATM Phases](ontology/atmphases.md) | Information about groupings of related collaborative ATM activities relative to a flight or a group of flights. |
| `Air Traffic Operations` | [ATM Service Delivery Management](ontology/atmservicedeliverymanagement.md) | Information about the balance and consolidation of the decisions of the various other processes/services, as well as the time horizon at which, and the conditions under which, these decisions are made. |
| `Air Traffic Operations` | [Cargo Operations](ontology/cargooperations.md) | Information on all activities required to enable the safe transport of cargo by air. |
| `Air Traffic Operations` | [Conflict Management](ontology/conflictmanagement.md) | Information about a) the strategic conflict management through airspace organization and management, the demand and capacity balancing, and traffic synchronization; b) separation provision; c) and collision avoidance. |
| `Air Traffic Operations` | [Demand and Capacity Balancing](ontology/demandandcapacitybalancing.md) | Information about the strategic evaluation of the system-wide traffic flows and aerodrome capacities to allow airspace users to determine when, where and how they operate, while mitigating conflicting needs for airspace and aerodrome capacity. |
| `Air Traffic Operations` | [Emergency Operations](ontology/emergencyoperations.md) | Information about the activities carried out in case of an emergency. |
| `Air Traffic Operations` | [Information Services Products](ontology/informationservicesproducts.md) | Information about the products exchanged by information services. |
| `Air Traffic Operations` | [Aeronautical Information Product](ontology/aeronauticalinformationproduct.md) | Aeronautical data and aeronautical information provided either as digital data sets or as a standardized presentation in paper or electronic media. |
| `Air Traffic Operations` | [Flight Information Product](ontology/flightinformationproduct.md) | Messages concerning the intended or actual movement of aircraft based on the latest information furnished to ATS units by the pilot, the operator or its designated representative, or derived from ATS surveillance systems. |
| `Air Traffic Operations` | [Meteorological Information Product](ontology/meteorologicalinformationproduct.md) | Meteorological reports relating to existing or expected meteorological conditions. |
| `Air Traffic Operations` | [Military Operations](ontology/militaryoperations.md) | Information about ATM-related air traffic operations conducted by military stakeholders. |
| `Air Traffic Operations` | [Coordination](ontology/coordination.md) | Information about the coordination of flights between controllers. |

## Infrastructure

| AIRM Subject | Ontology | Description |
| :- | :- | :-------------------------- |
| `Aircraft` | [Aircraft](ontology/aircraft.md) | Information about the aircraft. |
| `Airspace Infrastructure` | [Airspace](ontology/airspace.md) | Information about the defined three-dimensional portions of the atmosphere relevant to ATS. |
| `Airspace Infrastructure` | [Infrastructure Point](ontology/infrastructurepoint.md) | Information about points in an airspace.  |
| `Airspace Infrastructure` | [Route and Procedure](ontology/routeandprocedure.md) | Information about the routes and procedures designed for channelling the flow of traffic en-route and while departing and landing. |
| `Base Infrastructure` | [Aerodrome Infrastructure](ontology/aerodromeinfrastructure.md) | Informaion about the  aerodrome including any installations and equipment. |
| `Base Infrastructure` | [Communication Infrastructure](ontology/communicationinfrastructure.md) | Information about the communication infrastructure. |
| `Base Infrastructure` | [Navigation Infrastructure](ontology/navigationinfrastructure.md) | Information about the navigation infrastructure.  |
| `Base Infrastructure` | [Surveillance Infrastructure](ontology/surveillanceinfrastructure.md) | Information about the surveillance infrastructure. |
| `Base Infrastructure` | [Obstacle](ontology/obstacle.md) | Information about ground based objects that are detrimental to the safe execution of flights. |
| `Base Infrastructure` | [Satellite System](ontology/satellitesystem.md) | Information about satellite systems. |

## Stakeholders

| AIRM Subject | Ontology | Description |
| :- | :- | :-------------------------- |
| `Stakeholders` | [Organisation, Role and Service](ontology/organisationroleandservice.md) | Generic framework for modeling organizations, roles and services. This is to be used for typing. Based on the W3C Organization proposal. |
| `Stakeholders` | [Agent](ontology/agent.md) | Specific common instances of "Agent" and their specialization relations. |
| `Stakeholders` | [Business Services](ontology/businessservices.md) | Specific common instances of "Service" and their specialization relations. |
| `Stakeholders` | [Document and Agreement](ontology/documentandagreement.md) | Description of cross-organizational agreements and documents. |
| `Stakeholders` | [Organisation](ontology/organisation.md) | Specific common instances of "Organisation" and their specialization relations. |
| `Stakeholders` | [Role](ontology/role.md) | Specific common instances of "Role" and their specialization relations |

## Other

| AIRM Subject | Ontology | Description |
| :- | :- | :-------------------------- |
| `Common` | [Geometry](ontology/geometry.md) | Information about ATM-related geometry concepts. |
| `Common` | [Geospatial](ontology/geospatial.md) | Information related to land, ice and ocean surfaces and any object with vertical extent above and/or under ground. |
| `Common` | [Temporal](ontology/temporal.md) | Information about ATM-related temporal concepts. |
| `Meteorology` | [Meteorology](ontology/meteorology.md) | Information about meteorological observation, forecast, phenomena and any other statement relating to existing or expected meteorological conditions. |

