# SmartScribe Coding Challenge

Welcome to the SmartScribe coding challenge! This challenge is designed to assess your problem-solving skills, familiarity with Python, and ability to document your thought process.

## Problem Statement

Our system receives audio data in 120-second chunks. This audio data is sent to a transcription service, which returns a JSON response. The JSON contains a field called `utterances` that is a list of objects. Each object has:

- `text`: The transcription of what was said by that person.
- `speaker`: A label ("A" or "B") indicating which person was talking.

The challenge is that between the 120-second chunks, there is no guarantee that "A" and "B" labels are stable. "A" is the first person that talks during that time window and "B" is the second. This can switch between 120-second windows, depending on where the conversation is. We need to determine which of the speakers in each chunk is the provider and which is the patient.

## Your Task

1. **Clone this repository** and write some basic Python code in a Jupyter notebook.
2. **Document your thought process** on how you approach the problem.

### Instructions

1. **Clone the Repository**

   ```sh
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Open the Jupyter Notebook**
   Open the provided Jupyter notebook template `solution.ipynb` and follow the instructions inside.

3. **Understand the Data**
   The provided `data.json` file contains sample data returned from the transcription API. You can load this data to understand its structure and contents.

4. **Propose a Solution**

   - Outline your approach to solving the problem.
   - Use any standard libraries, tools, models, or outside services as you see fit.
   - You don't need to write actual working code; just mock things up and write pseudocode.

5. **Submit Your Solution**

   - Once you're done, save the notebook with your changes.
   - Push your changes to a new branch and create a pull request.
   - In your pull request, explain your approach and any assumptions you made.

### Solution Approach

In your Jupyter notebook, you should:

1. **Load the data**: Use Python to load and inspect the `data.json` file.
2. **Analyze the Problem**: Discuss potential challenges and assumptions.
3. **Propose a Solution**:
   - Outline steps to determine which speaker is the provider and which is the patient.
   - Use pseudocode to describe your approach.
   - Suggest any models, algorithms, or outside apis, libraries, or tools that could help.
   - Explain how you might want to handle edge cases and ensure accuracy.

### Tools and Libraries

Feel free to suggest any tools, models, or services that could help solve the problem. Some examples include:

- Loading a pretrained NVIDIA speech detection model and running it on the audio? Fine.
- Using a low-cost LLM via API to classify something? Also fine.
- Using a scikit-learn model to classify something based on vocabulary? Great.

The sky's the limit—just explain what approach you would take and why.

We look forward to seeing your solution and understanding your thought process. Good luck!
