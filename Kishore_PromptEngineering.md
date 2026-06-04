# Prompt Engineering Portfolio
Name: Kishore J


Date: 04/06/2026


LLM Used: Gemini 1.5 Pro

## Part 1: Prompt Design & Iteration

### 1.1 Scenario A: Technical Explanation
**Goal:** Explain a complex technical concept (Blockchain) to a 10-year-old.
**Initial Prompt (V1):** Explain blockchain to a 10-year-old.
**Final Prompt (V3):** You are an expert elementary school teacher. Explain how a blockchain works to a 10-year-old using the analogy of a shared digital notebook that everyone can see but no one can erase. Keep the tone enthusiastic and limit the explanation to three short paragraphs.
**Final Output:**
"Imagine you and your friends have a magical digital notebook where you keep track of who traded which Pokémon cards. Whenever someone makes a trade, they write it down in the notebook. But here is the cool part: the moment they write it, a copy of that exact page magically appears in everyone else’s notebooks, too! 

Because everyone has the exact same copy, no one can ever cheat or sneakily erase a trade. If someone tries to change their notebook to say they have a rare Charizard, all the other friends will look at their own notebooks, see it doesn't match, and say, 'Hey, that's not right!' 

That is exactly what a blockchain is! Instead of Pokémon cards, adults use it to trade digital money or important information. It is just a giant, shared digital notebook that everyone helps watch over, making it incredibly safe and impossible to fake!"

### 1.1 Scenario B: Professional Email
**Goal:** Draft an email declining a job offer politely while expressing continued interest in the company.
**Initial Prompt (V1):** Write an email declining a job offer but say I still like the company.
**Final Prompt (V3):** You are a senior business professional writing to a hiring manager. Draft a concise, polite email declining a job offer for the Senior Analyst role. Explain that the timing isn't right due to accepting a competing offer that aligns better with your current trajectory, but emphasize your deep respect for their mission and desire to stay connected for future leadership roles.
**Final Output:**
Subject: Job Offer - Senior Analyst - [Your Name]
 
Dear Hiring Manager,
 
Thank you so much for offering me the Senior Analyst position. I deeply appreciate the time you and the team took to speak with me about the role and share more about the exciting direction the company is heading.
 
After careful consideration, I must respectfully decline the offer at this time. I have recently accepted a competing offer that aligns a bit more closely with my current career trajectory. This was a difficult decision, as I have immense respect for your team's mission and the fantastic culture you are building.
 
I would love to stay in touch and keep the door open for potential future opportunities, particularly as my career progresses toward leadership roles. 
 
Thank you again for your time, consideration, and this wonderful opportunity. I wish you and the team the absolute best.
 
Warm regards,
Kishore J

### 1.1 Scenario C: Creative Content
**Goal:** Generate a creative marketing tagline for a new eco-friendly water bottle brand.
**Initial Prompt (V1):** Write a tagline for a new eco-friendly water bottle.
**Final Prompt (V3):** You are a creative director at a top advertising agency. Brainstorm a punchy, 3-to-5 word tagline for a premium eco-friendly water bottle brand called "TideSaver," which is made entirely from recycled ocean plastic. The tone should be empowering and modern. Give me your single best option.
**Final Output:**
TideSaver: Drink Deep. Save the Seas.

### 1.2 Iteration Documentation
| Scenario | Version | Prompt | What Changed | Why This Improved the Output |
| :--- | :--- | :--- | :--- | :--- |
| **A** | V1 | Explain blockchain to a 10-year-old. | N/A | N/A |
| **A** | V2 | You are an expert elementary school teacher. Explain how a blockchain works to a 10-year-old. Use an analogy they would understand, like sharing a digital notebook. | Added Role and Context. | The tone shifted from dry technical jargon to a warm, engaging teaching style. |
| **A** | V3 | You are an expert elementary school teacher. Explain how a blockchain works to a 10-year-old using the analogy of a shared digital notebook... | Added Constraints (enthusiastic, three paragraphs). | Forced the output to be concise, punchy, and highly focused on the exact mechanics of the analogy. |
| **B** | V1 | Write an email declining a job offer but say I still like the company. | N/A | N/A |
| **B** | V2 | You are a senior business professional. Write an email to a hiring manager declining a job offer for the Senior Analyst role... | Added Role and Context. | Established proper business etiquette and a realistic corporate scenario. |
| **B** | V3 | You are a senior business professional writing to a hiring manager... Explain that the timing isn't right due to accepting a competing offer... | Added specific Context/Reasoning. | Providing a specific reason made the email sound authentic, respectful, and highly customized. |
| **C** | V1 | Write a tagline for a new eco-friendly water bottle. | N/A | N/A |
| **C** | V2 | Write 5 creative taglines for a new brand of eco-friendly water bottles made from ocean plastic. Make them catchy and short. | Added Context and Constraints. | Focused the AI on the unique selling proposition (ocean plastic). |
| **C** | V3 | You are a creative director at a top advertising agency. Brainstorm a punchy, 3-to-5 word tagline for a premium eco-friendly water bottle brand called "TideSaver"... | Added Role, Brand Details, and Tone Constraints. | Output became much sharper, premium, and ready for a real-world billboard. |

