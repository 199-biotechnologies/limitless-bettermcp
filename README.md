# Advanced Limitless MCP Server (v0.6.0) 🚀
![Version](https://img.shields.io/badge/version-0.6.0-blue) ![License](https://img.shields.io/badge/license-MIT-green) ![NPM](https://img.shields.io/npm/v/199bio-mcp-limitless-server)

An **intelligent MCP (Model Context Protocol) server** that transforms your Limitless Pendant data into actionable intelligence for AI tools like Claude, Windsurf, and others. Version 0.6.0 introduces the revolutionary **Speech Vitality Index (SVI)** - a single, reliable health score from quality conversations, replacing complex biomarkers with trustworthy simplicity.

## 📑 Table of Contents

- [🆚 Original vs Enhanced Comparison](#-original-vs-enhanced-comparison)
- [🚀 Quick Start](#quick-start-with-npx-no-installation-required)
- [🎯 Perfect for Claude AI Users](#-perfect-for-claude-ai-users)
- [📋 Prerequisites](#prerequisites)
- [🔧 Installation Options](#installation-options)
- [⚙️ Configuration](#configuration-client-side)
- [🏃 Running the Server](#running-the-server)
- [🛠️ Available MCP Tools](#️-available-mcp-tools-v050)
  - [🎯 Smart & Intuitive Tools](#-smart--intuitive-new)
  - [📚 Core Foundation Tools](#-core-foundation-tools)
- [💬 Real-World Examples](#-real-world-examples-with-v050-features)
  - [🧠 Health Monitoring Examples](#-health-monitoring-examples)
  - [🗣️ Communication Style Analysis](#️-communication-style-analysis)
  - [⚡ Performance Optimization](#-performance-optimization)
  - [📊 Trend Analysis](#-trend-analysis)
  - [🏥 Clinical-Grade Analysis](#-clinical-grade-analysis)
- [📅 Supported Natural Time Expressions](#-supported-natural-time-expressions-v050)
- [📝 Notes & Limitations](#notes--limitations)
- [🔬 Technical Architecture](#-technical-architecture)
- [🚧 Roadmap & Future Enhancements](#-roadmap--future-enhancements)
- [🤝 Contributing](#-contributing)
- [📚 Peer-Reviewed Documentation](#-peer-reviewed-documentation)

## 🆚 Original vs Enhanced Comparison

| Feature | Original v0.1.0 | Enhanced v0.5.0 | Improvement |
|---------|----------------|------------------|-------------|
| **Time Queries** | Manual date calculation required | Natural language: "today", "past week", "last Monday" | 🎯 **10x easier** |
| **Meeting Detection** | Manual log analysis | Automatic detection with participants, topics, action items | 🤖 **Fully automated** |
| **Search Scope** | Recent 20 logs only | Full history with relevance scoring | 🔍 **50x larger scope** |
| **Action Items** | Manual extraction from logs | Smart pattern recognition with priorities | ✅ **Intelligent extraction** |
| **Daily Insights** | None - manual analysis required | Comprehensive summaries with productivity metrics | 📊 **Complete analytics** |
| **Speaker Analysis** | Basic speaker names only | Full conversation analytics with patterns | 👥 **Deep relationship insights** |
| **Health Monitoring** | None | Speech Vitality Index (0-100) from quality conversations | 🧠 **Simple & Reliable** |
| **Data Quality** | All data analyzed | Only quality conversations (5+ min) analyzed | ✅ **100% Reliable** |
| **Complexity** | Not available | One clear score with trend analysis | 📊 **Actually Usable** |
| **Honesty** | N/A | "Insufficient data" when appropriate | 🎯 **Trustworthy** |
| **User Experience** | 3-5 tool calls for simple tasks | 1 tool call with intelligent results | ⚡ **5x faster workflows** |

**✨ What's New in v0.6.0 - The Simplification Update:**
- 🎯 **Speech Vitality Index (SVI)** - One reliable score (0-100) replacing 20+ complex biomarkers
- ✅ **Quality-First Analysis** - Only analyzes 5+ minute conversations with clear audio
- 📊 **Simple Components** - Fluency (words per burst), Energy (dynamic range), Consistency (stability)
- 🚫 **No Bad Data** - Rejects poor quality segments instead of statistical guessing
- 📈 **Clear Trends** - "Improving", "Stable", "Declining", or "Insufficient Data"
- 💡 **Actionable Insights** - "Have a conversation" not "Your pause duration is 2.3σ above normal"

**Why the Change?**
We applied Occam's Razor: Better to be a reliable flashlight than an unreliable lighthouse. The pendant records ~30% of your day randomly - trying to extract 24/7 health insights from this was like measuring running speed by randomly sampling your day. Now we focus on what we can measure well: quality conversations.

**Legacy Features (v0.4.0-v0.5.1):**
- Complex speech biomarkers with 20+ metrics (replaced by SVI)
- Population percentiles and statistical analysis (removed - context-dependent)
- Multiple health scores and predictions (simplified to one score)

**Previous v0.3.1 Features:**
- 📅 **50+ Natural Time Expressions** - "last month", "tomorrow", "this weekend", etc.
- 🎯 **Flexible Relative Dates** - "past 5 days", "in 2 weeks", "3 days ago"
- 💼 **Business Time Support** - Quarters (Q1-Q4), year references, month boundaries
- 🌅 **Enhanced Time Periods** - "yesterday afternoon", "tomorrow morning", "last night"

**Previous v0.3.0 Features:**
- 📄 **Raw Transcript Extraction** - Clean, AI-optimized transcript formats
- 🔬 **Detailed Technical Analysis** - Precision extraction of scientific/medical terms
- 🎯 **Multi-Format Support** - Raw text, verbatim, structured, timestamps
- 📊 **Enhanced Context Preservation** - Maximum technical detail retention

**Previous v0.2.0 Features:**
- 🕒 **Natural Time Queries** - "yesterday", "this morning", "past week"
- 🤝 **Smart Meeting Detection** - Automatic participant and topic extraction
- 🔍 **Full History Search** - Search ALL lifelogs with intelligent context
- 📊 **Daily Summaries** - Complete productivity insights and analytics
- 👥 **Speaker Analytics** - Detailed conversation analysis per person
- ✅ **Action Item Extraction** - Smart task recognition with priority inference

**Enhanced by:** Boris Djordjevic, 199 Longevity  
**Original Foundation by:** Ryan Boyle (ipvr9)

## Quick Start with npx (No Installation Required!)

You can run this intelligent MCP server directly using npx without any installation:

```json
{
  "mcpServers": {
    "limitless": {
      "command": "npx",
      "args": ["199bio-mcp-limitless-server"],
      "env": {
        "LIMITLESS_API_KEY": "<YOUR_LIMITLESS_API_KEY_HERE>"
      }
    }
  }
}
```

This automatically downloads v0.5.1 with advanced health monitoring features when your MCP client starts.

## 🎯 Perfect for Claude AI Users

The v0.5.0 upgrade transforms your Claude conversations with comprehensive health insights:

**Before:** "Let me check your logs... *reads through everything* ... based on my analysis..."  
**After:** "What action items came from today's meetings?" → *Instant intelligent response*

**Common Use Cases:**
- 💼 "Give me a summary of yesterday's meetings"
- ✅ "What do I need to do from today's conversations?"  
- 👥 "How much did I talk with my manager this week?"
- 🔍 "When did I last discuss the budget proposal?"
- 📊 "Show me my productivity insights for today"
- 🧠 "What's my speechclock?" - Get your Speech Vitality Score
- 📊 "Show me my speech age" - View your SVI trend over time
- ✅ "How's my speech health?" - Simple score with clear next steps

> **What's MCP?**  
> [Model Context Protocol](https://modelcontextprotocol.io/introduction) is an open standard for connecting AI models to external tools and data—think of it like the USB-C port or even the HTTP protocol for AI—universal, reliable, and designed for extensibility. The standard that everyone adopts. It enables rich integrations, custom workflows, and seamless communication between AI and the tools you use every day.

**IMPORTANT NOTE:** As of March 2025, the Limitless API **requires data recorded via the Limitless Pendant**. This server depends on real data recorded from your Limitless Pendant—it won't return anything meaningful without it. Ensure your Pendant is connected and recording.

**API Status:**
*   The official Limitless API is currently in **beta**. As such, it may occasionally be unreliable, subject to change, or experience temporary outages.
*   Requesting large amounts of data may sometimes result in **timeout errors** due to API constraints. The server includes a 120-second timeout per API call to mitigate this.
*   The Limitless API is under **active development**. This MCP server will be updated with new features as they become available.

## Prerequisites

*   Node.js (v18 or later required)
*   A Limitless account and API key ([Get one here](https://limitless.ai/developers))
*   **A Limitless Pendant (Required for data)**
*   An MCP Client application (e.g., Claude, Windsurf, Cursor, ChatWise, ChatGPT (coming soon!)) capable of spawning stdio servers and passing environment variables.

## Installation Options

### Option 1: Using npx (Recommended - No Installation)

Simply configure your MCP client to use npx as shown in the Quick Start section above. The server will be downloaded and run automatically.

### Option 2: Local Installation

1.  **Clone or download this project.**
2.  **Navigate to the directory:**
    ```bash
    cd mcp-limitless-server
    ```
3.  **Install dependencies:**
    ```bash
    npm install
    ```
4.  **Build the code:**
    ```bash
    npm run build
    ```

## Configuration (Client-Side)

This server expects the `LIMITLESS_API_KEY` to be provided as an **environment variable** when it is launched by your MCP client.

### For npx usage:

```json
{
  "mcpServers": {
    "limitless": {
      "command": "npx",
      "args": ["199bio-mcp-limitless-server"],
      "env": {
        "LIMITLESS_API_KEY": "<YOUR_LIMITLESS_API_KEY_HERE>"
      }
    }
  }
}
```

### For local installation:

You need to add a server configuration block to your MCP client's settings file. Below are two examples depending on whether you are adding this as your first server or adding it alongside existing servers.

**Example A: Adding as the first/only server**

If your client's configuration file currently has an empty `mcpServers` object (`"mcpServers": {}`), replace it with this:

```json
{
  "mcpServers": {
    "limitless": {
      "command": "node",
      "args": ["<FULL_FILE_PATH_TO_DIST_SERVER.js>"],
      "env": {
        "LIMITLESS_API_KEY": "<YOUR_LIMITLESS_API_KEY_HERE>"
      }
    }
  }
}
```

**Example B: Adding to existing servers**

If your `mcpServers` object already contains other servers (like `"notion": {...}`), add the `"limitless"` block alongside them, ensuring correct JSON syntax (commas between entries):

```json
{
  "mcpServers": {
    "some_other_server": {
      "command": "...",
      "args": ["..."],
      "env": {
        "EXAMPLE_VAR": "value"
      }
    },
    "limitless": {
      "command": "node",
      "args": ["<FULL_FILE_PATH_TO_DIST_SERVER.js>"],
      "env": {
        "LIMITLESS_API_KEY": "<YOUR_LIMITLESS_API_KEY_HERE>"
      }
    }
  }
}
```

**Important:**
*   Replace `<YOUR_LIMITLESS_API_KEY_HERE>` with your actual Limitless API key.
*   For local installation, replace `<FULL_FILE_PATH_TO_DIST_SERVER.js>` with the correct, **absolute path** to the built server script (e.g., `/Users/yourname/Documents/MCP/mcp-limitless-server/dist/server.js`).
*   MCP config files **cannot contain comments**. Remove any placeholder text and replace it with actual values.

## Running the Server

**For npx:** Your MCP client will automatically download and run the server when needed.

**For local installation:** 
1.  Ensure the server is built successfully (`npm run build`).
2.  Configure your MCP client as shown above.
3.  Start your MCP client application. It will launch the `mcp-limitless-server` process automatically when needed.

## 🛠️ Available MCP Tools (v0.5.0)

### 🎯 Smart & Intuitive (NEW!)

6.  **`limitless_get_by_natural_time`** - Natural language time queries ✨ **ENHANCED in v0.3.0**
    - **Basic:** "today", "yesterday", "tomorrow"
    - **Time periods:** "this morning", "yesterday afternoon", "last night", "tomorrow evening"
    - **Calendar:** "last month", "this month", "next month", "this year", "last year" 🆕
    - **Weeks:** "this week", "last week", "next week", "past 2 weeks" 🆕
    - **Weekends:** "this weekend", "last weekend", "next weekend" 🆕
    - **Relative:** "past 5 days", "3 days ago", "in 2 days", "recently", "the other day" 🆕
    - **Business:** "Q1", "Q2", "Q3", "Q4", "this quarter", "last quarter" 🆕
    - **Boundaries:** "beginning of the month", "end of the week", "start of the month" 🆕
    - **Same-day:** "earlier today", "earlier", "later today" 🆕
    - **Perfect for:** Natural conversation queries like "What did I discuss last month?"

7.  **`limitless_detect_meetings`** - Automatic meeting detection & analysis  
    - **Intelligence:** Participant extraction, topics, action items, duration
    - **Perfect for:** "What meetings did I have today?"

8.  **`limitless_search_conversations_about`** - Full history search with context
    - **Advanced:** Searches ALL lifelogs (not just recent 20), includes context
    - **Perfect for:** "When did I last discuss Project Alpha?"

9.  **`limitless_get_daily_summary`** - Comprehensive daily insights
    - **Analytics:** Meetings, action items, productivity metrics, key participants  
    - **Perfect for:** "Give me a summary of yesterday"

10. **`limitless_analyze_speaker`** - Detailed speaker analytics
    - **Insights:** Speaking time, topics, interaction patterns, frequency
    - **Perfect for:** "How much did I talk with Sarah this month?"

11. **`limitless_extract_action_items`** - Smart task extraction
    - **Intelligence:** Context-aware, priority inference, assignee detection
    - **Perfect for:** "What do I need to do from today's meetings?"

12. **`limitless_get_raw_transcript`** - Extract clean transcripts for AI processing 🆕
    - **Formats:** raw_text, verbatim, structured, timestamps, speakers_only
    - **Perfect for:** "Give me the exact transcript without formatting"

13. **`limitless_get_detailed_analysis`** - Technical precision analysis 🆕
    - **Focus areas:** technical, financial, decisions, research, all
    - **Perfect for:** "What were the exact specifications mentioned?"

14. **`speechclock`** / **`speechage`** - Speech Vitality Index (SVI) 🆕
    - **What it is:** A single, reliable health score (0-100) calculated from quality conversations only
    - **How it works:** 
      - ✅ **Quality First:** Only analyzes 5+ minute conversations with clear audio
      - 🎯 **Three Simple Components:** 
        - Fluency: Words per speech burst (not per minute)
        - Energy: Dynamic range and variation
        - Consistency: Stability throughout conversation
      - 📊 **Clear Trends:** "Improving", "Stable", "Declining", or "Insufficient Data"
    - **Why it's revolutionary:** No fake statistics from bad data - if we can't measure it well, we don't measure it
    - **Parameters:**
      - `time_expression` (optional): "past 7 days" (default), "today", "this week", etc.
      - `timezone` (optional): IANA timezone
      - `detailed` (optional): Show component scores breakdown
    - **Usage examples:**
      - "What's my speechclock?" → "Speech Vitality: 82/100, Trend: Stable"
      - "Show my speechage" → Simple score with actionable next steps
    - **Output:** 
      - Your SVI score (0-100) with confidence level
      - Trend direction with confidence percentage
      - Clear next action (e.g., "Have a 5+ minute conversation")
      - Recent score history (if available)

### 📚 Core Foundation Tools

1.  **`limitless_get_lifelog_by_id`**: Retrieves a single Pendant recording by its specific ID.
2.  **`limitless_list_lifelogs_by_date`**: Lists Pendant recordings for a specific date.
3.  **`limitless_list_lifelogs_by_range`**: Lists Pendant recordings within a date/time range.
4.  **`limitless_list_recent_lifelogs`**: Lists the most recent Pendant recordings.
5.  **`limitless_search_lifelogs`**: Searches title/content of *recent* Pendant recordings (limited scope).

## 💬 Real-World Examples with v0.5.0 Features

### 🧠 Speech Vitality Examples

**Basic Score Check:**
```
User: "What's my speechclock?"
Claude: Speech Vitality: 78/100
Trend: Stable (85% confidence)

Next Step: Your speech vitality is being tracked
```

**Insufficient Data:**
```
User: "Show my speechage"
Claude: Speech Vitality: --/100

Have a 5+ minute conversation to establish baseline
```

**Detailed View:**
```
User: "What's my speech vitality with details?"
Claude: Speech Vitality: 82/100
Trend: Improving (72% confidence)

Components:
• Fluency: 85/100
• Energy: 78/100
• Consistency: 83/100

Next Step: 2 more conversations needed for reliable trends
```

### 📊 Why Speech Vitality Index?

**The Problem:** The pendant records ~30% of your day randomly. Previous versions tried to extract 24/7 health insights from this partial data using complex statistics.

**The Solution:** Focus on what we can measure reliably - quality conversations. One clear score from good data beats 20 metrics from questionable data.

**Key Benefits:**
- ✅ 100% reliable data (quality conversations only)
- 🎯 One score you can actually understand
- 📊 Clear trends without statistical gymnastics
- 💡 Actionable next steps, not confusing metrics

## 📅 Supported Natural Time Expressions (v0.5.0)

The enhanced time parser now supports over 50 natural language expressions:

### Basic Time References
- `today`, `yesterday`, `tomorrow`
- `morning`, `afternoon`, `evening`, `tonight`
- `earlier today`, `earlier`, `later today`

### Specific Time Periods
- `yesterday morning`, `yesterday afternoon`, `yesterday evening`, `last night`
- `tomorrow morning`, `tomorrow afternoon`, `tomorrow evening`
- `this morning`, `this afternoon`, `this evening`

### Calendar Periods 🆕
- **Months**: `last month`, `this month`, `next month`
- **Years**: `last year`, `this year`
- **Quarters**: `Q1`, `Q2`, `Q3`, `Q4`, `this quarter`, `last quarter`

### Week & Weekend References 🆕
- `this week`, `last week`, `next week`
- `this weekend`, `last weekend`, `next weekend`

### Flexible Relative Expressions 🆕
- **Past**: `past N days/weeks/months` (e.g., `past 5 days`, `past 2 weeks`)
- **Ago**: `N days/weeks/months ago` (e.g., `3 days ago`, `2 weeks ago`)
- **Future**: `in N days/weeks/months` (e.g., `in 2 days`, `in a week`)

### Informal References 🆕
- `recently` (past 14 days)
- `the other day` (2-4 days ago)
- `a few days ago` (2-4 days ago)
- `a couple days ago` (exactly 2 days ago)

### Boundary References 🆕
- `beginning of the week`, `start of the week`
- `end of the week`
- `beginning of the month`, `start of the month`
- `end of the month`

### Day Names
- `monday`, `tuesday`, `wednesday`, etc.
- `last monday`, `next friday`
- `last tuesday` (most recent Tuesday)

## Notes & Limitations

🚫 **Pendant Required**  
This server depends on data generated by the Limitless Pendant.

🧪 **API Beta Status**  
The Limitless API is in beta and may experience occasional instability or rate limiting. Large requests might result in timeouts (e.g., 504 errors).

🔍 **Search Scope**  
`limitless_search_lifelogs` only scans a limited number of recent logs (default 20, max 100). It does *not* search your full history — use listing tools first for broader analysis.

⚠️ **Error Handling & Timeout**  
API errors are translated into MCP error results. Each API call has a 120-second timeout.

🔌 **Transport**  
This server uses `stdio` and is meant to be launched by an MCP-compatible client app.

## 🔬 Technical Architecture

**v0.5.0 Advanced Features:**
- **Natural Language Processing:** Robust time expression parser with timezone support
- **Machine Learning Patterns:** Intelligent meeting detection using speaker analysis
- **Context-Aware Search:** Full-text search with relevance scoring and context inclusion
- **Analytics Engine:** Comprehensive daily summaries with productivity insights
- **Relationship Intelligence:** Speaker analytics with temporal patterns

**Built with Production Standards:**
- TypeScript with comprehensive type safety
- Modular architecture with separation of concerns  
- Robust error handling and graceful degradation
- Memory-efficient processing for large datasets
- Timezone-aware processing throughout

## 🚧 Roadmap & Future Enhancements

### 📋 Completed Features ✅
- ✅ Natural language time parsing with timezone support
- ✅ Intelligent meeting detection with speaker analysis
- ✅ Full history search with context and relevance scoring
- ✅ Comprehensive daily summaries with productivity insights
- ✅ Speaker analytics with conversation patterns
- ✅ Smart action item extraction with priority inference
- ✅ Speech rhythm analysis with entropy calculation
- ✅ Disfluency detection (fillers, repairs, hesitations)
- ✅ Energy and fatigue assessment with predictions
- ✅ Personal baseline tracking and deviation alerts
- ✅ Environmental activity analysis and sleep detection
- ✅ Integrated health scoring (0-100 scales)
- ✅ Production-quality TypeScript architecture
- ✅ Robust error handling and performance optimization

### 🔮 Planned Features (v0.5.0+)
- 🔄 **Intelligent Caching Layer** - Smart caching for repeated queries
- 🧪 **Unit Test Suite** - Comprehensive testing for all features
- 📈 **Advanced Analytics** - Weekly/monthly productivity trends
- 🎯 **Goal Tracking** - Action item completion tracking
- 🔔 **Smart Notifications** - Proactive insights and reminders
- 📊 **Custom Reports** - Configurable productivity reports
- 🤖 **AI Insights** - Machine learning-powered conversation insights
- 🔍 **Semantic Search** - Meaning-based search beyond keywords
- 📝 **Meeting Templates** - Auto-generate meeting notes formats
- 🔗 **Integration APIs** - Connect with Notion, Todoist, Calendar apps

## 🤝 Contributing

Enhanced by **Boris Djordjevic** from **199 Longevity** with advanced AI features.  
Original foundation by **Ryan Boyle** (ipvr9).

Have ideas, improvements, or feedback? Feel free to open an issue or PR—contributions are always welcome! Let's keep pushing the boundaries of what's possible with wearable context and intelligent tools.

**Repository:** [https://github.com/199-biotechnologies/mcp-limitless-enhanced](https://github.com/199-biotechnologies/mcp-limitless-enhanced)  
**NPM Package:** [https://www.npmjs.com/package/199bio-mcp-limitless-server](https://www.npmjs.com/package/199bio-mcp-limitless-server)

## 📚 Documentation

### Current Implementation (v0.6.0+)

- **[Speech Vitality Index: A Simplified Approach](docs/SPEECH_VITALITY_INDEX.md)** - The current implementation using a single, reliable score from quality conversations. Explains the rationale for simplification and the methodology behind SVI.

### Legacy Documentation (v0.4-0.5)

- **[Speech Biomarker Analysis: Methodology and Clinical Validation](docs/SPEECH_BIOMARKERS.md)** - Complex statistical methodology with 20+ biomarkers (deprecated)
- **[Advanced Speech Biomarkers: Enhanced Health Monitoring](docs/ADVANCED_SPEECH_BIOMARKERS.md)** - Rhythm analysis, disfluency detection, and energy assessment (deprecated)

The legacy documentation is preserved for reference but the complex approach has been replaced with the simpler, more reliable Speech Vitality Index.