<H3>ENTER YOUR NAME: Darshan V</H3>
<H3>ENTER YOUR REGISTER NO: 212224230050</H3>
<H3>DATE: </H3>
<H1 Align="center">Project Based Experiment<H1>
<H3>Objective:<H3>
To perform sentiment analysis on Facebook data and filter for messages, comments, or posts with negative feedback.
<H3>Program:</H3>
  
  ```py
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer

# Download NLTK resources 
nltk.download('vader_lexicon')

# Load the sentiment analyzer
sia = SentimentIntensityAnalyzer()

# Example Facebook data 
facebook_data = [
    "I love the new feature! It's amazing.",
    "The service was terrible. I'm very disappointed.",
    "Great job on the update!",
    "The product quality is poor. I won't be buying again.",
    
]

# Perform sentiment analysis and filter for negative feedback
negative_feedback = []

for message in facebook_data:
    sentiment_score = sia.polarity_scores(message)['compound']
    if sentiment_score < 0:  # Negative sentiment
        negative_feedback.append(message)

# Print the negative feedback
print("Negative Feedback:")
for feedback in negative_feedback:
    print(feedback)

 ```

<H3>Output:</H3>

![image](https://github.com/PriyankaAnnadurai/Project-Based-Experiment-AAI/assets/118351569/c6211e29-f9ba-41b1-a4b7-74a20541a9cc)

<H3>Inference:</H3>
 A sentiment analysis project using Facebook data provides valuable learning experiences in data handling, text processing, sentiment analysis, and ethical considerations, while also honing communication, problem-solving, and project management skills.
