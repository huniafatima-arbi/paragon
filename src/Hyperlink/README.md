---
title: 'Hyperlink'
type: 'component'
components:
- Hyperlink
categories:
- Buttonlike
status: 'Needs Work'
designStatus: 'Done'
devStatus: 'To Do'
notes: |
  Improve prop naming. Deprecate content prop.
  Use React.forwardRef for ref forwarding.
---

### minimal usage

```jsx live
<Hyperlink href="https://en.wikipedia.org/wiki/Hyperlink">edX.org</Hyperlink>
```

### with blank target

```jsx live
<Hyperlink destination="https://www.edx.org" target="_blank" rel="noopener noreferrer">
  edX.org
</Hyperlink>
```

### with onClick

```jsx live
<Hyperlink
  destination="https://www.edx.org"
  target="_blank"
  onClick={e => {
    e.preventDefault();
    console.log('click');
  }}
>
  edX.org
</Hyperlink>
```

### with icon

```jsx live
<Hyperlink destination="https://www.edx.org">
  <Icon
    id="SampleIcon"
    className="fa fa-book"
    screenReaderText="Visit edX Home"
  />
</Hyperlink>
```