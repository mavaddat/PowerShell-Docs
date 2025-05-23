---
description: SelectionSetName Element for SelectionCondition for EntrySelectedBy for WideEntry
ms.date: 08/25/2021
title: SelectionSetName Element for SelectionCondition for EntrySelectedBy for WideEntry
---
# SelectionSetName Element for SelectionCondition for EntrySelectedBy for WideEntry

Specifies the set of .NET types that trigger the condition. When any of the types in this set are
present, the condition is met, and the object is displayed by using this definition of the wide
view.

## Schema

- Configuration Element
- ViewDefinitions Element
- View Element
- WideControl Element
- WideEntries Element
- WideEntry Element
- EntrySelectedBy Element
- SelectionCondition Element
- SelectionSetName Element

## Syntax

```xml
<SelectionSetName>NameofSelectionSet</SelectionSetName>
```

## Attributes and Elements

The following sections describe attributes, child elements, and the parent element of the
`SelectionSetName` element.

### Attributes

None.

### Child Elements

None.

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[SelectionCondition Element for EntrySelectedBy for WideEntry](./selectioncondition-element-for-entryselectedby-for-widecontrol-format.md)|Defines the condition that must exist for this definition to be used.|

## Text Value

Specify the name of the selection set.

## Remarks

The selection condition can specify a selection set or .NET type, but cannot specify both. For more
information about how to use selection conditions, see [Defining Conditions for when Data is Displayed](./defining-conditions-for-displaying-data.md).

Selection sets are common groups of .NET objects that can be used by any view that the formatting
file defines. For more information about creating and referencing selection sets, see [Defining Sets of Objects](./defining-selection-sets.md).

For more information about other components of a wide view, see [Creating a Wide View](./creating-a-wide-view.md).

## See Also

[Creating a Wide View](./creating-a-wide-view.md)

[Defining Conditions for When Data Is Displayed](./defining-conditions-for-displaying-data.md)

[Defining Selection Sets](./defining-selection-sets.md)

[SelectionCondition Element for EntrySelectedBy for WideEntry](./selectioncondition-element-for-entryselectedby-for-widecontrol-format.md)

[TypeName Element for SelectionCondition for EntrySelectedBy for WideEntry](./typename-element-for-selectioncondition-for-entryselectedby-for-widecontrol-format.md)

[Writing a PowerShell Formatting File](./writing-a-powershell-formatting-file.md)
