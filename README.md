# MCQ Video Maker

Create quiz videos from multiple-choice questions, with voice, a countdown, an answer reveal and a score screen. It runs in the browser from a single HTML file. There is nothing to install.

## Features

- Load questions from a JSON file, or paste the JSON into the page.
- Built-in prompt for Gemini that writes the questions for you.
- One video segment per question: options appear, a countdown runs, then the correct answer is revealed.
- Final screen that asks viewers to write their score in the comments.
- Optional voice that reads each question and answer, using Gemini text-to-speech.
- Countdown ticks and an answer chime, recorded into the video.
- Seven themes: Midnight, Emerald, Ocean, Sunset, Rose, Graphite and Daylight.
- A font choice for the question, the options, the letters and numbers, and the watermark.
- Watermark with your page name and logo, placed at the top or bottom.
- Four video sizes: 16:9, 9:16, 4:5 and 1:1.
- Export as one video, or as one file per question, in MP4 or WebM.
- Light and dark app appearance.

## How to use

1. Open the **Questions** tab. Enter a topic, then press **Copy prompt**.
2. Paste the prompt into Gemini. Save its reply as a `.json` file.
3. Upload the file, or paste the JSON, then press **Load questions**.
4. Choose a size in the **Video** tab, and a look in the **Theme** tab.
5. Press **Preview with sound** to check the video.
6. Press **Export video**. Keep the page open and in front until the download finishes.

## Question format

```json
{
  "title": "Quiz title",
  "questions": [
    {
      "question": "Which planet is known as the Red Planet?",
      "options": ["Venus", "Mars", "Jupiter", "Mercury"],
      "answer": "B"
    }
  ]
}
```

Each question needs 2 to 5 options. The `answer` is the letter of the correct option, from A to E.

## Voice

Voice is optional. To use it:

1. Get a Gemini API key from [aistudio.google.com](https://aistudio.google.com).
2. Paste it in the **Voice** tab and choose a voice.
3. Turn on **Voice reads each question, then the answer**.

With voice off, the countdown starts shortly after the options appear. You can change the pause in the **Video** tab.

## Privacy

- Everything runs in your browser. Your questions, logo and videos are not uploaded to any server.
- Your Gemini API key is saved in your browser only. It is sent to Google and nowhere else.
- Settings such as theme, fonts and watermark are saved in your browser's local storage.
- Voice, fonts and the Gemini prompt need an internet connection.

## Browser notes

- MP4 export works only in browsers that support it. Otherwise the app saves WebM. Use a converter such as HandBrake or VLC if a platform needs MP4.
- On iPhone, use Safari and keep the screen on and the page in front while exporting.
- A recent version of Chrome, Edge or Safari is recommended.

## Run it

Open `index.html` in a browser, or host it on GitHub Pages:

1. Go to **Settings**, then **Pages**.
2. Set **Source** to **Deploy from a branch**, then choose `main` and `/ (root)`.
3. Open the link GitHub shows you.

## License

© 2026 Your Name. All rights reserved.
