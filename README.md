# Stimulus Calendar
## Date and time input stimulus controller 

> ⚠️ Package under development don't use yet. ⚠️

### Installation

`yarn add stimulus-clock`
`npm install stimulus-clock`


### Usage

```js
// bootstrap.js
import { Application } from '@hotwired/stimulus'
import Calendar from 'stimulus-calendar'

const app = Application.start()
app.register('calendar', Calendar)
```

```html
<div data-controller="calendar" data-calendar-is-disabled-value="false">
    <input type="datetime" data-calendar-target="dateInput" value="{{ post.date|format_datetime() }}"/>
</div>
```


### Config

`data-calendar-is-disabled-value="true"` - disables the input to select a year, month, day, hour and minute.
