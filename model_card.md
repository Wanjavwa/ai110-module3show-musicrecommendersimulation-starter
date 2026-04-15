# 🎧 Model Card: Music Recommender Simulation

## 1. Model Name  

**VibeMatcher 1.0**

---

## 2. Intended Use  

Generates personalized music recommendations based on user preferences for genre, mood, and energy level. Designed for educational exploration of content-based filtering algorithms, not for real-world production use.

---

## 3. How the Model Works  

The model scores songs by matching user preferences: +1.0 for genre match, +1.0 for mood match, and double-weighted energy similarity (2.0 * (1 - energy difference)). Songs are ranked by total score descending.

---

## 4. Data  

20 songs from a CSV file, representing diverse genres (pop, lofi, rock, hip-hop, etc.) and moods (happy, chill, intense, etc.). Energy ranges from 0.2 to 0.99. Added 10 songs to expand variety.

---

## 5. Strengths  

Works well for users with specific genre and mood preferences, accurately capturing energy levels. Recommendations for "Chill Lofi" matched low-energy songs.

---

## 6. Limitations and Bias 

Small dataset limits variety. Over-prioritizes energy when weight is high, potentially ignoring genre. Missing valence and tempo in scoring, biasing towards energy-focused users.

---

## 7. Evaluation  

Tested with 3 profiles: High-Energy Pop, Chill Lofi, Deep Intense Rock. Rankings shifted when doubling energy weight, showing sensitivity. Surprised by how energy closeness dominated.

---

## 8. Future Work  

Add valence and tempo features. Implement collaborative filtering. Improve diversity in top results.

---

## Personal Reflection

Biggest learning: How simple rules can create effective recommendations. AI tools helped brainstorm and debug code. Surprised by how energy weight shifts rankings drastically. Next, I'd add user feedback loops.  

---

## 9. Personal Reflection  

A few sentences about your experience.  

Prompts:  

- What you learned about recommender systems  
- Something unexpected or interesting you discovered  
- How this changed the way you think about music recommendation apps  
