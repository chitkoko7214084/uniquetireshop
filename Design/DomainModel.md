
# Domain Model

classDiagram
    direction RL

    class User {
        userID : int
        name: string
        phonenumber: int
        language: string (Burmese, Spanish, English)
    }

    class Customer {
        customerID: int
        + bookService()
        + chooseDateAndTime()
    }

    class ServiceProvider {
        login: string
        password: string
        + viewAppointments()
        + updateBooking()
        + deleteBooking()
        + makeCall()
    }

    class Appointment {
        appointmentID: string
        date: string
        serviceType: string
        customerName: string
    }




# Classes

- Users
    - The users are customers and service providers. This class have both user and service provider behaviors. 

- Customers
    - In sub class of customer offer book service and choose dates and time for their appointments.

- Service_provider
    - Service provider can view the customer data, they can update and delete the bookings. They can also make a calls.

- Appointment
    - This class will have a unique ID, also contain date and time, and service type. 