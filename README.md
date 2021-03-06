# react-sortable-dnd

A React component to sort elements of any type. It also supports dropping external elements in any position.

> [Demo](http://educastellano.github.io/react-sortable-dnd)

## Install

```
npm i react-sortable-dnd --save 
```

## Usage

```html
<Sortable onSort={components => console.log(components)}>
    <div>Apple</div>
    <div>Mango</div>
    <div>Pineapple</div>
</Sortable>
```

## Props

Prop                | Type/Options              | Default             | Description
---                 | ---                       | ---                 | ---
`className`         | *string*                  | `Sortable`          | **`Optional`** The class name of the component
`classPlaceholder`  | *string*                  | `Placeholder`       | **`Optional`** The class name of the placeholder component when dragging external elements.
`enabled`           | *boolean*                 | `true`              | **`Optional`** Enable/disable the sorting 
`type`              | *string*                  | ``                  | **`Optional`** Type of the elements to sort, in case you want to restrict elements of other Sortable lists.

## Event Props

Prop                | Parameters                | Description
---                 | ---                       | ---
`onSort`            | *(components)*            | The sorting callback function.
`onSortStart`       | *(components)*            | Triggered when an element starts being dragged.
`onDrop`            | *(e, data, index)*        | **`Optional`** Called when an external element is dropped.


## Changelog

* 1.0.0 
    * Initial release :tada:

## License

[ISC License](http://opensource.org/licenses/ISC)
