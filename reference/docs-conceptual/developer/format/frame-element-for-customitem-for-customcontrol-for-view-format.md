---
description: Frame Element for CustomItem for CustomControl for View
ms.date: 08/23/2021
title: Frame Element for CustomItem for CustomControl for View
---
# Frame Element for CustomItem for CustomControl for View

Defines how the data is displayed, such as shifting the data to the left or right. This element is
used when defining a custom control view.

## Schema

- Configuration Element
- ViewDefinitions Element
- View Element
- CustomControl Element
- CustomEntries Element
- CustomEntry Element
- CustomItem Element
- Frame Element

## Syntax

```xml
<Frame>
  <LeftIndent>NumberOfCharactersToShift</LeftIndent>
  <RightIndent>NumberOfCharactersToShift</RightIndent>
  <FirstLineHanging>NumberOfCharactersToShift</FirstLineHanging>
  <FirstLineIndent>NumberOfCharactersToShift</FirstLineIndent>
  <CustomItem>...</CustomItem>
</Frame>
```

## Attributes and Elements

The following sections describe attributes, child elements, and the parent element of the `Frame`
element.

### Attributes

None.

### Child Elements

|Element|Description|
|-------------|-----------------|
|`CustomItem Element`|Required Element|
|[FirstLineHanging Element](./firstlinehanging-element-for-frame-for-customcontrol-for-view-format.md)|Optional element.<br /><br /> Specifies how many characters the first line of data is shifted to the left.|
|[FirstLineIndent Element](./firstlineindent-element-for-frame-for-customcontrol-for-view-format.md)|Optional element.<br /><br /> Specifies how many characters the first line of data is shifted to the right.|
|[LeftIndent Element](./leftindent-element-for-frame-for-customcontrol-for-view-format.md)|Optional element.<br /><br /> Specifies how many characters the data is shifted away from the left margin.|
|[RightIndent Element](./rightindent-element-for-frame-for-customcontrol-for-view-format.md)|Optional element.<br /><br /> Specifies how many characters the data is shifted away from the right margin.|

### Parent Elements

|Element|Description|
|-------------|-----------------|
|[CustomItem Element for CustomEntry for View](./customitem-element-for-customentry-for-customcontrol-for-view-format.md)|Defines what data is displayed by the control and how it is displayed.|

## Remarks

You cannot specify the [FirstLineHanging](./firstlinehanging-element-for-frame-for-customcontrol-for-view-format.md) and the [FirstLineIndent](./firstlineindent-element-for-frame-for-customcontrol-for-view-format.md) elements in the same `Frame` element.

## See Also

[FirstLineHanging Element](./firstlinehanging-element-for-frame-for-customcontrol-for-view-format.md)

[FirstLineIndent Element](./firstlineindent-element-for-frame-for-customcontrol-for-view-format.md)

[LeftIndent Element](./leftindent-element-for-frame-for-customcontrol-for-view-format.md)

[RightIndent Element](./rightindent-element-for-frame-for-customcontrol-for-view-format.md)

[CustomItem Element for CustomEntry for View](./customitem-element-for-customentry-for-customcontrol-for-view-format.md)

[Writing a PowerShell Formatting File](./writing-a-powershell-formatting-file.md)
