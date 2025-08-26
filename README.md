# Vector-CANoe-Project

The Vector-CANoe-Project is a hands-on automotive communication simulation and testing project developed using Vector CANoe and CAPL scripting. The main objective of this project is to design, simulate, and validate Controller Area Network (CAN) based communication between Electronic Control Units (ECUs) in a vehicle environment.

## Development Tools
- **Vector CANoe** - Comprehensive software for simulation, test, and analysis of ECU networks
  - [Official Vector CANoe Product Page](https://www.vector.com/int/en/products/products-a-z/software/canoe/)
  - [Vector CANoe Documentation](https://www.vector.com/int/en/products/products-a-z/software/canoe/#documents)
  - [Vector Download Center](https://www.vector.com/int/en/services/downloads/)

- **CAPL Programming** - C-like language for ECU simulation and testing
  - [CAPL Programming Guide](https://www.vector.com/int/en/know-how/technology/capl/)

- **CANdb++ Editor** - Database editing tool for CAN networks
  - [CANdb++ Documentation](https://www.vector.com/int/en/products/products-a-z/software/candb/)

## Related Vector Tools
- **CANalyzer** - Analysis tool for CAN networks
  - [CANalyzer Product Page](https://www.vector.com/int/en/products/products-a-z/software/canalyzer/)
  
- **vTESTstudio** - Test design and automation environment
  - [vTESTstudio Product Page](https://www.vector.com/int/en/products/products-a-z/software/vteststudio/)

## Project Structure
- **Tx.can** - CAPL transmitter node handling switch inputs
- **Rx.can** - CAPL receiver node processing CAN messages
- **LightingControl.dbc** - CAN database defining message structure
- **ControlPanel.xml** - User interface for system interaction

## Key Features
- Headlight, foglight, and indicator control simulation
- Blinking logic implementation for turn signals
- Comprehensive diagnostic messaging
- System variable integration for hardware interaction

## CAN Message Protocol
| Message ID | Function | Data Payload |
|------------|----------|-------------|
| 0x14D (333) | Headlight Control | 0xCC (ON), 0xDD (OFF) |
| 0x1BC (444) | Foglight Control | 0xEE (ON), 0xFF (OFF) |
| 0x22B (555) | Indicator Control | 0xAB/0xBA (Left), 0xCD/0xDC (Right) |
| 0x29A (666) | Parking Light | 0xAD (ON), 0xDA (OFF) |

## System Requirements
- Vector CANoe v11.0 or newer
- Windows 10/11 operating system
- Minimum 8GB RAM (16GB recommended)
- CAN interface hardware (virtual or physical)

## Usage
1. Install Vector CANoe from the [Vector Download Center](https://www.vector.com/int/en/services/downloads/)
2. Open project in Vector CANoe environment
3. Compile and load CAPL nodes
4. Start simulation
5. Use control panel to toggle switches
6. Monitor CAN traffic and system responses

## Learning Resources
- [Vector E-Learning Portal](https://www.vector.com/int/en/services/training/e-learning/)
- [Vector YouTube Channel](https://www.youtube.com/user/VectorIVX)
- [CAPL Programming Examples](https://www.vector.com/int/en/know-how/technology/capl/capl-code-examples/)

This project demonstrates practical implementation of automotive networking concepts suitable for ECU development and validation roles using industry-standard Vector tools.
