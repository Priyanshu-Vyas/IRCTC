Wednesday, 25 December 2024

# IRCTC: JAVA Backend Project
## Ticket Booking System
### Project Setup
![image](https://github.com/user-attachments/assets/cc645062-0cca-4a70-a7fc-ccf09ff4d0f2)

### Writing Functional Requirements including Entities, Services, and utils. Also, Created localDb to store data as json.
Functional requirements
- able to login and signup
- fetch search trains
- show available seats
- book seat
- ticket fetch

1. Prepare LLD
    1. Entities
        1. User
            1. String Name
            2. String hashedPassword
            3. List<Ticket> ticketsBooked
            4. String userId
        2. Ticket
            1. String ticketId
            2. String userId
            3. String source
            4. String destination
            5. DateTime dateofTravel
            6. Train train
        3. Train
            1. String trainId
            2. String trainNo
            3. DateTime departTime
            4. DateTime arrivalTime
            5. List<List<Boolean>> seats
            6. Map<String, Time> stationTimes
            7. List<String> stations
    2. Service
        1. UserBookingService
            1. loginUser(User user)
            2. signUp(User user)
            3. fetchBookings(User user)
            4. cancel(User user)
            5. bookTicket(String a,String b)
        2. TrainService
            1. searchTrains(String a,String b)
            2. getSeatsAvailable(Train t1)

### Running Instances
<img width="1440" alt="image" src="https://github.com/user-attachments/assets/5bb820c7-b1b4-4105-96b5-57dd59bd7f44" />

 
