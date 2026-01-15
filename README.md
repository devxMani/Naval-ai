# Naval AI 🧘‍♂️

An AI-powered chatbot that embodies Naval Ravikant's thinking, philosophy, and wisdom. Built with Next.js 15, Vercel AI SDK, and powered by multiple state-of-the-art language models.

![Naval AI](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5.8-blue?style=flat-square&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-4.1-38B2AC?style=flat-square&logo=tailwind-css)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

## ✨ Features

- **Naval's Wisdom at Your Fingertips** - Access Naval Ravikant's tweets, essays, podcast transcripts, and interviews through semantic search
- **Multi-Model Support** - Choose from multiple AI models:
  - Claude Sonnet 4.5 (Anthropic)
  - Kimi K2 Thinking (Moonshot AI)
  - Grok 4 Fast Reasoning (xAI)
  - Qwen3 VL Thinking (Alibaba)
- **Intelligent Tool Use** - AI automatically searches, browses, and reads Naval's content to provide grounded responses
- **Dark/Light Mode** - Beautiful UI with theme toggle support
- **Real-time Streaming** - Smooth streaming responses with markdown rendering
- **Web Search** - Fallback to web search for recent information

## 🛠️ Tech Stack

- **Framework**: [Next.js 15](https://nextjs.org/) with App Router
- **AI SDK**: [Vercel AI SDK](https://sdk.vercel.ai/) with Gateway
- **UI Components**: [Radix UI](https://www.radix-ui.com/) primitives
- **Styling**: [Tailwind CSS 4](https://tailwindcss.com/)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Content API**: [NIA API](https://trynia.ai/) for Naval's content

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- pnpm (recommended) or npm/yarn
- NIA API Key (for Naval's content)
- AI Gateway API Key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/devxMani/naval-ai.git
   cd naval-ai
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory:
   ```env
   # NIA API Configuration
   NIA_API_KEY=your_nia_api_key
   NAVAL_NIA_SOURCE=your_naval_source_id
   
   # AI Gateway Configuration
   AI_GATEWAY_API_KEY=your_gateway_api_key
   ```

4. **Run the development server**
   ```bash
   pnpm dev
   ```

5. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📁 Project Structure

```
naval-ai/
├── app/
│   ├── api/
│   │   └── chat/
│   │       └── route.ts      # Chat API endpoint
│   ├── globals.css           # Global styles
│   ├── layout.tsx            # Root layout
│   └── page.tsx              # Home page
├── components/
│   ├── ui/                   # Reusable UI components
│   ├── chat.tsx              # Main chat component
│   ├── model-selector.tsx    # AI model selector
│   └── theme-toggle.tsx      # Dark/light mode toggle
├── lib/
│   ├── constants.ts          # Model configurations
│   ├── gateway.ts            # AI Gateway setup
│   ├── nia-tools.ts          # NIA API tools
│   └── utils.ts              # Utility functions
└── public/                   # Static assets
```

## 🔧 Available Tools

The AI assistant has access to specialized tools for searching Naval's content:

| Tool | Description |
|------|-------------|
| `searchEssays` | Semantic search across all Naval content |
| `browseEssays` | View the complete structure of available content |
| `listDirectory` | Explore content in specific categories |
| `readEssay` | Read the full content of any piece |
| `grepEssays` | Find specific phrases using pattern matching |
| `webSearch` | Search the web for recent information |

## 🎨 Key Naval Themes

The AI is trained to discuss Naval's core philosophies:

- 💰 **Wealth Creation** - Specific knowledge, leverage, and accountability
- 😊 **Happiness** - Happiness as a skill that can be trained
- 📚 **Learning** - The importance of reading and continuous learning
- 🧠 **Judgment** - Judgment over raw intelligence
- ⏳ **Long-term Thinking** - Compounding and patience
- 🕉️ **Philosophy** - Blending Eastern philosophy with modern rationalism

## 📝 Scripts

```bash
# Development
pnpm dev          # Start development server

# Production
pnpm build        # Build for production
pnpm start        # Start production server

# Code Quality
pnpm lint         # Run ESLint
pnpm type-check   # Run TypeScript type checking
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Naval Ravikant](https://nav.al/) for his wisdom and philosophy
- [Vercel](https://vercel.com/) for the AI SDK and hosting
- [NIA](https://trynia.ai/) for the content API
- [NIA Docs](https://docs.trynia.ai) for API documentation

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/devxMani">devxMani</a>
</p>
