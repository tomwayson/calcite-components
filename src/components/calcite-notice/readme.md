# calcite-notice

You can programmatically focus the close button of a `dismissible` `calcite-notice` with the `setFocus()` method:

`<div onclick=document.querySelector('#my-notice').setFocus()>Focus!</div>`

<!-- Auto Generated Below -->


## Properties

| Property      | Attribute     | Description                                              | Type                                     | Default     |
| ------------- | ------------- | -------------------------------------------------------- | ---------------------------------------- | ----------- |
| `active`      | `active`      | Is the notice currently active or not                    | `boolean`                                | `false`     |
| `color`       | `color`       | Color for the notice (will apply to top border and icon) | `"blue" \| "green" \| "red" \| "yellow"` | `"blue"`    |
| `dismissible` | `dismissible` | Select theme (light or dark)                             | `boolean`                                | `false`     |
| `icon`        | `icon`        | If false, no icon will be shown in the notice            | `boolean`                                | `false`     |
| `scale`       | `scale`       | specify the scale of the notice, defaults to m           | `"l" \| "m" \| "s"`                      | `"m"`       |
| `theme`       | `theme`       | Select theme (light or dark)                             | `"dark" \| "light"`                      | `undefined` |
| `width`       | `width`       | specify the width of the notice, defaults to m           | `"auto" \| "full" \| "half"`             | `"auto"`    |


## Events

| Event                | Description                    | Type               |
| -------------------- | ------------------------------ | ------------------ |
| `calciteNoticeClose` | Fired when an notice is closed | `CustomEvent<any>` |
| `calciteNoticeOpen`  | Fired when an Notice is opened | `CustomEvent<any>` |


## Methods

### `close() => Promise<void>`

close the notice emit the `calciteNoticeClose` event - <calcite-notice> listens for this

#### Returns

Type: `Promise<void>`



### `open() => Promise<void>`

open the notice and emit the `calciteNoticeOpen` event - <calcite-notice> listens for this

#### Returns

Type: `Promise<void>`



### `setFocus() => Promise<void>`

focus the close button, if present and requested

#### Returns

Type: `Promise<void>`




## Slots

| Slot               | Description                                                                   |
| ------------------ | ----------------------------------------------------------------------------- |
| `"notice-link"`    | Optional action to take from the notice (undo, try again, link to page, etc.) |
| `"notice-message"` | Main text of the notice                                                       |
| `"notice-title"`   | Title of the notice (optional)                                                |


## Dependencies

### Depends on

- [calcite-icon](../calcite-icon)

### Graph
```mermaid
graph TD;
  calcite-notice --> calcite-icon
  style calcite-notice fill:#f9f,stroke:#333,stroke-width:4px
```

----------------------------------------------

*Built with [StencilJS](https://stenciljs.com/)*
