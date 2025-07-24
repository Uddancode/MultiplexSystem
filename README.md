# MultiplexSystem

A web-based multiplex movie booking system built with Node.js, Express, MongoDB, and EJS.

## Features
- User registration and login
- Browse movies by category (Action, Comedy, Thriller, Romantic, etc.)
- Theatre-wise movie availability
- Book movie tickets with seat selection (Platinum, Gold, Silver)
- Booking history page showing all bookings
- Responsive UI with Bootstrap and custom CSS

## Technologies Used
- Node.js
- Express.js
- MongoDB (Mongoose)
- EJS (Embedded JavaScript Templates)
- Bootstrap 5
- Vanilla JavaScript

## Project Structure
```
MultiplexSystem/
├── app.js                  # Main server file
├── package.json            # Project dependencies
├── public/                 # Static assets (CSS, JS, images, vendor libraries)
├── views/                  # EJS templates (pages, partials)
│   ├── partials/           # Header and footer
│   └── ...                 # All main pages (booking, reviews, etc.)
└── README.md               # Project documentation
```

## Setup Instructions

### Prerequisites
- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [MongoDB](https://www.mongodb.com/) (local or Atlas)

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Tusharinvincible/MultiplexSystem.git
   cd MultiplexSystem
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Start MongoDB:**
   - Make sure your MongoDB server is running locally on the default port (27017), or update the connection string in `app.js` if using a remote database.
4. **Run the application:**
   ```bash
   node app.js
   # or, for auto-reload during development
   npx nodemon app.js
   ```
5. **Open in your browser:**
   - Visit [http://localhost:3000](http://localhost:3000)

## Usage
- **Register** a new user or **sign in** with existing credentials.
- **Browse movies** by category or see theatre-wise availability.
- **Book tickets** by selecting a movie, date, time, and available seats.
- **View booking history** after booking, with all details shown in a table.
- **Log out** when finished.

## Booking Flow
1. Go to the **Booking** page.
2. Fill in your name, email, select a movie, date, and time.
3. Select available seats (Platinum, Gold, Silver).
4. Click **Book Your Seat**.
5. After booking, you will be redirected to the **Booking History** page.
6. All booking details are also printed in the server console.

## Customization
- **Add new movies:** Edit the EJS files in `views/` and update the booking form options.
- **Change seat layout:** Modify the seat checkboxes in `views/booking.ejs`.
- **Styling:** Update CSS in `public/css/style.css` or add new styles.

## Contribution Guidelines
1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a Pull Request

## License
This project is licensed under the MIT License.

## Contact
For questions or support, open an issue on GitHub or contact the maintainer.
