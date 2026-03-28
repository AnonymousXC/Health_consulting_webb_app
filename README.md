# AI Health Consult

AI-powered health consultation app with 3D rotatable body diagram and pain intensity assessment.

## Features

- 🎨 Vibrant, responsive design with glass morphism effects
- 🔄 3D rotatable body diagram for precise body part selection
- 📊 Pain intensity slider (0-10 scale) with visual feedback
- 🤖 AI-powered health consultations via Groq API
- 📱 Fully responsive mobile-friendly interface
- 🌍 Multi-language support (auto-detects user language)

## Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Backend**: Node.js serverless functions
- **API**: Groq AI for health consultations
- **Deployment**: Vercel/Netlify ready

## Quick Setup

### 1. Environment Variables

Create a `.env` file or set up environment variables:

```bash
GROQ_API_KEY=your_groq_api_key_here
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run Locally

```bash
npm run dev
```

Open http://localhost:3000 in your browser.

## Deployment Options

### 🚀 Vercel (Recommended)

1. **Install Vercel CLI**:
   ```bash
   npm i -g vercel
   ```

2. **Deploy**:
   ```bash
   vercel --prod
   ```

3. **Set Environment Variable**:
   ```bash
   vercel env add GROQ_API_KEY
   ```

### 🌊 Netlify

1. **Install Netlify CLI**:
   ```bash
   npm i -g netlify-cli
   ```

2. **Deploy**:
   ```bash
   netlify deploy --prod
   ```

3. **Set Environment Variable** in Netlify dashboard:
   - Go to Site settings > Environment variables
   - Add `GROQ_API_KEY`

### 🔧 Traditional Hosting

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Start server**:
   ```bash
   npm start
   ```

3. **Configure reverse proxy** (Nginx/Apache) to route `/api/*` to Node.js server

## Configuration

### Groq API Setup

1. Sign up at [Groq Console](https://console.groq.com)
2. Create an API key
3. Add the key to your environment variables

### Customization

- Modify `api/chat.js` to change AI behavior
- Update `public/index.html` for UI changes
- Adjust colors and styling in the `<style>` section

## Project Structure

```
ai-health-consult/
├── public/
│   └── index.html          # Main frontend application
├── api/
│   └── chat.js             # Serverless function for AI chat
├── package.json            # Dependencies and scripts
├── vercel.json            # Vercel configuration
├── netlify.toml           # Netlify configuration
└── README.md              # This file
```

## Features Details

### 3D Body Diagram
- Interactive SVG body parts
- 360° rotation with mouse/touch
- Visual feedback on selection
- Responsive sizing

### Pain Intensity Slider
- 0-10 scale with color gradient
- Real-time intensity descriptions
- Smooth animations and transitions

### AI Consultation
- Context-aware responses
- Multi-language support
- Structured health advice format
- Privacy-focused (no data storage)

## License

MIT License - feel free to use for personal or commercial projects.

## Support

For issues or questions:
1. Check the [Issues](https://github.com/yourusername/ai-health-consult/issues) page
2. Create a new issue with detailed description
3. Include screenshots if applicable

---

**Disclaimer**: This app provides general health information and is not a substitute for professional medical advice. Always consult with qualified healthcare providers for medical concerns.