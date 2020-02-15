## MODAL WEB COMPONENT

`<mo-dal></mo-dal>`

#### Example

```html
<mo-dal>
  <h1 slot="title">Please Confirm</h1>
  <p>Are you sure you want to go there</p>
</mo-dal>
```

---

> To open the modal from javascript

```js
const modal = document.querySelector('mo-dal')
modal.open()
// OR
modal.setAttribute('opened', '')
```

> To hide the modal from javascript

```js
const modal = document.querySelector('mo-dal')
modal.hide()
// OR
modal.removeAttribute('opened')
```

> To check if modal is opened

```js
const modal = document.querySelector('mo-dal')
console.log(modal.isOpen) // true or false
```

---

**_Events_**

- Confirm Event

```js
const modal = document.querySelector('mo-dal')
modal.addEventListener('confirm', () => {
  console.log('Confirmed')
})
```

- Cancel Event

```js
const modal = document.querySelector('mo-dal')
modal.addEventListener('cancel', () => {
  console.log('Cancelled')
})
```

---
