# 🌍 Natours — Tour Booking API

A full-featured RESTful API for a tour booking platform, built with Node.js, Express, and MongoDB.

## 📖 About This Project

This project was built while following [Jonas Schmedtmann's Node.js course](https://www.udemy.com/course/nodejs-express-mongodb-bootcamp/) on Udemy. It served as my hands-on deep dive into backend development with the Node.js ecosystem.

**But this isn't where the story ends.** I'm actively extending this project with my own features and improvements beyond what the course covers — applying what I've learned to solve new problems and explore new ideas.

## ⚡ Features

- **Authentication & Authorization** — JWT-based auth with role-based access control (admin, guide, user)
- **Tour Management** — Full CRUD with advanced filtering, sorting, pagination, and field limiting
- **Geospatial Queries** — Find tours within a radius, get distances to tours from a point
- **Booking System** — Stripe checkout integration for tour payments
- **Reviews & Ratings** — Users can review tours with ratings that auto-calculate averages
- **Image Uploads** — Photo upload and processing with Sharp
- **Email Notifications** — Welcome emails, password reset, and booking confirmations
- **Security** — Rate limiting, data sanitization, HTTP headers hardening, and more

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Runtime | Node.js |
| Framework | Express.js |
| Database | MongoDB + Mongoose |
| Auth | JWT + bcrypt |
| Payments | Stripe |
| Email | Nodemailer |
| Image Processing | Sharp |
| Templating | Pug |

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/abbdelrhman/Tours-Natours.git

# Install dependencies
npm install

# Set up environment variables
# Create a config.env file with your own values (see config.env.example)

# Run in development
npm start
```

## 🔧 Environment Variables

Create a `config.env` file in the root directory with:

```
NODE_ENV=development
PORT=3000
DATABASE=your_mongodb_connection_string
DATABASE_PASSWORD=your_db_password
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=90d
JWT_COOKIE_EXPIRES_IN=90
EMAIL_USERNAME=your_email_username
EMAIL_PASSWORD=your_email_password
EMAIL_HOST=your_email_host
EMAIL_PORT=your_email_port
STRIPE_SECRET_KEY=your_stripe_key
```

## 🗺️ Roadmap — What I'm Adding Next

- [ ] Add a wishlist/favorites feature
- [ ] Implement tour search with autocomplete
- [ ] Add real-time notifications with WebSockets
- [ ] Build a full admin dashboard
- [ ] Add unit and integration tests
- [ ] Dockerize the application

## 📝 Lessons Learned

Building this project gave me solid experience with:
- Designing and consuming RESTful APIs
- MongoDB data modeling and Mongoose middleware
- Authentication patterns and security best practices
- Error handling in production vs development
- File uploads and image processing pipelines
- Payment integration with third-party services

## 🤝 Acknowledgments

Course by [Jonas Schmedtmann](https://github.com/jonasschmedtmann) — an excellent teacher who makes complex concepts click.

---

*Built with ☕ and curiosity.*
