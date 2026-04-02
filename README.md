# CourierShipmentTrackingApp
<img width="752" height="492" alt="image" src="https://github.com/user-attachments/assets/5f2ab33c-d481-4a95-a1a2-77c57cbb412d" />

A Java-based logistics application demonstrating SOLID principles and Role-Based Access Control.

### Architecture
- **Models:** Courier, Shipment, User, Customer, Manager.
- **Logic:** Centralized tracking management with specialized permissions for staff.

### Key Highlights
- **Polymorphic Behavior:** Shared `viewTracking` logic across all users, with privileged `update` overrides for Managers with role based access that customer cannot update the shipping status and manager can pnly update the status.
- **Data Integrity:** Ensures that shipments are linked to specific couriers and customers via object composition.
- **Scalability:** Built with an abstract foundation to easily add new shipment types (e.g., Fragile, International) or new user roles.
