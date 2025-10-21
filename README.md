# RecipeExplorer 🍳

A modern, responsive recipe finder web app built with Next.js and TailwindCSS. Discover delicious recipes based on ingredients you have at home with a beautiful, app-like interface.

## ✨ Features

- **Ingredient-based Search**: Find recipes using ingredients you have
- **Real-time Auto-complete**: Smart ingredient suggestions as you type
- **Modern Recipe Cards**: Beautiful cards with images, prep time, and category tags
- **Expandable Recipe View**: Detailed view with ingredients and step-by-step instructions
- **Dark/Light Mode**: Toggle between themes for comfortable viewing
- **Save Recipes**: Bookmark your favorite recipes using localStorage
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Fast & Modern**: Built with Next.js 15 and TailwindCSS 4

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- npm, yarn, pnpm, or bun

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd recepi-finder
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

3. Get a Spoonacular API key:
   - Visit [Spoonacular API](https://spoonacular.com/food-api)
   - Sign up for a free account
   - Get your API key from the dashboard

4. Configure the API key:
   - Open `.env.local` file in the root directory
   - Replace `your-spoonacular-api-key-here` with your actual API key

5. Run the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

6. Open [http://localhost:3000](http://localhost:3000) in your browser

## 🎨 Customization

### Theme Colors
The app uses CSS custom properties for theming. You can customize colors in `src/app/globals.css`:

```css
:root {
  --primary: #f59e0b;        /* Main accent color */
  --background: #ffffff;      /* Light mode background */
  --foreground: #171717;      /* Light mode text */
  /* ... other color variables */
}

.dark {
  --background: #0a0a0a;      /* Dark mode background */
  --foreground: #ededed;      /* Dark mode text */
  /* ... other dark mode colors */
}
```

### API Configuration
The app uses the Spoonacular API. Configure your API key in the `.env.local` file:

```env
# .env.local
NEXT_PUBLIC_SPOONACULAR_API_KEY=your-actual-api-key-here
```

**Important:** 
- The `.env.local` file is already created with a placeholder
- Replace `your-spoonacular-api-key-here` with your actual API key
- Never commit your `.env.local` file to version control
- The `NEXT_PUBLIC_` prefix makes the variable available in the browser

## 🛠️ Built With

- **Next.js 15** - React framework with App Router
- **TypeScript** - Type safety and better development experience
- **TailwindCSS 4** - Utility-first CSS framework
- **Spoonacular API** - Recipe and ingredient data
- **React Hooks** - State management and side effects
- **localStorage** - Client-side data persistence

## 📱 Features in Detail

### Search & Discovery
- Type ingredients to get real-time suggestions
- Add multiple ingredients to refine your search
- Remove ingredients easily with one click
- Search for recipes based on available ingredients

### Recipe Display
- Grid layout with responsive design
- High-quality recipe images
- Prep time and serving information
- Category tags for easy identification
- Hover effects and smooth transitions

### Recipe Details
- Full-screen modal with detailed recipe information
- Complete ingredient list with measurements
- Step-by-step cooking instructions
- Save/unsave functionality
- Responsive layout for all screen sizes

### User Experience
- Dark/light mode toggle with system preference detection
- Smooth animations and transitions
- Keyboard navigation support
- Mobile-optimized interface
- Persistent theme and saved recipes

## 🔧 Development

### Project Structure
```
src/
├── app/
│   ├── globals.css      # Global styles and theme variables
│   ├── layout.tsx       # Root layout with metadata
│   └── page.tsx         # Main RecipeExplorer component
├── components/          # Reusable components (future)
└── types/              # TypeScript type definitions (future)
```

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server

## 🌐 Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add your Spoonacular API key as an environment variable:
   - Go to your Vercel project settings
   - Add environment variable: `NEXT_PUBLIC_SPOONACULAR_API_KEY`
   - Set the value to your actual API key
4. Deploy!

### Other Platforms
The app can be deployed to any platform that supports Next.js:
- Netlify
- Railway
- AWS Amplify
- DigitalOcean App Platform

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 📞 Support

If you have any questions or need help, please open an issue or contact the maintainers.

---

Made with ❤️ using Next.js and TailwindCSS
