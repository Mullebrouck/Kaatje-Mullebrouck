# HTML Input Types

###Input Types

[](codepen://Kaatje/GoQQov)

**Search Input**

```html
<input type="search" />
```

**Email Input**

```html
<input type="email" />
```

**URL Input**

```html
<input type="url" />
```

**Date Input**

```html
<input type="date" />
```

**Tel Input**

```html
<input type="tel" />
```

**Number Input**

```html
<input type="number" />
```

**Range Input**

```html
<input type="range" />
```
You will get a slider with the range input. 

**Month/week Input**

```html
<input type="month" /> selecting a month 
<input type="week" /> selecting a giving week 
```


**Time, DateTime-local Input**

```html
<input type="time" /> 
<input type="datetime-local" /> selecting date and time
```

**Color Input**

```html
<input type="color" /> 

```


###Form Elements

**Datalist (Autocomplete suggestion)**

```html
<input type="text" list="browsers" />
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
  <option value="Internet Explorer">
  <option value="Opera">
  <option value="Safari">
</datalist>
```
Value of `<list>` and `<id>` need to be the same, so they will be linked together.

`<option value>` allows you to get autocomplete suggestions when you type: F...-> Firefox


###Form Attributes

**Placeholder Attribute**

```html
<input type="text" placeholder="PUT TEXT HERE" />
```

**Autofocus Attribute**

```html
<input type="text" autofocus />
```

**Require Attribute**

```html
<input type="text" required />
```

**Pattern Attribute**

```html
<input type="text" pattern="[0-9]{3}" /> Ex: we want pattern to be 3 0-9 digits
```
Get error until pattern matches. 