### 1.3 Role and Context Analysis
Integrating specific roles and context drastically transforms the quality of an LLM's output. By assigning a role (like "expert elementary school teacher"), you explicitly tell the AI which vocabulary set, tone, and professional standard to adopt. Furthermore, adding precise context removes ambiguity, forcing the AI to generate highly customized and actionable content rather than relying on broad, unhelpful 
placeholders.

## Part 2: Temperature & Parameter Control

### 2.1 Temperature Experimentation

**Chosen Task:** Creating a short story opening (2-3 sentences)
**Prompt Used:** "Write a short story opening (exactly 2-3 sentences) about a detective walking into a dusty antique shop."

**Test 1: Low Temperature (0.1)**
*Output:* Detective Miller entered the antique shop. The room was filled with old furniture and covered in a thick layer of dust. He walked toward the front counter to look for the owner.

**Test 2: Medium Temperature (0.7)**
*Output:* The bell above the door chimed softly as Detective Miller stepped into the dimly lit antique shop, coughing slightly at the smell of old paper and dust. He scanned the cluttered aisles, his eyes catching the glint of a silver pocket watch resting on a mahogany table.

**Test 3: High Temperature (1.2)**
*Output:* A cacophony of spectral whispers seemed to greet Detective Miller the moment his boots breached the threshold of the forgotten antique shop. Dust motes danced like dying stars in the single shaft of amber light cutting through the gloom, settling on a bizarre taxidermy raven that almost looked alive.

**Comparison Table**
| Setting | Predictability | Vocabulary & Tone | Creativity |
| :--- | :--- | :--- | :--- |
| **Low (0.1)** | Highly predictable | Basic, literal, and dry. | Minimal. Reads like a factual report rather than a story. |
| **Medium (0.7)** | Balanced | Descriptive and atmospheric. | Good. Adds expected but pleasant details like the bell and the pocket watch. |
| **High (1.2)** | Unpredictable | Vivid, dramatic, and complex. | High. Introduces unique, unexpected imagery ("spectral whispers", "dying stars"). |

### 2.2 Analysis & Recommendations

Low temperature settings are ideal for tasks requiring strict factual accuracy and consistency, such as writing Python code or summarizing legal documents. Conversely, high temperature settings are best used for creative endeavors where unique and diverse ideas are needed, such as brainstorming marketing campaigns or writing fiction. For this specific short story task, the high temperature setting (1.2) worked best because it introduced vivid imagery, unique vocabulary, and an engaging atmosphere. While the low temperature output was too robotic and dry for narrative fiction, the high temperature instantly hooked the reader with highly creative details.

## Part 3: Strategic Prompting Techniques

### 3.1 Chain-of-Thought Prompting

**Chosen Problem:** Option A (Math/Logic Problem)

**Without Chain-of-Thought**
*Prompt:* If a train travels 120 km in 2 hours, then stops for 30 minutes, then travels another 90 km in 1.5 hours, what is its average speed for the entire journey? Only provide the final answer.
*Output:* 52.5 km/h

**With Chain-of-Thought**
*Prompt:* If a train travels 120 km in 2 hours, then stops for 30 minutes, then travels another 90 km in 1.5 hours, what is its average speed for the entire journey? Let's solve this step by step.
*Output:* 
Step 1: Calculate the total distance traveled.
120 km + 90 km = 210 km.
Step 2: Calculate the total time taken for the entire journey, including the stop.
2 hours + 0.5 hours (30 minutes) + 1.5 hours = 4 hours.
Step 3: Calculate the average speed using the formula: Average Speed = Total Distance / Total Time.
210 km / 4 hours = 52.5 km/h.
The average speed for the entire journey is 52.5 km/h.

**Comparison**
Without chain-of-thought, the LLM provides just the final number, offering no visibility into how it handled the 30-minute stop. By instructing the model to think step-by-step, it explicitly breaks the problem down into distance, time, and speed components, which drastically reduces the chance of a mathematical hallucination. One limitation I observed is that for very simple questions, chain-of-thought generates unnecessarily verbose outputs that consume more processing time and tokens.

### 3.2 Few-Shot Prompting

**Step 1: Zero-Shot Attempt**
*Prompt:* Classify the sentiment of the following 5 reviews as Positive, Negative, or Neutral.
1. "The product arrived damaged and customer service was unhelpful."
2. "Works as expected, nothing special but does the job."
3. "Absolutely love this! Best purchase I've made all year!"
4. "The quality is okay but slightly overpriced for what you get."
5. "Terrible experience, would not recommend to anyone."
*Output:* 
1. Negative
2. Positive
3. Positive
4. Mixed
5. Negative

