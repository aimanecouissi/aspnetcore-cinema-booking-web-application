# CINEMA BOOKING WEB APPLICATION 🎬

A personal project built with ASP.NET Core and SQL Server that allows users to browse movies, select showtimes, and complete bookings through Stripe Checkout. The application also provides printable tickets and an administration interface for managing the movie catalog.

## FEATURES ✨

- **Movie Search** — Browse and search the movie catalog by title.
- **Showtime Selection** — Choose from available showtimes and screening dates.
- **Payment Integration** — Complete the checkout process through Stripe.
- **Booking Confirmation** — Generate booking confirmations with printable barcode tickets.
- **Admin Panel** — Add, edit, and delete movies, with showtimes generated from movie details.
- **Admin Authentication** — Manage administrator access and account information.

## TECHNOLOGIES 🚀

- **C#** — Programming language used for backend development.
- **ASP.NET Core MVC (.NET 6)** — Framework for building the web application.
- **Entity Framework Core** — Object-relational mapping framework for database access and migrations.
- **SQL Server** — Relational database for storing movies, showtimes, and bookings.
- **ASP.NET Core Identity** — Authentication and account management framework.
- **Stripe** — Payment processing integration through Stripe Checkout.
- **HTML/CSS/JavaScript** — Frontend markup, styling, and interactivity.
- **Bootstrap** — Responsive UI component library.

## DEMO 🎬

Watch the demo on [YouTube](https://youtu.be/md3oHAhkOto).

## PREREQUISITES 📋

Before getting started, ensure you have the following:

- **.NET 6 SDK and Runtime** — Required to build and run the application.
- **SQL Server** — A local or accessible database instance.
- **Entity Framework Core Tools** — A version compatible with Entity Framework Core 6 for applying database migrations.
- **Stripe Account** — Required for configuring Stripe Checkout with test API credentials.
- **Development Environment** — Visual Studio or another compatible .NET development tool.

Windows is the recommended development environment because barcode generation uses `System.Drawing`.

## INSTALLATION ⚙️

1. Clone the repository to your local machine.
2. Open `CineAimane.sln` in Visual Studio, or use the .NET CLI from the repository root.
3. Restore the project dependencies: `dotnet restore .\CineAimane\CineAimane.csproj`.
4. Open `CineAimane/appsettings.json` and configure:
   - `ConnectionStrings:DefaultConnection` with your SQL Server connection details.
   - `StripeSettings` with your Stripe test API credentials.
5. Apply the existing Entity Framework Core migrations: `dotnet ef database update --project .\CineAimane\CineAimane.csproj`.
6. Populate the movie catalog through the administration interface once an administrator account is available. Adding movies through the application also generates their showtimes.
7. If you want to use administrator password recovery, configure the SMTP settings expected by the `EmailConfiguration` class in `CineAimane/Helpers/EmailHelper/`.
8. Configure and trust a local HTTPS development certificate, then run the application: `dotnet run --project .\CineAimane\CineAimane.csproj --urls https://localhost:44315`.
9. Open `https://localhost:44315` in your browser.

The supplied `CineAimane.sql` file contains a partial movie schema and sample data, not the complete application database. Do not execute the entire SQL file after applying migrations because it attempts to create a table that already exists.

The application currently uses `https://localhost:44315` in its Stripe success and cancellation URLs, so the development address must match unless those URLs are changed in the source code.

The complete administrator provisioning and sample-data initialization workflow has not been verified on a fresh installation.

## CONTRIBUTING 🤝

Contributions are welcome! Please follow these guidelines:

1. Follow the existing project structure and coding conventions.
2. Use [Conventional Commits](https://www.conventionalcommits.org/) for commit messages.
3. Test your changes locally whenever possible.
4. Update the documentation when introducing new features or changing existing functionality.

## LICENSE 📄

This project is licensed under the [MIT License](LICENSE).

## CONTACT 📧

For any questions or feedback, reach out at [contact@aimanecouissi.com](mailto:contact@aimanecouissi.com).
