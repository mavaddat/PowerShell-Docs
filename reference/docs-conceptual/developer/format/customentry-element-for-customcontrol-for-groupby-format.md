---
description: CustomEntry Element for CustomControl for GroupBy
ms.date: 08/20/2021
title: CustomEntry Element for CustomControl for GroupBy
---
# CustomEntry Element for CustomControl for GroupBy

Provides a definition of the control. This element is used when defining how a new group of objects
is displayed.

## Schema

- Configuration Element
- ViewDefinitions Element
- View Element
- GroupBy Element
- CustomControl Element
- CustomEntries Element
- CustomEntry Element

## Syntax

```xml
<CustomEntry>
  <EntrySelectedBy>...</EntrySelectedBy>
  <CustomItem>...</CustomItem>
</CustomEntry>
```

## Attributes and Elements

The following sections describe attributes, child elements, and the parent elements of the
`CustomEntry` element.

### Attributes

None.

### Child Elements

|Element|Description|
|-------------|-----------------|
|[EntrySelectedBy Element for CustomEntry for GroupBy](./entryselectedby-element-for-customentry-for-groupby-format.md)|Optional element.<br /><br /> Defines the .NET types that use this control definition or the condition that must exist for this definition to be used.|
|[CustomItem Element for CustomEntry for GroupBy](./customitem-element-for-customentry-for-groupby-format.md)|Required element.<br /><br /> Defines how the control displays the data.|

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[CustomEntries Element for CustomControl for GroupBy](./customentries-element-for-customcontrol-for-groupby-format.md)|Provides the definitions for the control.|

## Remarks

## See Also

[EntrySelectedBy Element for CustomEntry for GroupBy](./entryselectedby-element-for-customentry-for-groupby-format.md)

[CustomItem Element for CustomEntry for GroupBy](./customitem-element-for-customentry-for-groupby-format.md)

[CustomEntries Element for CustomControl for GroupBy](./customentries-element-for-customcontrol-for-groupby-format.md)

[Writing a PowerShell Formatting File](./writing-a-powershell-formatting-file.md)
