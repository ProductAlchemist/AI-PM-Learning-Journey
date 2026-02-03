# AI PM Learning Journey

**Building AI/LLM product expertise through hands-on experimentation and systematic learning**

This repository documents my journey from fintech PM to AI-enabled PM — combining platform thinking, behavioral design, and LLM capabilities.

---

## Why This Learning Path

**Context:** PM at Porter (approaching 4 years) with expertise in:
- Platform development (taxation engine, lending infrastructure)
- Behavioral product design (recovery mechanisms, compliance nudges)
- Fintech domain depth (regulatory compliance, fraud prevention, transaction systems)

**Gap Identified:** AI/LLM is transforming fintech products, but most PMs lack hands-on understanding.

**Opportunity:** Combine existing fintech expertise + platform thinking WITH AI/LLM technical depth = rare skillset.

**Goal:** Become PM who can design and ship AI-enabled fintech products (not just "have AI team figure it out").

---

## Why NOW (Strategic Timing)

### 1. Fintech is AI-First in 2026

**Traditional Fintech (2022-2024):**
- Rule-based credit scoring
- Manual fraud review
- Static compliance checks
- Batch transaction processing

**AI-Enabled Fintech (2025-Present):**
- LLM-powered credit assessment (analyze unstructured data — social media, transaction narratives)
- Real-time fraud detection with anomaly models
- Conversational compliance (chatbots that explain regulations)
- Predictive transaction monitoring (prevent issues before they happen)

**Porter Context:**
- Current lending: CIBIL score + manual underwriting
- AI-enabled future: Analyze partner behavior patterns (delivery completions, earnings consistency, app usage) for better credit assessment
- Current fraud: Rule-based blacklist (PAN, Aadhaar, DL, RC)
- AI-enabled future: Behavioral anomaly detection (identify fraudulent patterns before first transaction)

---

### 2. Senior PM Roles Require AI Product Judgment

**What Hiring Managers Ask (2026 Job Market):**
- "How would you evaluate LLM vs traditional ML for this use case?"
- "What are the latency constraints for real-time RAG systems?"
- "How do you measure quality for generative AI outputs?"

**Current Gap:** Can talk about AI conceptually, but can't evaluate technical tradeoffs or communicate with AI/ML engineers effectively.

**Solution:** Hands-on learning (same approach as PlayLoop Studios — build to understand).

---

### 3. Platform Thinking + AI = Force Multiplier

**What I Already Know (Platform Thinking):**
- Extensible systems (taxation engine TCS-ready before TCS existed)
- Behavioral mechanisms (flexible payment loop psychology)
- Systems architecture (coordinated infrastructure, not isolated features)

**What AI Adds (Force Multiplier):**
- Personalization at scale (LLMs adapt to user context automatically)
- Unstructured data processing (analyze text, not just structured fields)
- Predictive capabilities (prevent problems before they happen)

**Example - Porter Lending + AI:**
- **Current:** Rule-based credit scoring (CIBIL + income verification)
- **AI-Enabled:** LLM analyzes partner conversation history, delivery notes, support tickets → identifies repayment intent signals
- **Platform Thinking:** Build RAG system that works for lending AND fraud detection AND compliance (shared infrastructure)

---

## Progress To Date (Nov 2025 → Feb 2026)

### Technical Learning Achieved

**Starting Point (Nov 22, 2025):**
- Zero development experience
- No understanding of React, TypeScript, or modern web development
- Never deployed an application to production
- PM who could talk about tech but couldn't build with tech

**3-Month Journey:**

