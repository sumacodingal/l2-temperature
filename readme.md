# 🤖 L2: Advanced Prompt Engineering - Temperature & Instruction-Based Prompts

An interactive activity to explore how temperature settings and instruction-based prompts affect AI responses using Google Gemini API.

## 🎯 Learning Objectives

By completing this activity, you will:
- Understand how temperature controls AI creativity and randomness
- Learn to write effective instruction-based prompts
- Practice hands-on with the Google Gemini API
- Experiment with different prompt engineering techniques

## 📋 What You'll Do

### Part 1: Temperature Exploration
Compare AI responses at different temperature settings:
- **Low Temperature (0.1)**: Focused, deterministic responses
- **Medium Temperature (0.5)**: Balanced creativity and accuracy
- **High Temperature (0.9)**: Creative, varied outputs

### Part 2: Instruction-Based Prompts
Learn how specific instructions guide AI to produce:
- Summaries
- Simplified explanations
- Pro/Con lists
- Creative content

### Part 3: Create Your Own
Experiment with custom prompts and temperature combinations!

## 🚀 Setup Instructions

### Step 1: Get Your Google Gemini API Key

1. Visit: **https://makersuite.google.com/app/apikey**
2. Sign in with your Google account
3. Click **"Create API Key"** or **"Get API Key"**
4. Copy the entire key (it looks like: `AIzaSy...`)

### Step 2: Configure Your API Key

1. Find the file `config_template.py` in this project folder
2. **Rename it to:** `config.py`
3. Open `config.py` in any text editor (Notepad, VS Code, etc.)
4. Replace `YOUR_API_KEY_HERE` with your actual API key
5. Save the file

**Example:**
```python
# Before:
GEMINI_API_KEY = "YOUR_API_KEY_HERE"

# After:
GEMINI_API_KEY = "AIzaSyD1234567890abcdefghijklmnop"  # Your actual key
```

### Step 3: Install Required Library

Open Terminal/Command Prompt in this project folder and run:

```bash
pip install google-genai
```

### Step 4: Run the Activity

```bash
python prompt_lab.py
```

Follow the on-screen prompts and explore!

## 🎓 Activity Structure

The activity has three main parts:

1. **Temperature Exploration** - See how the same prompt produces different outputs
2. **Instruction-Based Prompts** - Experiment with 4 pre-designed prompts
3. **Custom Prompts** - Create and test your own prompts

**Bonus:** Optional streaming response demonstration

## ⚠️ Important Security Notes

- **NEVER share your API key** with anyone
- **NEVER upload `config.py`** to GitHub or public spaces
- **Keep your key private** like a password
- If your key is accidentally exposed, generate a new one immediately at: https://makersuite.google.com/app/apikey

## 🐛 Troubleshooting

### Error: "No module named 'config'"
**Solution:** Make sure you renamed `config_template.py` to `config.py`

### Error: "No module named 'google.genai'"
**Solution:** Run `pip install google-genai`

### Error: "Invalid API key" or Authentication error
**Solution:** 
- Check that you copied the entire key correctly (no extra spaces)
- Verify your API key is active at https://makersuite.google.com/app/apikey
- Make sure you replaced `YOUR_API_KEY_HERE` with your actual key

### Error: Rate limit exceeded
**Solution:** Wait a moment between requests (the code includes delays, but if you run it multiple times quickly, you might hit limits)

### Program crashes or unexpected errors
**Solution:** 
- Make sure you're using Python 3.7 or higher: `python --version`
- Try reinstalling the library: `pip install --upgrade goog