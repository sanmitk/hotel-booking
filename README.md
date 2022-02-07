# hotel-booking

The objective is for you to build an API to manage Booking.com Hotels, from dealing with inventory queries to searching for the best hotel for a customer.


You’re given a pre-configured Spring Boot project, with the following capabilities already implemented:

 

A /hotel GET endpoint, listing all the hotels in our system.

An H2 in-memory data source containing all our hotel inventory.

A basic service implementation layer to retrieve information from the hotel and city inventory.

Example implementations of functional tests (testing a bit of logic) and integration tests (testing an HTTP endpoint in your API).

 

If you like writing tests for your code and feel comfortable with it, we encourage you to do so, since it will contribute considerably towards improving your score.

 

But if you’re more of a problem solver, you can focus more on solving all the problems presented without writing tests for them and that's perfectly fine!

---------------------------------------------------------------------------------------------------------------------------------------------------------

Your tasks:

1. Create an API to retrieve a hotel. e.g. I want to retrieve a hotel using id

endpoint should look like - "hotel/{id}"

e.g. the endpoint - "/hotel/10" should give me the below response

    { hotel : 
       {
         id : "10",
         name : "xyz"
         .
         .
         . <all other hotel details>
        }
     }
     
 2. Create an API to Delete a hotel. I want to delete a particular hotel from the system, but it 
    should not do a permananet delete in the database. It should just be a logical delete.
    
    endpoint should look like ; "hotel/{id}"
    
 3. Get me hotels closest to the city center. I want 3 hotels closest from the city center,
    so that I can go to the nearest hotel.
    
    API endpoint should look like : "hotel/<name_of_ur_endpoint>?searchBy=distance"
    
    e.g. "hotel/closest-hotels?searchBy=distance"
    
    response - JSON - top 3 hotels matching the search
    
    TIP : distance between 2 geographic points can be calculated using 'Haversine Formula'. You
    can google that and feel free to use any 3rd party library.
     
     
