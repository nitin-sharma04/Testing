# Voice Command Shopping Assistant

A modern web application that allows users to manage their shopping lists using voice commands. Built with Next.js, React, and the Web Speech API.

## 🚀 Features

- **Voice Recognition**: Use natural language to add, remove, and update shopping list items
- **Smart Categorization**: Automatically categorizes items into Dairy, Fruits, Vegetables, etc.
- **Seasonal Suggestions**: Get recommendations based on current season
- **Real-time Feedback**: See your voice commands transcribed in real-time
- **Responsive Design**: Mobile-first design that works on all devices
- **Offline Support**: Works with localStorage when offline

## 🛠️ Tech Stack

- **Frontend**: Next.js 14, React, TypeScript
- **Styling**: Tailwind CSS, shadcn/ui components
- **Voice**: Web Speech API
- **Storage**: localStorage (Firebase ready)
- **Deployment**: Vercel/Firebase Hosting ready

## 📱 Voice Commands

Try these natural language commands:

- `"Add 2 bottles of milk"`
- `"Remove bread from list"`
- `"Add 1 kg apples"`
- `"Update milk to 3 bottles"`
- `"Show me my shopping list"`
- `"Clear my shopping list"`

## 🏃‍♂️ Quick Start

1. **Clone and Install**
   \`\`\`bash
   git clone <repository-url>
   cd voice-shopping-assistant
   npm install
   \`\`\`

2. **Run Development Server**
   \`\`\`bash
   npm run dev
   \`\`\`

3. **Open in Browser**
   Navigate to `http://localhost:3000`

## 🔧 Configuration

### Firebase Setup (Optional)

1. Create a Firebase project at [Firebase Console](https://console.firebase.google.com)
2. Enable Firestore Database
3. Update `utils/firebase.ts` with your config:

\`\`\`javascript
export const firebaseConfig = {
  apiKey: "your-api-key",
  authDomain: "your-project.firebaseapp.com",
  projectId: "your-project-id",
  // ... other config
}
\`\`\`

### Browser Compatibility

- **Chrome**: Full support ✅
- **Edge**: Full support ✅
- **Firefox**: Limited support ⚠️
- **Safari**: Limited support ⚠️

## 📁 Project Structure

\`\`\`
src/
├── app/
│   ├── page.tsx              # Main application page
│   └── layout.tsx            # Root layout
├── components/
│   ├── VoiceInput.tsx        # Voice recognition component
│   ├── ShoppingList.tsx      # List display and management
│   └── SuggestionBox.tsx     # Smart recommendations
├── utils/
│   ├── nlpParser.ts          # Voice command parsing
│   ├── firebase.ts           # Database operations
│   └── suggestions.ts        # Recommendation logic
├── types/
│   └── index.ts              # TypeScript definitions
└── public/
    └── mock-data/            # Sample data files
\`\`\`

## 🎯 Key Features Explained

### Voice Recognition
- Uses Web Speech API for browser-native speech recognition
- Supports continuous and interim results
- Handles multiple languages (extensible)
- Graceful fallback for unsupported browsers

### NLP Parsing
- Regex-based command parsing
- Supports natural language variations
- Extracts quantities, units, and items
- Handles common shopping phrases

### Smart Suggestions
- Seasonal item recommendations
- Popular item suggestions
- Complementary item suggestions based on current list
- Customizable recommendation logic

### Data Management
- Real-time list updates
- Category-based organization
- Persistent storage (localStorage/Firebase)
- Offline-first approach

## 🚀 Deployment

### Vercel (Recommended)
\`\`\`bash
npm run build
vercel --prod
\`\`\`

### Firebase Hosting
\`\`\`bash
npm run build
npm run export
firebase deploy
\`\`\`

## 🔮 Future Enhancements

- [ ] Multi-language support (Hindi, Spanish, etc.)
- [ ] Price tracking and budget management
- [ ] Store location integration
- [ ] Barcode scanning
- [ ] Recipe-based shopping lists
- [ ] Family sharing features
- [ ] Push notifications for reminders

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

MIT License - see LICENSE file for details

## 🆘 Support

For issues and questions:
- Create an issue on GitHub
- Check browser compatibility
- Ensure microphone permissions are granted

---

**Built with ❤️ using Next.js and the Web Speech API**
