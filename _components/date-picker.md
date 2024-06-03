---
title: Date Picker
layout: components
version: 1.0.0
figma: https://www.figma.com/design/P2gZJjVaAqHJwB1tGbwtjw/RAADS?node-id=5178-8295&t=DaQuC2pMFYEZZcOO-1
---

The date picker is great!


## Structure

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FpC6ZhE3ixUPT7MbTPPaVc0%2FRAADS-visual-examples%3Fnode-id%3D1-65%26t%3DFprFJtU0BJbww0zq-1%26scaling%3Dmin-zoom%26page-id%3D0%253A1&hide-ui=1" allowfullscreen></iframe>

1. **Default (inline):** Fields are aligned 'inline'.
1. **Mobile (stacked):** Fields are stacked.
1. **Text fields:** Text fields and labels inherit from [form inputs]({{site.baseurl}}/components/form-inputs).
1. **Calendar dropdown button:** Will display a calendar picker dropdown.

## Validation

It has specs. They are good.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FpC6ZhE3ixUPT7MbTPPaVc0%2FRAADS-visual-examples%3Fnode-id%3D44-1178%26t%3DylD63g8qa222Va07-1%26scaling%3Dmin-zoom%26page-id%3D0%253A1&hide-ui=1" allowfullscreen></iframe>

1. **Error styles:** Date picker text field validation styles inherit from [form inputs]({{site.baseurl}}/components/form-inputs).
1. **Error message:** Single error message for date picker form component.
3. **Button error state:** Date picker calendar button styles inherit from [buttons]({{site.baseurl}}/components/buttons)

## Behaviour

1. The error must not be shown when the user is tabbing between the day, month and year inputs.
1. Only when the user moves focus away from all three inputs can the validation be triggered. 

## Accessibility

1. The user must always be in control. DO not hijack the cursor.
