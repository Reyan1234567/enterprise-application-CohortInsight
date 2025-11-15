| Full Name | ID Number |
| :--- | :--- |
| Eyosyas Solomon | UGR/9247/15 |
| Reyan Berhanu | UGR/1650/15 |
| Saba Habtamu | UGR/7546/15 |
| Biniam Markos | UGR/6500/15 |
| Yunus Kedir | UGR/8173/13 |

# CohortInsight – Spotify Audience Intelligence Platform

## 1. Business Problem
Podcast and music creators on Spotify often lack visibility into the broader listening habits of their audience beyond their own shows or tracks. They cannot easily understand what other podcasts, genres, or artists their listeners follow, making it difficult to tailor content, plan collaborations, or identify emerging trends.

**CohortInsight** solves this by allowing creators to invite their audience to anonymously share their Spotify listening data (top artists, top podcasts, genres, and playlists). Once a cohort reaches a threshold (e.g., 100 users), the system aggregates and analyzes the data to deliver powerful insights across the Spotify ecosystem.

---

## 2. Domain Decomposition & Business Value

### **Core Domain: Audience Intelligence Synthesis**
- **Business Value:** Converts raw Spotify listening data into actionable intelligence, enabling creators to understand audience behavior across the entire platform.

### **Supporting Subdomain: Cohort & Listener Management**
- **Business Value:** Handles invitation flows, listener onboarding, cohort grouping, and data consent management.

### **Generic Subdomain: Notification Service**
- **Business Value:** Sends notifications for cohort completion, insight availability, etc. Easily replaceable via common messaging providers.

---

## 3. Bounded Contexts within the Core Domain

### **3.1 Data Ingestion & Preparation Context**
- **Responsibility:** Collect anonymized Spotify listening data (Top Tracks, Top Artists, Top Podcasts, Genres). Clean, validate, de-duplicate, and enrich with metadata.

### **3.2 Pattern Analysis Context**
- **Responsibility:** Apply ML algorithms to detect listening trends, identify clusters, compare creator’s content with cohort preferences, and compute statistical insights.

### **3.3 Insight Synthesis Context**
- **Responsibility:** Generate human-readable insight summaries: genre affinities, audience overlap with other creators, discovery trends, and collaboration opportunities.

---

## 4. User Stories Spanning Multiple Bounded Contexts

### **User Story 1 – Cohort Completion Triggers Analysis**
As a Creator,  
I want analysis to begin when 100 listeners join my cohort  
so that I receive insights automatically.

### **User Story 2 – From Raw Data to Insights**
As a Creator,  
I want AI-generated insights from listener behavior  
so that I can make informed content and collaboration decisions.

### **User Story 3 – Insight Delivery**
As a Creator,  
I want to be notified when insights are ready  
so that I can review them immediately.

---

## 5. AI-Driven Feature

### **AI-Powered Listening Pattern Opportunity Mapping**
The system identifies:
- Overlapping audiences between creators  
- Fast-growing genres within the cohort  
- Podcast discovery pathways (e.g., “listeners who follow you also follow X”)  
- Underserved niches based on listener interests but low content supply  

**Example Insight:**  
“Your audience shows strong interest in motivational podcasts with short-form episodes. There is high demand but low supply for *5-minute productivity boosters*—a strong opportunity area.”
