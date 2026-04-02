# CourierShipmentTrackingApp
<img width="752" height="492" alt="image" src="https://github.com/user-attachments/assets/5f2ab33c-d481-4a95-a1a2-77c57cbb412d" />

A Java-based logistics application demonstrating SOLID principles and Role-Based Access Control.

### Architecture
- **Models:** Courier, Shipment, User, Customer, Manager.
- **Logic:** Centralized tracking management with specialized permissions for staff.
### OUTPUT
<img width="860" height="399" alt="Screenshot 2026-04-02 213438" src="https://github.com/user-attachments/assets/0ddea069-e2c4-44cf-a4a1-3c96b028d478" />
<img width="827" height="410" alt="Screenshot 2026-04-02 213517" src="https://github.com/user-attachments/assets/a9598fca-3b70-4ce7-b820-1816dd2b6d30" />
<img width="954" height="359" alt="Screenshot 2026-04-02 213609" src="https://github.com/user-attachments/assets/adef5262-a9f8-4469-b78c-6c84096d9b95" />
<img width="945" height="430" alt="Screenshot 2026-04-02 213914" src="https://github.com/user-attachments/assets/b4e4425f-1273-4519-a768-fe3ee709ec46" />


### Key Highlights
- **Polymorphic Behavior:** Shared `viewTracking` logic across all users, with privileged `update` overrides for Managers with role based access that customer cannot update the shipping status and manager can pnly update the status.
- **Data Integrity:** Ensures that shipments are linked to specific couriers and customers via object composition.
- **Scalability:** Built with an abstract foundation to easily add new shipment types (e.g., Fragile, International) or new user roles.
