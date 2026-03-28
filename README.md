# CINEMA BOOKING WEB APPLICATION 🎬

A personal project built with ASP.NET Core and SQL Server that allows users to search for movies, select showtimes, and complete secure online bookings. The application includes a Stripe payment integration and an admin panel for managing the movie catalog.

## FEATURES ✨

- **Movie Search** — Browse and search the movie catalog by title and genre.
- **Showtime Selection** — Choose from available showtimes and screening dates.
- **Secure Payment** — Complete bookings with integrated Stripe payment processing.
- **Booking Management** — View and manage reservations from a dedicated user interface.
- **Admin Panel** — Add, edit, and delete movies, showtimes, and screening dates.

## TECHNOLOGIES 🚀

- **ASP.NET Core** — Framework for building the web application backend.
- **SQL Server** — Relational database for storing movies, showtimes, and bookings.
- **Stripe** — Payment processing integration for secure online transactions.
- **HTML/CSS/JavaScript** — Frontend markup, styling, and interactivity.
- **Bootstrap** — Responsive UI component library.

## DEMO 🎬

Watch the demo on [YouTube](https://youtu.be/md3oHAhkOto).

## INSTALLATION ⚙️

> This guide assumes you have Visual Studio, the .NET SDK, and SQL Server installed.

1. Clone the repository and open `CineAimane.sln` in Visual Studio.
2. Open `appsettings.json` and update the following values:
   - Connection string pointing to your SQL Server instance.
   - `PublishableKey` and `SecretKey` with your Stripe API keys from the [Stripe Dashboard](https://dashboard.stripe.com/).
3. Import `CineAimane.sql` into SQL Server to create the schema and load the sample movie data.
4. Build and run the project from Visual Studio.

## CONTRIBUTING 🤝

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/my-new-feature`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add feature description'`).
5. Push to the branch (`git push origin feature/my-new-feature`).
6. Open a Pull Request.

## LICENSE 📄

This project is licensed under the [MIT License](LICENSE).

## CONTACT 📧

For any questions or feedback, reach out at [contact@aimanecouissi.com](mailto:contact@aimanecouissi.com).
