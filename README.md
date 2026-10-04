# 🎨 Kalaverse

### Preserving traditional craftsmanship through interactive learning

Kalaverse is a web-based social learning platform that helps **independent artists, artisans, and traditional craft practitioners** share their work and teach their techniques through **interactive AR-assisted tutorials**.

Instead of relying only on passive videos or written instructions, Kalaverse combines:

**Artisan knowledge + Social discovery + Structured tutorials + Hand tracking + AI feedback**

The goal is not to replace the artist with AI, but to use technology to **amplify human expertise, preserve traditional knowledge, and make hands-on learning more accessible.**

---

# 🌍 Problem

Traditional art and craft knowledge is often passed from **master to apprentice**.

The most important parts of many crafts are difficult to communicate through text alone:

* Hand position
* Finger movement
* Timing
* Movement direction
* Relative positioning
* Repetition
* Technique

Although platforms such as YouTube provide enormous amounts of educational content, they are primarily **passive learning experiences**.

A learner may watch a craft tutorial but still struggle to answer:

> "Am I performing this movement correctly?"

At the same time, independent artists and traditional artisans often struggle with:

* Digital visibility
* Discoverability
* Reaching new learners
* Converting expertise into structured tutorials
* Preserving tacit knowledge

This creates a gap between **existing craft knowledge and modern digital learning.**

---

# ❓ Why Kalaverse?

The knowledge already exists.

The problem is **how that knowledge is discovered, taught, practiced, and preserved digitally.**

Kalaverse addresses both sides of the problem:

### For experts

It provides a digital space to:

* Build a profile
* Share their work
* Publish tutorials
* Teach learners
* Preserve structured craft knowledge

### For learners

It provides:

* Expert discovery
* Tutorial discovery
* Interactive practice
* Real-time hand tracking
* AI-generated guidance

---

# 💡 Solution

Kalaverse combines a social platform with interactive AR-assisted learning.

The basic learning cycle is:

```text
Expert Knowledge
       ↓
Structured Tutorial
       ↓
Learner Practice
       ↓
Webcam
       ↓
MediaPipe Hand Tracking
       ↓
Craft-specific Rule Engine
       ↓
Practice Result
       ↓
Gemini AI
       ↓
Human-readable Feedback
```

The expert remains the source of craft knowledge.

AI and computer vision act as **supporting tools** that help the learner practice.

---

# ✨ Key Features

### 👨‍🎨 1. Expert Profiles

Experts can create profiles containing:
* Biography
* Experience
* Contact information
* Tutorials

### 📱 2. Social Feed

Experts and learners can create craft-related posts.
This allows users to discover creators organically instead of treating the platform only as a course marketplace.

### 📚 3. Tutorial Publishing

Experts can create tutorials containing:
* Description
* Category
* Free/Paid status
* Tutorial steps
* AR tracking actions

### 🧑‍🎓 4. Learner Features

Learners can:
* Browse the social feed
* Discover experts
* Open expert profiles
* Browse tutorials
* Access free tutorials
* View paid tutorial information
* Start AR-assisted practice
  

# 🖐️ Interactive AR Practice

The main technical feature of Kalaverse is the AR-assisted practice system.
The learner uses a webcam while following a tutorial.
The system observes hand movements and checks them against the expected action for the current tutorial step.
The learner does not need special VR hardware.A normal webcam is sufficient for the MVP.

# 🏗️ System Architecture

```text
                         KALAVERSE
                              │
              ┌───────────────┴───────────────┐
              │                               │
           EXPERT                          LEARNER
              │                               │
       Create Profile                   Create Profile
              │                               │
         Create Posts                   View Feed
              │                               │
       Create Tutorials                Discover Experts
              │                               │
       Define AR Steps                 View Tutorials
              │                               │
              └───────────────┬───────────────┘
                              │
                         REST API
                              │
                    ┌─────────┴─────────┐
                    │                   │
                Backend              Database
                    │                   │
                    │                MongoDB
                    │
          ┌─────────┴─────────┐
          │                   │
      MediaPipe            Gemini
          │                   │
   Hand Landmarks       AI Feedback
          │                   │
          └─────────┬─────────┘
                    │
              Learner Feedback
```

# 🧰 Technology Stack

* **React.js**
* **Vite**
* **Tailwind CSS**
* JavaScript / TypeScript
* **Node.js**
* **Express.js**
* **Google MediaPipe**
* Hand Landmarker
* **Google Gemini API**

> **Kalaverse — where traditional knowledge meets interactive learning.**

**Preserve the craft.
Empower the creator.
Teach the next generation.**
