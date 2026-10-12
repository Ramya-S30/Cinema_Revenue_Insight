CH29 - CINEMA REVENUE INSIGHT DATASET
========================================
This is a SYNTHETIC practice dataset created to match the CH29 challenge schema.
It is not real SilverScreen Cinemas data. Do not report illustrative findings as real-world facts.

Files:
- bookings.csv: 1,200 booking/show records; booking_id, date, cinema, screen, movie, show_time, seat_class, tickets, revenue
- movies.csv: 20 movies; movie, movie_title, genre, language, runtime, certification
- cinemas.csv: 8 cinemas; cinema, city, screen_capacity, screen
- pricing.csv: seat_class, ticket_price, offer, discount_rate
- calendar.csv: 70 daily calendar records; date, weekday, holiday, release_week

Join suggestions:
- bookings.movie = movies.movie
- bookings.cinema = cinemas.cinema
- bookings.seat_class = pricing.seat_class (pricing contains multiple offer rows; join on seat_class + offer after mapping)
- bookings.date = calendar.date

Notes:
- Revenue is generated from tickets and seat-class price, adjusted for the selected offer.
- This dataset is suitable for practicing preprocessing, EDA, feature engineering, regression and visualization.
- The generated values are synthetic and should be described as such in reports.
