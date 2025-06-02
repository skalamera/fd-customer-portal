# FD Customer Portal

A comprehensive customer support portal for **Benchmark Education**'s "Benchmark Universe" educational platform. This portal provides technical support services, real-time status monitoring, and knowledge base access for educators and school administrators.

## 🌟 Features

### **Portal Dashboard**
- **Welcome Section**: Personalized greeting with integrated search functionality
- **Action Cards**: Quick access to submit tickets, manage tickets, and join office hours
- **Real-time Status Monitor**: Live system status with glowing indicators
- **Knowledge Base**: Role-based help articles for Educators and Rostering Contacts
- **Quick Links**: Video tutorials, help center, and meeting booking

### **Real-time Status Monitoring**
- **Live Status Updates**: Monitors Benchmark Universe services every 3 minutes
- **Visual Indicators**: Color-coded status circles with glowing effects
- **Status Types**: Operational, Degraded, Partial Outage, Major Outage
- **Manual Control**: Global functions for status updates
- **Comprehensive Logging**: For debugging and monitoring

### **User Experience**
- **Responsive Design**: Mobile-friendly layout with adaptive grid system
- **Interactive Features**: Dismissible notices, sidebar navigation
- **Accessibility**: Skip links, ARIA labels, proper heading structure
- **Modern UI**: Glass-morphism effects with backdrop blur

## 🚀 Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Styling**: Custom CSS with responsive design
- **Fonts**: Google Fonts (Roboto), Material Icons, Custom fonts
- **External Integrations**: 
  - Freshworks Widget (support tickets)
  - Freshstatus (system status)
  - Cloudinary (image hosting)
  - Office365 (meeting booking)
  - Zoom (webinars)

## 📁 Project Structure

```
FD Customer Portal/
├── layout/                    # Core layout components
│   ├── header.html           # Navigation and branding
│   ├── footer.html           # Contact info and social links
│   ├── head.html             # Meta tags and external resources
│   └── layout.html           # Main template structure
├── pages/                    # Application pages
│   └── general-pages/
│       ├── portal-home.html      # Main landing page
│       ├── login-page.html       # Authentication
│       ├── new-user-signup.html  # User registration
│       └── search-results.html   # Search functionality
├── solutions/                # Knowledge base section
│   ├── solutions-home.html   # KB main page
│   └── [other KB pages]
├── tickets/                  # Support ticket system
│   └── [ticket management pages]
├── stylesheet/
│   └── style.css            # Custom styling
└── README.md
```

## 🎨 Design System

### **Color Palette**
- **Primary**: `#12344D` (dark blue)
- **Success**: `#009348` (green)
- **Warning**: `#ffc107` (yellow)
- **Danger**: `#dc3545` (red)
- **Background**: Custom SVG with educational theme

### **Status Indicators**
- 🟢 **Operational**: Green with glowing pulse animation
- 🟡 **Degraded**: Yellow with glowing pulse animation
- 🟠 **Partial Outage**: Orange with glowing pulse animation
- 🔴 **Major Outage**: Red with glowing pulse animation

## 🔧 Status Monitor Integration

The portal includes a sophisticated status monitoring system that:

1. **Monitors Service Health**: Checks connectivity to `benchmarkeducation.freshstatus.io`
2. **Updates Automatically**: Refreshes status every 3 minutes
3. **Provides Visual Feedback**: Glowing status circles with animations
4. **Offers Manual Control**: Global functions for emergency updates
5. **Logs Comprehensively**: Detailed console logging for debugging

### **Manual Status Updates**
```javascript
// Set status manually (useful during incidents)
setBUStatus('major-outage', 'Database maintenance in progress');

// Check if monitor is ready
if (isBUStatusReady()) {
    // Monitor is ready for updates
}

// Wait for monitor to initialize
waitForBUStatus().then(monitor => {
    // Use monitor instance
});
```

## 📱 Responsive Design

- **Desktop**: Full 3-column layout with all features
- **Tablet** (991px and below): 2-column layout with adjusted spacing
- **Mobile** (767px and below): Single column with optimized touch targets
- **Small Mobile** (480px and below): Stacked layout with compressed status display

## 🎯 Key Components

### **Status Monitor Section**
- Single-line display below search bar
- Real-time connectivity testing
- Animated status indicators
- Automatic fallback handling

### **Action Cards**
- **Submit a Ticket**: Direct access to Freshworks widget
- **Manage My Tickets**: View and track existing tickets
- **Office Hours**: Join virtual support sessions

### **Knowledge Base**
- **Educators**: Resources for classroom management
- **Rostering Contacts**: Technical administration guides
- **General**: FAQ and best practices

## 🔗 External Integrations

- **Freshworks**: Support ticket management and live chat
- **Freshstatus**: Real-time system status monitoring
- **Cloudinary**: Optimized image hosting and delivery
- **Office365**: Meeting booking integration
- **Zoom**: Virtual office hours and webinars

## 🚀 Getting Started

1. Clone the repository
2. Open `pages/general-pages/portal-home.html` in a web browser
3. The status monitor will automatically initialize and begin monitoring

## 📄 License

© 2024 Benchmark Education Company, LLC. All rights reserved.

## 🤝 Contributing

This project is maintained for Benchmark Education's internal customer support portal.

---

**Built with ❤️ for Benchmark Education Community** 