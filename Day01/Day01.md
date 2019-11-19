# Day 01

### TransitionEvent
It's a interface represents events providing information related to transitions. 
```console
TransitionEvent {isTrusted: true, propertyName: "box-shadow", elapsedTime: 0.07, pseudoElement: "", type: "transitionend", …}
bubbles: true
cancelBubble: false
cancelable: true
////////OMIT//////////
srcElement: div.key
target: div.key
timeStamp: 1335872.2199999902
type: "transitionend"
__proto__: TransitionEvent
```

### transitionend event
It is fired when a CSS transition has completed
```js
// When you want to remove CSS style after it's fired
key.addEventListener('transitionend', removeTransition)

function removeTransition(e) {
      // e is TransitionEvent interface
      if(e.type === 'transitionend') {
        this.classList.remove('playing');
      }
    }
```

### HTMLMediaElement.currentTime
The HTMLMediaElement interface's currentTime property specifies the current playback time in seconds.
```js
audio.currentTime = 0; // rewind to the start 
audio.play();
```

### Complex Document.querySelector()
```HTML
<div class="user-panel main">
  <input name="login"/>
</div>

<script>
  let el = document.querySelector("div.user-panel.main input[name='login']");
</script>
```

```js
const audio = document.querySelector(`audio[data-key="${e.keyCode}"]`);
const key = document.querySelector(`div[data-key="${e.keyCode}"]`);
```

### KeyboardEvent.code
The KeyboardEvent.code property represents a physical key on the keyboard

!> In ther drum kit we used `keyCode` but it's not recommended now 
<br>
key 'a' KeyboardEvent 
```console
code: "KeyA"
key: "a"
keyCode: 65
```

### What I've made from this challenge
Sponge bob drum kit<br>
![alt text](https://user-images.githubusercontent.com/47588349/69106458-bf1c1800-0ab1-11ea-803d-e82ee7c647ac.png)
