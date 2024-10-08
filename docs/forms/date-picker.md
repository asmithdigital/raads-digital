---
title: Date Picker
layout: components
version: 1.0.0
figma: https://www.figma.com/design/P2gZJjVaAqHJwB1tGbwtjw/RAADS?node-id=5178-8295&t=DaQuC2pMFYEZZcOO-1
intro: The date picker is really great!
promo-image: date-1.png
parent: Forms
---

## Structure

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="494" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FpC6ZhE3ixUPT7MbTPPaVc0%2FRAADS-visual-examples%3Fnode-id%3D1-65%26t%3DFprFJtU0BJbww0zq-1%26scaling%3Dmin-zoom%26page-id%3D0%253A1&hide-ui=1" allowfullscreen></iframe>

1. **Fieldset legend:** Legend for fieldset group `<legend>` See [form inputs]({{site.baseurl}}/docs/components/form-inputs)
1. **Form label and input:** Label for each form input `<label for>`See [form inputs]({{site.baseurl}}/docs/components/form-inputs)
1. **Calendar button:** See [buttons]({{site.baseurl}}/docs/components/buttons).
1. **Horizontal spacing:** `2 XS` See [spacing]({{site.baseurl}}/docs/foundations/spacing)
1. **Vertical spacing:** `3 SM` See [spacing]({{site.baseurl}}/docs/foundations/spacing)
1. **Calendar picker dropdown:** TBD.


## Validation

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="429" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FpC6ZhE3ixUPT7MbTPPaVc0%2FRAADS-visual-examples%3Fnode-id%3D44-1178%26t%3DylD63g8qa222Va07-1%26scaling%3Dmin-zoom%26page-id%3D0%253A1&hide-ui=1" allowfullscreen></iframe>

1. **Group label:** See [form inputs]({{site.baseurl}}/docs/components/form-inputs).
1. **Field label and input:** See [form inputs]({{site.baseurl}}/docs/components/form-inputs).
1. **Error message:** One error message positioned below form inputs. See [form inputs]({{site.baseurl}}/docs/components/form-inputs) and [behaviour](#behaviour).
1. **Stacked positioning:** Stacked layout error message sits below form inputs.

## Behaviour

1. The error must not be shown when the user is tabbing between the day, month and year inputs.
1. Only trigger validation when the user moves focus away from all three inputs. Consider using `FocusEvent.relatedTarget`./ (see [MDN web docs FocusEvent.relatedTarget](https://developer.mozilla.org/en-US/docs/Web/API/FocusEvent/relatedTarget)).

## Stacked
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="100%" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Fproto%2FpC6ZhE3ixUPT7MbTPPaVc0%2FRAADS-visual-examples%3Fnode-id%3D375-234%26t%3Dsyk5biH86e4TRIbx-1%26scaling%3Dmin-zoom%26page-id%3D0%253A1&hide-ui=1" allowfullscreen></iframe>

1. **Default state:** Stacked layout for screen resolution `@media screen and (max-width: 258px)` only
1. **Error state:** Error message sits below the component


## Accessibility

1. Do not hijack the cursor by automatically moving the cursor to the next input. The user must always be in control.
2. Validation message must specify which field is in error state (eg 'Please enter a valid day and year'), and must not rely on colour alone to indicate error state.
1. All form input validation for date picker inherit from [form inputs]({{site.baseurl}}/docs/components/form-inputs). 
