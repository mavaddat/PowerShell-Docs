---
description: SelectionSetName Element for ViewSelectedBy
ms.date: 08/25/2021
title: SelectionSetName Element for ViewSelectedBy
---
# SelectionSetName Element for ViewSelectedBy

Specifies a set of .NET objects that are displayed by the view.

## Schema

- Configuration Element
- ViewDefinitions Element
- View Element
- ViewSelectedBy Element
- SelectionSetName Element

## Syntax

```xml
<SelectionSetName>Name of selection set<SelectionSetName>
```

## Attributes and Elements

The following sections describe the attributes, child elements, and the parent element of the
`SelectionSetName` element.

### Attributes

None.

### Child Elements

None.

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[ViewSelectedBy Element](./viewselectedby-element-format.md)|Defines the .NET objects that are displayed by the view.|

## Text Value

Specify the name of the selection set that is defined by the `Name` element for the selection set.

## Remarks

You can use selection sets when you have a set of related objects that you want to reference by
using a single name, such as a set of objects that are related through inheritance. For more
information about defining and referencing selection sets, see [Defining Sets of Objects](./defining-selection-sets.md).

## Example

The following example shows how to specify a selection set for a list view. The same schema is used
for table, wide, and custom views.

```xml
<View>
  <Name>Name of View</Name>
  <ViewSelectedBy>
    <SelectionSetName>NameofSelectionSet</SelectionSetName>>
  </ViewSelectedBy>
  <ListControl>...</ListControl>
</View>
```

## See Also

[Defining Selection Sets](./defining-selection-sets.md)

[ViewSelectedBy Element](./viewselectedby-element-format.md)

[Writing a PowerShell Formatting File](./writing-a-powershell-formatting-file.md)
