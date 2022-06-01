# Alexey Kuptsov
## My contacts:

__Phone:__ +7 7212 25 99 94

__Mobile-Phone:__ +7 778 141 50 31

__e-mail:__ [kuptsovalexey@mail.ru](mailto:kuptsovalexey@mail.ru)

## About Me
I've been coding sins school time, more than 15 years. I have no experience in programming large projects and I've never work in large companies. I learn and find solutions quickly.

## Skills:
* HTML/CSS/JS
* C/C++ for microcontrollers
* Java
* vb.net scripts for video production

## Code examples:
Little script for autostart and stor YouTube translation:
```javascript
let h = 17, m = 59;
let h2 = 19, m2 = 30;

let wostart = true;
let woend = false;
let hn, mn;


let timerId = setInterval(() => { 
	if (wostart){
		let now = new Date();
		if (now.getMinutes() != mn) {
			hn = now.getHours();
			mn = now.getMinutes();
			showTimeMsg = true;
			console.log("Ждем начала, время: "+now.getHours().toString()+":"+now.getMinutes().toString()+" начало в "+h.toString()+":"+m.toString());
		}
		if ((hn >= h) && (mn >= m)) {
			wostart = false;
			woend = true;
			console.log("ЗАПУСКАЮ СТРИМ!");
			document.getElementById('start-stream-button').click();
		}
	}

	if (woend){
		let now = new Date();
		if (now.getMinutes() != mn) {
			hn = now.getHours();
			mn = now.getMinutes();
			console.log("Ждем конца, время: "+now.getHours().toString()+":"+now.getMinutes().toString()+" конец в "+h2.toString()+":"+m2.toString());
		}
		if ((hn >= h2) && (mn >= m2)){
			woend = false;
			console.log("ОСТАНАВЛИВАЮ СТРИМ!");
			document.getElementById('end-stream-button').click();
			document.getElementsByClassName('style-scope ytcp-confirmation-dialog')[34].click();
		}
	}
}, 10000);
```

## Experience:
* University projects
* avr microcontroller programming for DMX-receiver (prolight devices)
* Arduino projects:
  * remote controller for main-light in concert hall
  * Art-Net controller for prolight devices
  * Controller for warm floor with GPRS
* Android App for camera operators (Tally Light)

## English
I'm learning English at InterPress. My current level is B1 (Pre-Intermediate).