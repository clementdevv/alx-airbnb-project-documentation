# Airbnb Clone — Backend Features & Functionalities

This document provides a breakdown of all core features and functionalities expected from the backend system of the Airbnb Clone project. It is intended to accompany the visual diagram provided in `features-and-functionalities/features-map.png`.

---

## Feature Categories

### 1. User Authentication & Management
- **User Registration**: Create new user accounts (guests, hosts, admins)
- **Login/Logout**: Secure session/token-based authentication
- **Role-based Access**: Different permissions for guest, host, and admin roles
- **Profile Management**: Users can update personal information and settings
- **Password Security**: Hashed password storage, password reset flows

---

### 2. Property Management
- **List New Property**: Hosts can create property listings with details (name, location, description, price)
- **Update/Delete Property**: Hosts can manage their listings
- **View Properties**: Public and authenticated users can browse available properties
- **Image Uploads (optional)**: Support media storage for listings

---

### 3. Booking System
- **Make a Booking**: Guests can reserve properties by selecting dates
- **Manage Bookings**: Users can view, modify, or cancel their bookings
- **Check Availability**: System ensures no double bookings for same dates
- **Booking Status**: Track status — pending, confirmed, or canceled

---

### 4. Payment Processing
- **Initiate Payment**: Users pay for bookings using supported methods (e.g., credit card, PayPal)
- **Track Transactions**: Payment data is stored for verification and history
- **Payment Confirmation**: Only confirmed payments trigger booking finalization

---

### 5. Review & Rating System
- **Submit Review**: Guests can leave reviews and ratings for properties after stay
- **Read Reviews**: Users can browse reviews on listings
- **Edit/Delete Review**: Review owners can modify their feedback

---

### 6. Messaging System
- **Send Messages**: Guests and hosts can communicate before/after bookings
- **Inbox/Outbox Views**: View conversations with other users
- **Timestamped History**: Messages are stored with sent timestamps

---

### 7. Security & Roles
- **Authorization**: Enforce route-level access control (e.g., only host can update their property)
- **Validation**: Input checks to prevent malicious payloads
- **Rate Limiting**: Protect against brute force login attacks
- **Secure Storage**: Encrypt sensitive data (e.g., payment tokens, password hashes)

---

### 8. CI/CD & DevOps (Infrastructure Layer)
- **Dockerized Deployment**: Use Docker for containerization
- **CI/CD Pipeline**: GitHub Actions for testing and automated deployments
- **Environment Configs**: Store environment variables securely using `.env` files or secrets managers

---

## Visual Feature Map

The accompanying **PNG diagram** (`features-map.png`) visually represents:

- Each functional block (e.g., "Authentication", "Booking System")
- Arrows showing how components interact or flow into each other
- Groupings by user type (guest, host, admin) and module

You can find it in this directory:  
`features-and-functionalities/features-map.png`

---

## Tools Used

| Tool         | Purpose                    |
|--------------|----------------------------|
| **Draw.io**  | To design the feature map diagram |
| **Markdown** | For structured documentation |
| **GitHub**   | For version control and hosting |

---

## Summary

This feature map serves as a high-level overview of the core functionality that the backend must implement. It supports system planning, team coordination, and scalable implementation by clearly outlining each required capability.

# Use-Case Diagram