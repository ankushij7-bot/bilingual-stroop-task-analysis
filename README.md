# bilingual-stroop-task-analysis
language and reaction time based Stroop task experiment and analysis
# Bilingual Stroop Task Experiment

## Aim
To investigate cognitive interference in a bilingual context using a Stroop task.

## Method
Participants responded to the ink color of words presented in two languages under:
- Congruent condition
- Incongruent condition

## Data Processing
- Removed incorrect responses
- Filtered extreme reaction times (<200 ms, >3000 ms)

## Analysis
Reaction time data was analyzed using Python to compare performance across conditions.

## Result
Incongruent trials showed slower reaction times, demonstrating interference effects. Differences across languages suggest variation in automaticity of processing.

## Interpretation
Findings are consistent with the Stroop effect and highlight how language processing influences attentional control.

## Tools
PsychoPy, Python (pandas, matplotlib)
Bilingual Stroop Task (Replication Guide)

This project is a simple PsychoPy-based implementation of a bilingual Stroop task using both text (English) and image-based (Hindi) stimuli. The goal is to measure reaction time while participants respond to colour information under interference.

## What you need
PsychoPy installed
Python (if running outside PsychoPy)
A folder containing colour images (for the Hindi trials)

## About the colour image folder

The Hindi trials use a folder of images instead of text. Each image should represent a colour, and the naming is important.

The code reads the first letter of the file name as the correct response key. So make sure your images are named in a way that matches the key you expect participants to press.

## How the task works
When you run the script, participants first see instructions asking them to respond to the colour, not the word.
In the English trials, colour words are shown on the screen in different ink colours. The participant has to press the key corresponding to the ink colour.
After a short break, the Hindi trials begin. Here, instead of words, images are shown from the folder. The participant again responds using the keyboard.
Reaction times are recorded for all trials.

## Data storage

The data is automatically saved in an Excel file. Each row contains:

Participant serial number
Time of experiment
Reaction times for all trials

If you’re not seeing the file, check that your file path is correct in the script.

## Notes
The trials are randomized, so each run will look slightly different.
Make sure your image folder path is correct, otherwise the Hindi trials won’t run.
Keep the naming consistent, otherwise responses won’t be recorded properly.

This was built as part of a psychology experiment setup, so it’s fairly simple but does the job for collecting reaction time data.
