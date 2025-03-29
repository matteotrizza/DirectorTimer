DirectorTimer is a small tool entirely **developed using Artificial Intelligence** (ChatGPT with gpt4 model), made for **content creators** and **streamers** who don't have a direction helping their content production and want an **automated system** to deal with timings.

We all know a too long or too short video may not get the success it deserves, so why not directly deleting the problem with DirectorTimer? You create a small _.txt_ file containing the sections (or chapters) you want your content to be divided into, and how much time you'd like any section to take, and you'll be helped with a big timer reminding you how much time you still have to cover a specific section of your video. Then, to go to the next section, click the dedicated button in the small and comfortable interface or use an API call via your **StreamDeck**.

# General information
DirectorTimer is entirely based on Python 3, with a series of external libraries to manage files, timers and automations.

You can find the application (_.exe_) and the code (_.py_) in the **RELEASE SECTION**.

# Tutorial
1. Launch the executable or the Python file via Command Prompt;
2. Click "Open" in the upper part of the window and select a **COMPATIBLE** text file (see specific requirements below);
3. When you're ready, click the green "Start" button

![image](https://github.com/user-attachments/assets/97ff894a-8fb1-48ee-bf1c-ae686caeea27)

4. The timer will start running;
5. If you're "late", timer will get red in order to catch your attention;

![image](https://github.com/user-attachments/assets/f140102d-3e40-4524-b075-cdc5153095b6)

6. When you're ready for the next chapter of your video/live stream, click the yellow "Next" button and the timer value will be updated with the result of the sum of the next chapter's dedicated time and the actual time remaining (to simplify...if you're late you'll see less time than the expected);
7. When you finish your recording/streaming, click the "Reset" button to return to the first chapter or close the app.

# Text file requirements
In order to split your content into multiple chapters and make them understandable for DirectorTimer, your text file (_.txt_), has to be formatted like this:
```
chapter1
0.1
---
chapter2
2
---
chapter3
1
---
```
The first row is dedicated to the title of the section and the second one to its duration written in decimal (ex. 1 minute = 1, 30 seconds = 0.5).

# StreamDeck Integration
In order to manage DirectorTimer's sections without moving your mouse, which is definitely unconvenient while recording or streaming, I developed a system of "API Calls" on a local server. Send a GET request in background to port 5000 when you want to start your timer or to go to the next section.

![image](https://github.com/user-attachments/assets/f0054c4d-9a59-4f1f-b554-5bec7c028055)


![image](https://github.com/user-attachments/assets/e0239f09-9f75-439c-a927-13f31742d23b)
