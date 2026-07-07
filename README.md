# Ambition Academy Website

## School Information
- **School Name:** Ambition Academy
- **Location:** Jhapa, Buddhasanti-2, Jayapur
- **Classes:** Nursery to 10
- **Tagline:** "You dream, We Create"
- **Contact:** +977 23416143
- **Facebook:** https://www.facebook.com/ambition.academy2016

## Features

### Frontend (Student/Parent/Public)
- ✅ Mobile-responsive design
- ✅ Photo & Video gallery
- ✅ Academic calendar, news, exam routines
- ✅ Real-time notifications for announcements
- ✅ Student/Parent feedback system (public advice board)
- ✅ Call now button with phone integration
- ✅ Dynamic wallpaper

### Admin Panel
- ✅ Manage announcements, posts, notifications
- ✅ Upload photos and videos
- ✅ Edit all website content (text, headlines, location, email)
- ✅ Change wallpapers/backgrounds
- ✅ Manage academic calendar
- ✅ Post news, exam routines, unit tests, monthly tests
- ✅ Class-specific content management
- ✅ Toggle announcement notifications

### Backend
- ✅ RESTful API
- ✅ Database for content management
- ✅ File upload handling (images/videos)
- ✅ Notification system
- ✅ Authentication & Authorization

## Tech Stack

### Frontend
- React 18+
- Tailwind CSS
- Axios
- React Router
- Firebase (for notifications)

### Backend
- Node.js
- Express.js
- MongoDB
- JWT Authentication
- Multer (file uploads)
- Nodemailer (notifications)

### Deployment
- Vercel (Frontend)
- Heroku/Railway (Backend)
- MongoDB Atlas (Database)

## Installation & Setup

### Prerequisites
- Node.js (v16+)
- npm or yarn
- MongoDB account

### Backend Setup
```bash
cd backend
npm install
cp .env.example .env
# Add your environment variables
npm start
```

### Frontend Setup
```bash
cd frontend
npm install
cp .env.example .env
# Add your API endpoint
npm start
```

## Project Structure
```
ambition-academy-website/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── package.json
│   ├── .env.example
│   └── server.js
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── admin/
│   │   ├── App.js
│   │   └── index.css
│   ├── package.json
│   ├── .env.example
│   └── public/
├── .gitignore
└── README.md
```

## API Endpoints

### Public Endpoints
- `GET /api/school/info` - Get school information
- `GET /api/announcements` - Get announcements
- `GET /api/gallery` - Get photos/videos
- `GET /api/academic` - Get academic calendar
- `POST /api/feedback` - Submit feedback
- `GET /api/feedback` - Get public feedback

### Admin Endpoints (Protected)
- `POST /api/auth/login` - Admin login
- `GET /api/auth/me` - Get current admin
- `POST /api/announcements` - Create announcement
- `PUT /api/announcements/:id` - Update announcement
- `DELETE /api/announcements/:id` - Delete announcement
- `POST /api/gallery` - Upload photos/videos
- `DELETE /api/gallery/:id` - Delete gallery item
- `PUT /api/school/info` - Update school info
- `POST /api/academic` - Create academic item
- `PUT /api/academic/:id` - Update academic item
- `DELETE /api/academic/:id` - Delete academic item
- `GET /api/feedback/admin/all` - Get all feedback
- `PUT /api/feedback/admin/:id/approve` - Approve feedback

## Demo Credentials
- **Email:** admin@ambitionacademy.com
- **Password:** (Set during first setup)

## Contributing
For contributions, please create a pull request.

## License
MIT
