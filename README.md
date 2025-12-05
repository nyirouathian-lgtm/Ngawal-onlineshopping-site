# 🛍️ Ngawal - South Sudan Online Shopping Platform
<img width="1024" height="1024" alt="Image" src="https://github.com/user-attachments/assets/e19f5bdf-5e18-4044-9e0c-fffd20bddb68" />
## 📋 Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Pages Structure](#pages-structure)
- [Technology Stack](#technology-stack)
- [Setup & Installation](#setup--installation)
- [Usage Guide](#usage-guide)
- [Key Functionalities](#key-functionalities)
- [Development Notes](#development-notes)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🌟 Project Overview

**Ngawal** is a modern, responsive e-commerce platform specifically designed for the South Sudanese market. It connects local buyers and sellers through an intuitive online marketplace with features tailored to the region's needs, including M-Gurush mobile money payments and cash on delivery options.

### 🎯 Mission
To revolutionize online shopping in South Sudan by providing a secure, user-friendly platform that supports local businesses and makes e-commerce accessible to everyone.

SCREENSHOT DEMO
![Image](https://github.com/user-attachments/assets/4b6f8aea-9cec-4951-93fa-1ec382b46d5c)
![Image](https://github.com/user-attachments/assets/99911bd2-27cb-4d80-b43c-47027a73fc22)
![Image](https://github.com/user-attachments/assets/d529ba5c-e10c-4bdf-a28d-ff5e16073bc0)
![Image](https://github.com/user-attachments/assets/78e57d0e-26a6-4289-bc5e-ced968f68bbb)

### ✨ Key Highlights
- **Localized Solutions**: Built for South Sudanese market needs
- **Multiple Payment Options**: M-Gurush (MTN) and Cash on Delivery
- **AI-Powered Support**: Integrated chatbot for customer assistance
- **Mobile-First Design**: Fully responsive across all devices
- **Local Storage**: No backend required for demo functionality

## 🚀 Features

### 🛒 Core E-commerce Features
- **Product Catalog**: 24+ products across 6 categories
- **Shopping Cart**: Persistent cart with quantity management
- **Wishlist**: Save products for later
- **Product Ratings**: Rate products and services
- **Search & Filter**: By category, location, and price
- **Sorting Options**: Price, rating, and newest

### 💳 Payment System
- **M-Gurush Integration**: Simulated MTN mobile money payments
- **Cash on Delivery**: Traditional payment method
- **Secure Transactions**: Mock payment processing with success/failure states
- **Payment History**: Transaction IDs and confirmation

### 🤖 Advanced Features
- **AI Chatbot**: 24/7 customer support
- **Service Ratings**: Rate delivery, support, and product quality
- **Seller Registration**: Complete seller onboarding process
- **User Accounts**: Login/registration system
- **Notifications**: Toast notifications for user actions
- **Responsive Design**: Works on mobile, tablet, and desktop

### 📱 Responsive Design
- Mobile-first approach
- Touch-friendly interface
- Optimized for low-bandwidth connections
- Cross-browser compatibility

## 📄 Pages Structure

### 1. **Home Page** (`index.html`)
- **Purpose**: Main landing page with all features
- **Components**:
  - Hero section with call-to-action
  - Category navigation
  - Featured products (24 items)
  - Payment methods showcase
  - AI chatbot
  - Service rating system
  - Shopping cart sidebar

### 2. **Login Page** (`login.html`)
- **Purpose**: User authentication
- **Features**:
  - Email/password login
  - Social login options (Google, Facebook)
  - Remember me functionality
  - Forgot password link
  - Demo credentials pre-filled

### 3. **Wishlist Page** (`wishlist.html`)
- **Purpose**: Saved items management
- **Features**:
  - View saved products
  - Move items to cart
  - Remove from wishlist
  - Product recommendations
  - Clear all functionality

### 4. **Account Page** (`account.html`)
- **Purpose**: User profile management
- **Features**:
  - Dual mode (login/register)
  - Account statistics
  - Recent orders (simulated)
  - Account settings
  - Security options

### 5. **Become a Seller Page** (`become-seller.html`)
- **Purpose**: Seller registration and onboarding
- **Features**:
  - Complete registration form
  - Business information collection
  - Document upload
  - Terms and conditions
  - Next steps guide

## 🛠️ Technology Stack

### Frontend Technologies
- **HTML5**: Semantic markup structure
- **CSS3/Tailwind CSS**: Utility-first styling framework
- **JavaScript (ES6+)**: Dynamic functionality
- **Font Awesome 6.4.0**: Icon library
- **Google Fonts (Poppins)**: Typography

### CDN Libraries
- **Tailwind CSS**: `https://cdn.tailwindcss.com`
- **Font Awesome**: `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css`
- **Google Fonts**: `https://fonts.googleapis.com/css2?family=Poppins`

### Storage
- **LocalStorage API**: Client-side data persistence
- **Session Management**: User authentication state

## ⚙️ Setup & Installation

### Quick Start (No Installation Required)
Simply open `index.html` in any modern web browser. All features work offline using LocalStorage.

### For Development
1. Clone or download the project files
2. Ensure all HTML files are in the same directory
3. Open `index.html` in your browser
4. No server required - works on `file://` protocol

### File Structure
```
ngawal-ecommerce/
├── index.html              # Main homepage
├── login.html              # Login page
├── wishlist.html           # Wishlist page
├── account.html            # Account page
├── become-seller.html      # Seller registration
└── README.md              # This documentation
```

## 📖 Usage Guide

### For Buyers
1. **Browse Products**: Navigate categories or use search
2. **Add to Cart**: Click "Add to Cart" on any product
3. **View Cart**: Click cart icon in header
4. **Checkout**: Choose M-Gurush or Cash on Delivery
5. **Track Orders**: View in account section (simulated)

### For Sellers
1. **Register**: Visit "Become a Seller" page
2. **Fill Form**: Complete registration details
3. **Submit**: Application sent for review (simulated)
4. **Start Selling**: Once approved (in future versions)

### Payment Demo
1. **M-Gurush Payment**:
   - Click "Try M-Gurush Payment Demo"
   - Enter demo phone: `+211 912 345 678`
   - Enter demo PIN: `1234`
   - Simulated transaction processing

### AI Chatbot
- Click robot icon in bottom-right
- Ask about orders, payments, delivery
- Get instant responses
- Useful for customer support queries

## 🔑 Key Functionalities

### LocalStorage Management
```javascript
// Cart Management
localStorage.setItem('ngawal_cart', JSON.stringify(cart));
let cart = JSON.parse(localStorage.getItem('ngawal_cart')) || [];

// Wishlist Management
localStorage.setItem('ngawal_wishlist', JSON.stringify(wishlist));
let wishlist = JSON.parse(localStorage.getItem('ngawal_wishlist')) || [];

// User Session
localStorage.setItem('ngawal_user', email);
localStorage.getItem('ngawal_user');
```

### Product Database
- 24 pre-defined products
- 6 categories: Electronics, Fashion, Food, Home, Beauty, Sports
- Each product includes: name, price, category, location, rating, image
- Realistic South Sudanese pricing (SSP)

### Payment Simulation
- 80% success rate for M-Gurush payments
- Random transaction IDs
- Success/failure states with appropriate messaging
- Progress animation during processing

## 🎨 Design System

### Color Palette
| Color | Hex | Usage |
|-------|-----|-------|
| Primary | `#1a365d` | Headers, buttons, accents |
| Secondary | `#2c5282` | Hover states, secondary elements |
| Accent | `#ed8936` | CTAs, highlights, warnings |
| MTN Yellow | `#FFCC00` | M-Gurush payment elements |
| MTN Brown | `#993300` | M-Gurush secondary color |
| Success | `#10b981` | Positive indicators |
| Error | `#ef4444` | Error messages, warnings |

### Typography
- **Primary Font**: Poppins (300-700 weights)
- **Font Sizes**: Responsive scaling
- **Line Heights**: Optimized for readability

### Animations
- **Fade In/Out**: Smooth transitions
- **Slide In**: Cart and modal animations
- **Hover Effects**: Interactive elements
- **Loading States**: Payment processing

## 🔧 Development Notes

### State Management
The application uses a simple state management system with LocalStorage for:
- Shopping cart
- Wishlist
- User session
- Ratings (simulated)

### Performance Considerations
- Minimal external dependencies
- Optimized images (emoji placeholders)
- Lazy loading for product images
- Efficient DOM manipulation

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+
- Mobile browsers (iOS Safari, Chrome for Android)

## 🚀 Future Enhancements

### Planned Features
1. **Backend Integration**
   - Real user authentication
   - Database for products and orders
   - Payment gateway integration

2. **Advanced Features**
   - Product reviews and comments
   - Order tracking with real-time updates
   - Seller dashboard
   - Inventory management

3. **Mobile App**
   - Progressive Web App (PWA)
   - Native mobile applications
   - Push notifications

4. **Localization**
   - Multiple languages (Arabic, local dialects)
   - Currency conversion
   - Regional shipping options

5. **Admin Features**
   - Admin dashboard
   - User management
   - Order management
   - Analytics and reporting

### Technical Improvements
- Implement proper MVC architecture
- Add unit and integration tests
- Improve accessibility (ARIA labels)
- Optimize for slower connections
- Add service worker for offline capabilities

## 🤝 Contributing

We welcome contributions to improve Ngawal! Here's how you can help:

### Development
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Areas for Contribution
- **Bug Fixes**: Report or fix issues
- **New Features**: Suggest and implement new features
- **Documentation**: Improve documentation
- **Design**: Enhance UI/UX
- **Localization**: Add support for more languages

### Code Guidelines
- Follow existing code style
- Add comments for complex logic
- Test changes thoroughly
- Ensure mobile responsiveness

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Attribution
- Icons by Font Awesome
- Fonts by Google Fonts
- Design inspiration from modern e-commerce platforms
- Colors inspired by South Sudanese flag and MTN branding

## 📞 Contact & Support

### For Users
- **Email**: support@ngawal.com (demo)
- **Phone**: +211 123 456 789 (demo)
- **Live Chat**: AI chatbot on website

### For Developers
- **Issues**: Report bugs via GitHub issues
- **Suggestions**: Feature requests welcome
- **Questions**: Open a discussion

### Project Team
- **Frontend Development**: KATRINA ATHIAN
- **Design**: Custom design for South Sudan market
- **Concept**: Local e-commerce solution

## 🙏 Acknowledgments

- **MTN South Sudan**: For M-Gurush payment concept
- **Local Businesses**: For product inspiration
- **Open Source Community**: For amazing tools and libraries
- **ALU**: For learning resources and support

---

## ⚠️ Important Notes

### Demo Purpose
This is a **demonstration project** designed for portfolio and educational purposes. It simulates real e-commerce functionality but does not process real transactions.

### Data Persistence
All data is stored in browser's LocalStorage and will be cleared if:
- Browser cache is cleared
- Private/incognito mode is used
- Different browser is used

### Payment Simulation
The M-Gurush payment system is a **simulation**. No real money transactions occur. Use the demo credentials provided for testing.

### Deployment
For production deployment, you would need:
1. Backend server (Node.js, Python, PHP, etc.)
2. Database (MySQL, MongoDB, PostgreSQL)
3. Payment gateway integration
4. SSL certificate for security
5. Domain name and hosting

---

**Built with ❤️ for South Sudan's digital economy**

*Last Updated: December 2025*
