# Introduction 

UNCITRAL OpenDigitalProcurement is an electronic procurement concept designed for end-to-end digital service supporting the entire public procurement process. It is a prototype developed by the EBRD UNCITRAL Initiative, a technical cooperation between the European Bank for Reconstruction and Development (EBRD) and the United Nations Commission for International Trade Law (UNCITRAL). This document contains the technical documentation that describes the implementation of architecture, data models, data standard and environment of the Architecture of the OCDS Open Source Central Unit of the electronic public procurement system.

| ![img](/src/assets/icons/introduction5.png) | ![img](/src/assets/icons/introduction4.png) | |

The document explains in detail:
- The design and development principles that guide the system implementation
- The system architecture, data standard, modules and components
- The business process engine that acts as logical layer for identifying an event, and then selecting and executing the appropriate reaction
- The system API and the processes to consume information from the system as well as description of system features to allow its use from endpoints (retrieving information, creating objects, updating information, etc.)

## General design

Generally electronic public procurement system consists of an open source central unit, a web-portal and several networking e-commerce platforms (NEPPs), and it uses an [Open Contracting Data Standard](https://standard.open-contracting.org) (OCDS) and based on a concept of open source distributed architecture in order to guarantee data standardisation and ensure user trust in data exchange accuracy.

Concept provides digital procurement services to end users – contracting authorities and economic operators through the NEPPs. The central unit serves as an interoperable online data exchange and a transaction repository for linked NEPPs. Data collected by the central unit is displayed in real time in the web-portal, which is accessible and searchable. This web-portal serves as a single point of access to all ‘collected at source’ procurement information, including electronic bidding. It is automatically synchronised in real time between all network members – the central unit, web portal, NEPPs, and e-government services and digital registers, when available.

MTender offers an end-to-end electronic procurement system with the three main characteristics of:
- modularity, which enables flexibility, self-executability and high levels of data resilience
- networked interoperability of the digital procurement solution, which allows for its open multi-platform implementation
- a transparent and comprehensive digital solution with structured transactional data, which allows for further public procurement process analyses

For additional information and the technical documentation of the UNCITRAL OpenDigitalProcurement see [documentation section] (#/content)
