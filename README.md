# Interview Pair Timer

A small offline timer for a 15-minute paired English interview rehearsal. It gives each person a speaking turn, a follow-up question, specific feedback, and a short retry.

This is a functional companion to the existing [peer-session handbook](https://szj2ys.github.io/peer-interview-session-plans/). The handbook describes several facilitation formats; this tool supplies the missing turn timer. It is not another copy of those guides.

## Use it

Open `index.html` in a browser. No build step, server, account, microphone, or network connection is needed. The first download of the folder is the only prerequisite for offline use.

- Start or pause the current step.
- Move to the next step whenever both participants are ready.
- The timer pauses at every boundary, including when the tab has been in the background.
- Reset keeps the current notes. Reloading or closing the page clears them.
- Print the notes or use the included one-page worksheet.

The eight steps total 15 active minutes; pauses and transitions are additional. Use more thinking time where appropriate. Notes are held only in the page's memory. There is no analytics, storage, external script, recording, or upload.

## Content and limits

The examples are prompts for truthful personal experiences, not sample claims to copy. This is practice guidance, not a hiring assessment or prediction. MakeInterview publishes a [free English interview guide](https://makeinterview.com/en/blog/job-interview-in-english) with more question pairs. The timer works independently of its AI interview service.

## Development

Edit `index.html` directly. The clock uses a monotonic deadline so an inactive tab does not extend the active step. Each completed step waits for the participant to continue. All controls use native buttons, focus styles, and a polite status announcement; the changing clock is not announced every second.

Code is MIT licensed. The worksheet may be copied and adapted for teaching with credit to MakeInterview.