**Month 1 (Nov 2025): Foundations**
- Installed: Node.js, Git, VS Code, Claude Code CLI
- First "Hello World" React component (Nov 28)
- Learned: Component structure, JSX syntax, props vs state
- **Breakthrough:** Realized React components = product modules (similar mental model to Porter's platform architecture)

**Month 2 (Dec 2025): Building Real Applications**
- Built **PlayLoop Studios** - 2 complete games deployed to production
  - Tic-Tac-Toe: Minimax AI algorithm (unbeatable), multiplayer with Firebase real-time sync
  - Snake: Game loop timing, collision detection, mobile touch controls
- Learned: React 19, TypeScript, Firebase (Realtime Database, Auth, Analytics), Tailwind CSS, Vite
- **Challenge:** Understanding game loops (setInterval vs requestAnimationFrame) - similar to order processing loops at Porter
- **Deployed:** playloop-studios.vercel.app (live with 2 working games)

**Month 3 (Jan 2026): Advanced Features & New Projects**
- Built **Cipher** - Daily word puzzle (Wordle clone)
  - React + TypeScript + Firebase
  - 2,000+ players engaging daily
  - Word validation with industry-standard lists (answers + valid guesses)
- Built **YouTube Automation System** - Video generation pipeline
  - MoviePy for video rendering
  - Upload automation
  - A/B testing framework
- **Challenge:** Word list validation - learned to research industry standards (official Wordle implementation) before building
- **Deployed:** cipher-daily.vercel.app (live daily puzzle)

**Skills Acquired (Proof: 3 Live Production Apps):**

*Frontend Development:*
- React 19 (concurrent rendering, hooks, state management)
- TypeScript (type safety, interfaces, generics)
- Tailwind CSS (utility-first, responsive design)
- Vite (build tooling, ESM-based dev server)

*Backend & Infrastructure:*
- Firebase Realtime Database (NoSQL, real-time sync, sub-100ms latency)
- Firebase Auth (anonymous users for multiplayer)
- Firebase Analytics (visitor tracking, event logging)
- API integration (REST, real-time listeners)

*DevOps & Deployment:*
- Vercel (edge network, serverless, auto-deploy on push)
- Git/GitHub workflows (commits, branches, pull requests)
- CI/CD concepts (build → test → deploy)

*Game Development Concepts:*
- Game loops (timing, frame rate management)
- Collision detection algorithms
- State synchronization (multiplayer)
- AI algorithms (minimax with alpha-beta pruning)

**PM Application Learnings:**

*1. Technical Tradeoff Evaluation:*
- **Before:** "Let's add real-time features" (vague understanding)
- **After:** "Real-time via Firebase = <100ms sync but vendor lock-in, WebSocket = full control but DevOps complexity" (can evaluate build vs buy)
- **Porter Impact:** Better architecture discussions with engineering (understand state management = order lifecycle complexity)

*2. Feasibility Assessment:*
- **Before:** "Is this hard?" (relied on engineering estimates)
- **After:** Can prototype features myself to validate feasibility before committing team resources
- **Porter Impact:** Can push back on "impossible" claims when I know the technical constraints

*3. Scalability Thinking:*
- **Before:** "Will this scale?" (surface-level question)
- **After:** Understand Firebase free tier (100 concurrent connections) vs enterprise needs (50K partners × 1M transactions)
- **Porter Impact:** Know when to optimize for speed vs cost, MVP architecture ≠ enterprise architecture

*4. Technical Debt Recognition:*
- **Before:** Technical debt was abstract concept
- **After:** Can identify overly complex state management, performance bottlenecks, architectural shortcuts
- **Porter Impact:** Better prioritization - know where technical debt lives and what it costs to fix

**Proof of Work:**
- ✅ playloop-studios.vercel.app (2 games, multiplayer, production-ready)
- ✅ cipher-daily.vercel.app (daily puzzle, 2,000+ players)
- ✅ GitHub repositories with meaningful commit history (not just final code dumps)
- ✅ Can ship React + TypeScript + Firebase apps independently

**What This Unlocked:**
- Credibility with engineering teams (PMs who code are respected)
- Faster prototyping (validate ideas without committing team resources)
- Better product judgment (understand what's hard vs easy technically)
- **Interview differentiator:** BharatPe interviewer got excited - "Why didn't you mention this earlier? This should be in your resume!"

---

## Learning Roadmap (What's Next)

### Phase 1: ✅ COMPLETED (Nov 2025 → Jan 2026)

**Original Goal:** Understand core AI/LLM concepts and terminology

**What Actually Happened:**
- Skipped theoretical learning, jumped straight to building production apps
- Learned React/TypeScript/Firebase through hands-on game development
- Achieved: Can ship production web applications independently

**Unexpected Outcome:** Technical credibility became interview differentiator (AI PM roles value hands-on building)

---

### Phase 2: AI/LLM Integration (Current - Feb 2026 Onwards)

**Goal:** Add AI/LLM capabilities to existing technical foundation

**Focus Areas:**
- LLM basics (transformer architecture, tokens, embeddings, context windows)
- Prompt engineering (zero-shot, few-shot, chain-of-thought prompting)
- RAG systems (retrieval-augmented generation architecture)
- Vector databases (Pinecone, Weaviate, Chroma)

**Hands-On Projects (Building on Cipher/PlayLoop Base):**
- Add AI hint system to Cipher (LLM suggests word patterns without giving answer)
- Build document Q&A chatbot using RAG (Porter policy docs use case)
- Experiment with prompt engineering (compare zero-shot vs few-shot for game AI)

**Porter Connection:**
- How would LLM-powered chatbot answer partner questions about tax deductions?
- How would RAG system retrieve relevant loan eligibility criteria from policy docs?
- Can AI detect fraudulent patterns in partner behavior (anomaly detection)?

---

### Phase 2: Practical Application (Q2 2026)

**Goal:** Build AI-enabled product prototypes

**Focus Areas:**
- Fine-tuning LLMs (domain-specific adaptation)
- Evaluation metrics (precision/recall for AI outputs)
- Latency optimization (real-time constraints)
- Cost management (token usage, API costs)

**Hands-On Projects:**
- Fintech chatbot (loan eligibility explainer)
- Fraud detection prototype (anomaly identification)
- Compliance assistant (regulatory Q&A with citations)

**Porter Connection:**
- Build prototype: Partner asks "Why was tax deducted?" → LLM explains TDS rules in simple language with legal citations
- Build prototype: Detect fraudulent onboarding attempts by analyzing document upload patterns + text inconsistencies

---

### Phase 3: Production Considerations (Q3 2026)

**Goal:** Understand how to ship AI products to production

**Focus Areas:**
- Monitoring & observability (how to detect LLM degradation)
- Safety & guardrails (preventing harmful outputs)
- A/B testing AI features (measuring quality, not just metrics)
- Fallback strategies (what happens when LLM fails?)

**Hands-On Projects:**
- Implement guardrails (content filtering, fact-checking)
- Build monitoring dashboard (token usage, latency, error rates)
- Design A/B test for AI feature (control vs treatment measurement)

**Porter Connection:**
- If LLM explains tax deductions incorrectly → compliance risk → how to prevent?
- If fraud detection model has false positives → partner churn → how to balance precision/recall?

---

## Key Questions I'm Exploring

### 1. When to Use LLMs vs Traditional ML?

**LLM Strengths:**
- Unstructured text processing (partner feedback, support tickets)
- Flexible reasoning (adapt to new scenarios without retraining)
- Natural language interfaces (conversational products)

**Traditional ML Strengths:**
- Structured data (transaction amounts, timestamps, cohort classifications)
- Real-time predictions (millisecond latency)
- Explainability (clear feature importance)

**Porter Example:**
- **Fraud Detection:** Traditional ML (analyze structured transaction patterns, need real-time scoring)
- **Partner Support:** LLM (answer unstructured questions, conversational interface)

---

### 2. How to Measure Quality for Generative AI?

**Traditional Product Metrics:**
- CTR, conversion rate, retention (quantifiable)

**AI Product Metrics:**
- Factual accuracy (how to measure for generative outputs?)
- Hallucination rate (how to detect?)
- User satisfaction (qualitative + quantitative mix)

**Learning Focus:** How to design evaluation frameworks for AI features (not just ship and hope).

---

### 3. What Are Latency Constraints for Real-Time AI?

**Porter Context:**
- Order assignment: < 100ms (driver gets matched to order instantly)
- Tax calculation: < 50ms (real-time deduction at order level)
- Fraud check: < 200ms (onboarding shouldn't feel slow)

**AI Considerations:**
- LLM inference: 500ms - 2s (too slow for real-time decisioning)
- RAG system: 1-3s (acceptable for explanatory features, not transactional)
- Vector similarity search: < 100ms (fast enough for real-time recommendations)

**Learning Focus:** When is AI fast enough? When do you need caching, pre-computation, or traditional rules?

---

## How This Connects to Porter Work

### Use Case 1: Lending - Credit Assessment

**Current State:**
- CIBIL score + income verification (structured data only)
- Manual underwriting for edge cases
- Binary decision (approve/reject)

**AI-Enabled Future:**
- LLM analyzes unstructured data (partner behavior patterns, delivery completion notes, support interactions)
- Identifies intent signals (partner who completes 95% of deliveries vs partner who frequently cancels)
- Risk scoring with explanations ("Approved because consistent earnings + high delivery completion + no compliance issues")

**Platform Thinking:**
- RAG system retrieves similar partner profiles (behavioral patterns match)
- Same infrastructure powers lending + fraud detection + compliance (shared embeddings)

---

### Use Case 2: Taxation - Partner Education

**Current State:**
- Tax deductions happen automatically (rule-based engine)
- Partners don't understand why (support tickets: "Why was money deducted?")
- Manual explanations by support team (not scalable)

**AI-Enabled Future:**
- Conversational interface: Partner asks "Why was ₹500 deducted?" → LLM explains TDS rules in simple language
- Personalized explanations (adapts to partner's PAN status, Aadhaar linkage, vehicle count)
- Cites legal source (links to IT Act section, builds trust)

**Platform Thinking:**
- Same LLM powers tax explanations + loan eligibility explanations + compliance FAQs (shared knowledge base)

---

### Use Case 3: Fraud Prevention - Behavioral Anomaly Detection

**Current State:**
- Rule-based blacklist (blocks known fraudulent documents)
- Reactive (only catches repeat offenders)
- No behavioral signals (only document matching)

**AI-Enabled Future:**
- Analyze behavioral patterns (upload timing, document quality, text consistency)
- Predictive (flag suspicious onboarding BEFORE first transaction)
- Adaptive (learns new fraud patterns automatically)

**Platform Thinking:**
- Vector embeddings capture partner behavior (onboarding patterns, transaction history, app usage)
- Same embeddings power fraud detection + credit assessment + churn prediction (shared representation)

---

## Proof of Learning (Public Artifacts)

**Current Projects:**
- [PlayLoop Studios](https://github.com/ProductAlchemist/playloop-studios) - React + Firebase (demonstrates learning velocity)
- [Porter Case Studies](https://github.com/ProductAlchemist/porter-case-studies) - Fintech domain depth (platform thinking + behavioral design)

**AI Learning Artifacts (In Progress):**
- Chatbot prototype (OpenAI API integration)
- RAG experiment (document Q&A system)
- Prompt engineering examples (zero-shot, few-shot, chain-of-thought)

**Target (Q2 2026):**
- Fintech AI prototype (lending, fraud, or compliance use case)
- Technical writeup (architecture decisions, tradeoffs, learnings)
- Public demo (live working prototype, not just slides)

---

## Resources I'm Using

**Courses & Learning:**
- OpenAI API documentation (hands-on experimentation)
- LangChain tutorials (RAG system building)
- Vector database documentation (Pinecone, Weaviate)
- AI PM communities (practical product discussions)

**Porter Connection:**
- Not generic AI learning — every concept mapped to Porter use case
- Example: Learning RAG → immediately ask "How would this work for tax policy retrieval?"

**Meta-Learning:**
- Same approach as PlayLoop Studios (build to understand, not just read documentation)
- Document learnings publicly (this repository)

---

## Why This Matters for Senior PM Roles

**What Hiring Managers Want (2026 Market):**
- PMs who can evaluate AI technical tradeoffs (not just "let's use AI")
- PMs who understand when AI adds value vs when traditional solutions better
- PMs who can design evaluation frameworks for AI products (quality measurement)
- PMs who can communicate with AI/ML engineers effectively (technical depth)

**What This Learning Path Provides:**
- Hands-on understanding (not just conceptual)
- Fintech-specific application (domain expertise + AI)
- Platform thinking (shared infrastructure for AI capabilities)
- Production considerations (monitoring, safety, cost management)

**Combined Skillset (Rare in Market):**
- Fintech domain expertise (Porter: lending, taxation, fraud)
- Platform thinking (extensible systems, coordinated infrastructure)
- Behavioral design depth (psychology-driven mechanisms)
- AI/LLM technical depth (hands-on prototyping capability)

**This is what Senior PM at AI-first fintech companies requires.**

---

## Current Status (Feb 2026)

**Phase 1 Progress:**
- ✅ Installed OpenAI API, experimented with basic prompts
- ✅ Built simple chatbot prototype (Q&A about Porter use cases)
- 🚧 Learning RAG architecture (document retrieval systems)
- 🚧 Experimenting with vector databases (embeddings, similarity search)

**Next Milestones:**
- Q2 2026: Phase 2 complete (fintech AI prototype live)
- Q3 2026: Phase 3 complete (production considerations documented)
- Target: Core AI PM competency by end of Q2 2026

---

## Connect

**GitHub:** [ProductAlchemist](https://github.com/ProductAlchemist)
**LinkedIn:** [kshitijkulkarni-productmanager](https://www.linkedin.com/in/kshitijkulkarni-productmanager/)
**Email:** kshitijkulkarni95@gmail.com

**Currently exploring:** Senior PM roles (Platform PM, Growth PM, Fintech PM, AI PM) where platform thinking + behavioral design + AI/LLM expertise combine at scale.

**Open to:** Conversations about AI in fintech, PM learning paths, or collaboration on AI product experiments.
```

### Rationale for Changes

**From Previous (Generic):**
- Listed AI learning topics
- No connection to existing expertise
- No strategic rationale ("why NOW")

**To This (Strategic + Connected):**
- **Why NOW:** Connects to 2026 fintech market (AI-first products, hiring manager questions)
- **Porter use cases:** Every AI concept mapped to concrete fintech application (not generic learning)
- **Phased roadmap:** Foundational → practical → production (clear progression)
- **Key questions explored:** When to use LLMs vs traditional ML, how to measure quality, latency constraints
- **Platform thinking connection:** Shows how AI capabilities become shared infrastructure (not isolated features)
- **Combined skillset:** Positions as "fintech expert + platform thinker + behavioral designer + AI depth" (rare combination)

**What Makes This Compelling:**
1. Strategic timing (why NOW matters)
2. Domain-specific (fintech AI, not generic AI)
3. Connected to existing work (Porter use cases throughout)
4. Phased roadmap (clear progression, not random experimentation)
5. Practical focus (hands-on prototypes, not just courses)