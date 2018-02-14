# react-bubble-chart-d3
ReactJS component to display data as a bubble chart using d3.

### General Usage

As you will be able to see in [test](test/src/App.js) in order to use the component we need to importe it as:
```JAVASCRIPT
import BubbleChart from '@weknow/react-bubble-chart-d3';
```

Then, in the render method we can just call it like:

```JAVASCRIPT
<BubbleChart
  width={1000}
  height={800}
  font={{
        family: 'Arial',
        size: 12,
        color: '#000',
        weight: 'bold',
      }}
  data={[
    { label: 'CRM', value: 1 },
    { label: 'API', value: 1 },
    { label: 'Data', value: 1 },
    { label: 'Commerce', value: 1 },
    { label: 'AI', value: 3 },
    { label: 'Management', value: 5 },
    { label: 'Testing', value: 6 },
    { label: 'Mobile', value: 9 },
    { label: 'Conversion', value: 9 },
    { label: 'Misc', value: 21 },
    { label: 'Databases', value: 22 },
    { label: 'DevOps', value: 22 },
    { label: 'Javascript', value: 23 },
    { label: 'Languages / Frameworks', value: 25 },
    { label: 'Front End', value: 26 },
    { label: 'Content', value: 26 },
  ]}
/>
```

The **data** prop receive and array of objects:
```javascript
{
  label: 'label', // Text to display.
  value: 1, // Numeric Value.
  /**
    Color of the circle this value it's optional,
    accept hex (#ff0000) and string (red) name values.
    If you don't provide a value the default behavior
    is assign a color based on a d3.schemeCategory20c
    color schema.
  */
  color: '#ff00ff',
}
```

The **font** prop receive a configuration object to set the font-family, font-size, font-weight and color of the text:
```javascript
// If you don't set this prop the default configuration will be this object.
{
  family: 'Arial',
  size: 12,
  color: '#000',
  weight: 'bold',
}
```

### Installation

Install this component is easy, just use npm as:
```BASH
npm install @weknow/react-bubble-chart-d3
```
