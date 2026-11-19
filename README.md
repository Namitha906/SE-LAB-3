# Lab 3: Component Modelling & Architectural Pattern Selection

## Scenario
This lab focuses on designing the software architecture of a Self-Service Coffee Kiosk System for a busy café.

The kiosk allows customers to:
- Select from three coffee types: Espresso, Americano, and Latte.
- Choose between Small and Large sizes.
- Pay using a credit card.
- Receive a printed receipt containing order details.

## Architecture Selected
**Layered Architecture**

The system is organized into three layers:

1. **Presentation Layer** – Handles touchscreen interactions and displays the menu and order information.
2. **Business Layer** – Manages order processing and payment operations.
3. **Data/Hardware Layer** – Stores menu and pricing information and communicates with the receipt printer.

## Components
The system consists of the following components:

- User Interface Component
- Order Manager Component
- Payment Service Component
- Receipt Printer Component
- Database Component

## Component Interactions
- The User Interface sends customer selections to the Order Manager.
- The Order Manager manages the order and requests payment processing from the Payment Service.
- The Order Manager accesses the Database to retrieve menu and pricing information.
- After successful payment, the Order Manager sends receipt details to the Receipt Printer.
- Components interact through interfaces and dependencies represented in the UML Component Diagram.

## Architectural Justification
Layered Architecture was selected because it provides separation of concerns and is suitable for a small, focused kiosk application. It keeps the interface, business logic, and data/hardware interactions organized, making the system easier to maintain and modify.

## Deliverables
- **Component Diagram:** UML component diagram showing components, interfaces, dependencies, and interactions.
- **Written Justification:** A document explaining the architectural choice, two reasons for selecting it, a security advantage, and a performance benefit.

## Tools Used
- draw.io for creating the UML Component Diagram.
- Microsoft Word for the written justification.

## Submission
The component diagram is exported as PNG/PDF, and the written justification is saved as PDF for submission through the designated GitHub repository.