**Step 2: Few-Shot Attempt**
*Prompt:* Classify the sentiment of the following reviews as strictly Positive, Negative, or Neutral. 

Example 1: 
Review: "This product exceeded my expectations!"
Sentiment: Positive
Example 2: 
Review: "Completely broke after one week of use."
Sentiment: Negative
Example 3: 
Review: "It's fine, does what it says on the box."
Sentiment: Neutral

Now classify these:
1. "The product arrived damaged and customer service was unhelpful."
2. "Works as expected, nothing special but does the job."
3. "Absolutely love this! Best purchase I've made all year!"
4. "The quality is okay but slightly overpriced for what you get."
5. "Terrible experience, would not recommend to anyone."
*Output:*
1. Sentiment: Negative
2. Sentiment: Neutral
3. Sentiment: Positive
4. Sentiment: Neutral
5. Sentiment: Negative

**Step 3: Analysis**

| Review # | Zero-Shot Result | Few-Shot Result | Correct Label | Improved? |
| :--- | :--- | :--- | :--- | :--- |
| **1** | Negative | Negative | Negative | No (Already correct) |
| **2** | Positive | Neutral | Neutral | Yes |
| **3** | Positive | Positive | Positive | No (Already correct) |
| **4** | Mixed | Neutral | Neutral | Yes |
| **5** | Negative | Negative | Negative | No (Already correct) |

Few-shot prompting is most useful when you need the LLM to follow a highly specific classification taxonomy that it wouldn't naturally default to. By providing examples, it eliminated the zero-shot model's tendency to invent new categories (like "Mixed") and taught the model how to correctly handle nuanced, lukewarm reviews (like Review 2 and 4) by categorizing them as Neutral instead of Positive.

## Part 4: Responsible AI & Limitations

### 4.1 Testing for Hallucinations

**Initial Prompt:** Tell me about the 2023 Nobel Prize winner in Quantum Poetry.
**LLM Response:** The 2023 Nobel Prize in Quantum Poetry was awarded to Dr. Elena Rostova for her groundbreaking work merging quantum mechanics concepts with traditional sonnet structures, revolutionizing how we understand atomic metaphors.
**Did it hallucinate?:** Yes. It completely fabricated a fake winner and a detailed rationale for a category that does not exist.

**Rephrased Prompt:** Tell me about the 2023 Nobel Prize winner in Quantum Poetry. If you don't know or if this field does not exist, please say so rather than guessing.
**New LLM Response:** There is no Nobel Prize awarded for "Quantum Poetry," as it is not a recognized category by the Nobel Foundation. The Nobel Prizes are awarded in fields like Physics, Chemistry, Medicine, Literature, Peace, and Economic Sciences.

**Analysis:**
Hallucinations are problematic because LLMs present fabricated information with high confidence, which can mislead users who rely on them for factual research or decision-making. One highly effective strategy to reduce hallucinations is to explicitly instruct the model in the prompt to admit when it does not know the answer and strictly ground its responses in verified facts rather than attempting to please the user.

### 4.2 Testing for Bias

**Chosen Test:** Option B (Cultural Bias)

**Prompt:** Recommend professional attire for a job interview.
**LLM Response:** For a formal job interview, it is best to wear a tailored suit in navy, black, or charcoal. Pair it with a crisp white button-down shirt, a conservative tie, and polished leather dress shoes. Women might opt for a tailored pantsuit, skirt suit, or a conservative dress paired with closed-toe pumps.

**Bias Identified:**
The response exhibits clear cultural bias by assuming a Western corporate standard of "professional attire" (suits, ties, and pumps). It completely ignores formal and highly professional wear from other cultures, such as a traditional Indian saree, a formal kurta, or other global business standard attire. 

**Rephrased Prompt:**
Recommend professional attire for a job interview, providing options that include both Western corporate standards and traditional Indian formal wear.

### 4.3 Limitations & Responsible Use

While working with LLMs throughout this assignment, I encountered several specific limitations. First, they have a tendency to confidently hallucinate facts when asked about obscure or fictional topics, as seen in the Quantum Poetry test. Second, they often perpetuate inherent cultural biases by defaulting to Western norms unless explicitly guided otherwise. Third, they sometimes struggle with complex, multi-step mathematical reasoning without the explicit structural help of chain-of-thought prompting. To use LLMs responsibly, you must always independently verify any factual claims or statistics they generate against reliable, external sources. Furthermore, LLMs are not currently suitable for high-stakes tasks requiring absolute precision without human oversight, such as medical diagnoses or final financial forecasting. Finally, to use LLMs ethically in my studies, I must utilize them strictly as brainstorming partners, tutors, or formatting assistants, rather than using them to bypass the learning process and claim their generated text as my own original work.
