---
description: EntrySelectedBy Element for CustomEntry for GroupBy
ms.date: 08/23/2021
title: EntrySelectedBy Element for CustomEntry for GroupBy
---
# EntrySelectedBy Element for CustomEntry for GroupBy

Defines the .NET types that use this control definition or the condition that must exist for this
definition to be used. This element is used when defining how a new group of objects is displayed.

## Schema

- Configuration Element
- ViewDefinitions Element
- View Element
- GroupBy Element for View
- CustomControl Element
- CustomEntries Element
- CustomEntry Element
- EntrySelectedBy Element

## Syntax

```xml
<EntrySelectedBy>
  <TypeName>Nameof.NetType</TypeName>
  <SelectionSetName>NameofSelectionSet</SelectionSetName>
  <SelectionCondition>...</SelectionCondition>
</EntrySelectedBy>
```

## Attributes and Elements

The following sections describe attributes, child elements, and parent element of the
`EntrySelectedBy` element. You must specify at least one type, selection set, or selection condition
for a definition. There is no maximum limit to the number of child elements that you can use.

### Attributes

None.

### Child Elements

|Element|Description|
|-------------|-----------------|
|[SelectionCondition Element for EntrySelectedBy for GroupBy](./selectioncondition-element-for-entryselectedby-for-groupby-format.md)|Optional element.<br /><br /> Defines the condition that must exist for this definition to be used.|
|[SelectionSetName Element for EntrySelectedBy for GroupBy](./selectionsetname-element-for-entryselectedby-for-groupby-format.md)|Optional element.<br /><br /> Specifies a set of .NET types that use this definition of the control.|
|[TypeName Element for EntrySelectedBy for GroupBy](./typename-element-for-entryselectedby-for-groupby-format.md)|Optional element.<br /><br /> Specifies a .NET type that uses this definition of the control.|

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[CustomEntry Element for CustomControl for GroupBy](./customentry-element-for-customcontrol-for-groupby-format.md)|Provides a definition of the control.|

## Remarks

Selection conditions are used to define a condition that must exist for the definition to be used,
such as when an object has a specific property or when a specific property value or script evaluates
to `true`. For more information about selection conditions, see [Defining Conditions for when a View Entry or Item is Used](./defining-conditions-for-displaying-data.md).

## See Also

[SelectionCondition Element for EntrySelectedBy for GroupBy](./selectioncondition-element-for-entryselectedby-for-groupby-format.md)

[SelectionSetName Element for EntrySelectedBy for GroupBy](./selectionsetname-element-for-entryselectedby-for-groupby-format.md)

[TypeName Element for EntrySelectedBy for GroupBy](./typename-element-for-entryselectedby-for-groupby-format.md)

[CustomEntry Element for CustomEntries for Controls for View](./customentry-element-for-customentries-for-controls-for-view-format.md)

[Writing a PowerShell Formatting File](./writing-a-powershell-formatting-file.md)
