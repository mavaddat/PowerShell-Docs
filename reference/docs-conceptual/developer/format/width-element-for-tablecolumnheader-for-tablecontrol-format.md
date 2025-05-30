---
description: Width Element for TableColumnHeader
ms.date: 08/25/2021
title: Width Element for TableColumnHeader
---
# Width Element for TableColumnHeader

Defines the width (in characters) of a column.

## Schema

- Configuration Element
- ViewDefinitions Element
- View Element
- TableControl Element
- TableHeaders Element
- TableColumnHeader
- Width Element

## Syntax

```xml
<Width>NumberOfCharacters</Width>
```

## Attributes and Elements

The following sections describe the attributes, child elements, and parent element of the `Width`
element used when defining column headers.

### Attributes

None.

### Child Elements

None.

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[TableColumnHeader Element for TableHeaders for TableControl](./tablecolumnheader-element-format.md)|Defines a label, width, and alignment of the data for a column of the table.|

## Text Value

When at all possible, specify a width (in characters) that is greater than the length of the
displayed property values.

## Remarks

For more information about the components of a table view, see [Creating a Table View](./creating-a-table-view.md).

## Example

The following example shows a `TableColumnHeader` element whose width is 16 characters.

```xml
<TableColumnHeader>
  <Label>Column 1</Label>
  <Width>16</Width>
  <Alignment>Left</Alignment>
</TableColumnHeader>
```

## See Also

[Creating a Table View](./creating-a-table-view.md)

[TableColumnHeader Element for TableHeader for TableControl](./tablecolumnheader-element-format.md)

[Writing a PowerShell Formatting File](./writing-a-powershell-formatting-file.md)
