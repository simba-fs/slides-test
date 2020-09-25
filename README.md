# Speech Recognition
[slides](https://hackmd.io/@simba-fs/speechRecognition)
[code](https://github.com/simba-fs/recognition)

---

# Take a Look
[Recognition](https://simba-fs.github.io/recognition)

---

# Speech Recognition API
[MDN](https://developer.mozilla.org/zh-TW/docs/Web/API/SpeechRecognition)

----

## Browser Support
Only Google Chrome

----

## Example
```javascript=
const SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
const recognition = new SpeechRecognition();

recognition.onresult = (event) => {
    console.log(event.results[0][0].transcript);
};

recognition.start();
```

---

# TTS API
Text To Sound
[MDN](https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesisUtterance)

----

## Browser Support
Except IE and Opera, all browser support this api

----

## example
```javascript=
const speech = new SpeechSynthesisUtterance();
speech.text = 'Hello world';
speech.volume = 1;
speech.rate = 1;
speech.pitch = 1;
speech.lang = 'en-US';

window.speechSynthesis.speak(speech);
```

---

# http-server

----

# Install node
Install node
[nodejs](https://nodejs.org/en/)

----

# Install http-server
[http-server](https://www.npmjs.com/package/http-server)
`npm i http-server -g`

---

# Let's make a voice assistent!
