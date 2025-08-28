# Auto-Form - Password Protected Contact App

A simple React application featuring password-protected contact information display. Built with modern React hooks and deployed on Cloudflare Pages.

## 🚀 Live Demo

**Production**: [https://auto-form.pages.dev](https://auto-form.pages.dev)  
**Latest Deployment**: [https://05753c88.auto-form.pages.dev](https://05753c88.auto-form.pages.dev)

## 📋 Features

- **Password Protection**: Secure access to contact information
- **React Hooks**: Uses `useState` for state management
- **Responsive Design**: Clean, minimal interface
- **Form Validation**: Password verification with instant feedback
- **Modern Build**: Vite-powered development and production builds
- **Global Deployment**: Hosted on Cloudflare's global CDN

## 🛠️ Tech Stack

- **Frontend**: React 19.1.1
- **Build Tool**: Vite 7.1.2
- **Deployment**: Cloudflare Pages
- **Package Manager**: npm
- **Linting**: ESLint with React plugins

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn
- Wrangler CLI (for deployment)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/oskarcode/auto-form.git
   cd auto-form
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open browser**
   Navigate to `http://localhost:5173`

### Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build production bundle
- `npm run preview` - Preview production build locally
- `npm run lint` - Run ESLint code analysis

## 🔐 Usage

1. **Access the app** - Visit the live URL or run locally
2. **Enter password** - Use the password `swordfish` to unlock content
3. **View contacts** - Access protected contact information

### Password

The current password is: **`swordfish`**

> **Note**: In a real application, passwords should be hashed and stored securely, not hardcoded in the frontend.

## 📁 Project Structure

```
auto-form/
├── public/
│   └── vite.svg                # Vite logo
├── src/
│   ├── assets/
│   │   └── react.svg           # React logo
│   ├── App.css                 # Component styles
│   ├── App.jsx                 # Main Contact component
│   ├── index.css               # Global styles
│   └── main.jsx                # React app entry point
├── dist/                       # Production build output
├── eslint.config.js            # ESLint configuration
├── index.html                  # HTML template
├── package.json                # Dependencies and scripts
├── vite.config.js              # Vite configuration
├── wrangler.toml               # Cloudflare deployment config
└── README.md                   # This file
```

## 🚀 Deployment

### Cloudflare Pages

This project is configured for automatic deployment to Cloudflare Pages.

1. **Build the project**
   ```bash
   npm run build
   ```

2. **Deploy with Wrangler**
   ```bash
   # First time setup
   wrangler pages project create auto-form --production-branch main
   
   # Deploy
   wrangler pages deploy dist --project-name auto-form
   ```

3. **Access your site**
   Your app will be available at `https://auto-form.pages.dev`

### Alternative Deployment Options

- **Netlify**: Connect your GitHub repo for automatic deployments
- **Vercel**: Import project from GitHub with zero configuration
- **GitHub Pages**: Use GitHub Actions to build and deploy

## 🔧 Development

### Component Architecture

The app uses a single `Contact` component that manages:
- Authentication state with `useState` hook
- Form submission handling
- Conditional rendering based on auth status

### Key Files

- **`src/App.jsx`**: Main component with password logic
- **`src/main.jsx`**: React DOM rendering setup
- **`index.html`**: Entry HTML with Vite integration
- **`vite.config.js`**: Build tool configuration

### Code Style

- **ESLint**: Configured with React-specific rules
- **Modern React**: Uses hooks instead of class components
- **ES6+**: Arrow functions, destructuring, template literals

## 🛡️ Security Considerations

> **Important**: This is a demo application with simplified security.

**Current limitations**:
- Password is stored in plain text in the frontend code
- No server-side validation
- Client-side only authentication

**For production use**:
- Implement proper authentication (JWT, OAuth, etc.)
- Use environment variables for sensitive data
- Add server-side password validation
- Implement rate limiting for login attempts

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Run linting (`npm run lint`)
5. Commit changes (`git commit -m 'Add amazing feature'`)
6. Push to branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Links

- **Live App**: [https://auto-form.pages.dev](https://auto-form.pages.dev)
- **GitHub Repo**: [https://github.com/oskarcode/auto-form](https://github.com/oskarcode/auto-form)
- **Cloudflare Pages**: [https://pages.cloudflare.com](https://pages.cloudflare.com)
- **React Documentation**: [https://react.dev](https://react.dev)
- **Vite Documentation**: [https://vitejs.dev](https://vitejs.dev)

## 📊 Performance

- **Bundle Size**: ~188KB (59KB gzipped)
- **Build Time**: <1 second
- **Global CDN**: Sub-100ms response times worldwide
- **Core Web Vitals**: Optimized for performance

---

**Built with ❤️ using React and deployed on Cloudflare Pages**