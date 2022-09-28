# Use case narrative

## Booking badminton court

### Use case name 
**Booking badminton court.**

### Goal in Context
**Reserving a badminton court at a specific available time.**

### Primary Actor
**Customer/User**

### Secondary Actor
**\-**

### Precondition
**The Badminton Court Booking System must be operating/online and user must have stable internet connection.**

### Trigger
**Customer opens the booking app and start looking for a court to reserve.**

### Scenario
1. **User log in to the system with username and password.**
2. **User searching for open badminton court near them or all available badminton court.**
3. **User choose a badminton court and browse through their available time-slots for booking.**
4. **If the court does not provide time-slots, the user will need to choose the start-time and end-time of their visit.**
5. **The user have an option to ask for renting the badminton court’s equipment in advance instead of renting it when they are there.**
6. **User pay the fees via provided payment methods by the badminton court and the application.**
7. **After the user paid, the system generate booking information and sent to the badminton court and give the booking number to both user and the court operator.**

### Exceptions 
- **If the user does not log in first, the user cannot use the function. So user must log in.**
- **If the user does not register an account yet, they must do so before to be able to access the application.**
- **If the user cancel the reservation and did not start playing yet, the application will return the money via the same purchasing method that the user chose.**
- **If the payment was decline, the user needed to change their payment method until successful or cancel the booking process.**
- **The user must have a stable internet connection.**

### Post-condition
**The booking information file is created by the application and sent to both user and court operator. After that, the badminton court operator is expecting the user to show up on time and there will be reserved court and equipment for them.**

---

## Update Badminton Court Status
### Use Case Name
**When the court is booked, canceled, or closed.**

### Goal in Context
**Update the court status in the application for user acknowledgement**

### Primary Actor
**Application system, Customer/User, Badminton court operator**

### Secondary Actor
**-**

### Precondition
**The Badminton Court Booking System must be operating/online and user must have stable internet connection.**

### Trigger
**The customer have generated a booking or cancel in the application.**  
**The Badminton court operator wanted to update the available time or close the court reserve ability.**

### Scenario
#### Booking Successfully
1. **When the court is successfully booked, the application system then generate a booking information which include date, time, equipment required, and booking number for verification.**
2. **The generated booking information then will be sent to both court operator and the user.**
3. **The system will update the court information in the application that the time-slot of the court have been reserved for other user to see.**
4. **If the court booking is full, then the application update the court information that it is currently full until what time or day and will not appear as a search result until there is an available time-slots for other user to book.**

#### Badminton court close unexpectedly
1. **The badminton court operator updated the court status to be closed unexpectedly in the application.**
2. **The application then cancel all reservation made with the court and return them the booking fees.**
3. **The application then remove the court from search result and will appear as closed in the application.**

### Exceptions 
**If the user does not log in first, the user cannot use the function. So user must log in.**

### Post-condition
**System update status of the badminton court to the application at the real-time.**

---

## Leaving a review on the Badminton Court
### Use Case Name
**Leaving a review on the Badminton Court**

### Goal in Context
**Creating a review in application on a specific badminton court**

### Primary Actor
**Customer/User**

### Secondary Actor
**Badminton court operator**

### Precondition
**The Badminton Court Booking System must be operating/online and user must have stable internet connection.**

### Trigger
**After the user finish playing badminton at the reserved court, they can leave a review on that specific court.**  

### Scenario
1. **After the user finished playing, the badminton court with reserved allotted time, they can choose to leave a review about the badminton court.**
2. **The user then open the booking application and choose the current booking information.**
3. **The user can choose to write a comment or give the court a star rating.**
4. **Post the review for other users and court operator to read and view the review.** 

### Exceptions 
- **If the user does not log in first, the user cannot use the function. So user must log in.**
- **If the user does not register an account yet, they must do so before to be able to access the application.**
- **If the user cancel the reservation and did not start playing yet, the user cannot leave a review on that court.**
- **The user must have a stable internet connection.**

### Post-condition
**The review is posted in the application on the specific court for other users and the court operators to view the review.**
