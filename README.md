# How to Add Image and Text Combinations to Radial Menu Items

This knowledge base article demonstrates how to add both image and text to each item in a Syncfusion SfRadialMenu in a .NET MAUI application. The sample project shows how to build a visually rich radial menu where each menu item contains a thumbnail image and a label, making it ideal for profile selection, contact lists, action groups, and categorized shortcuts.

## Overview

The Syncfusion Radial Menu control in .NET MAUI enables developers to present actions in a circular layout. In many UX scenarios, a plain icon or a plain text item is not enough. A combination of an image and a label creates a more intuitive menu and improves discoverability. This sample uses an `SfRadialMenuItem` with the `Image` and `Text` properties assigned together so that the item displays both a picture and a descriptive name.

The example application is structured as a simple MAUI page with a `SfRadialMenu` placed inside a Grid. The menu uses a center button titled `Profiles`, and each radial item is configured with a custom image and text. This pattern is ideal for selecting people, accounts, categories, or dashboard actions without crowding the interface.

## Project Features

- .NET MAUI application built using Syncfusion controls
- Circular radial menu layout with centered title
- Each menu item displays both image and text
- Easy to customize item size, alignment, and content
- Suitable for action menus, contact lists, and profile selection UIs

## Implementation Details

The core working pattern is to create an `SfRadialMenu` and define each item as an `SfRadialMenuItem`. Each item is assigned:

- `Text` for the visible label
- `Image` for the item icon or avatar
- `ItemHeight` and `ItemWidth` for consistent sizing

A typical XAML setup looks like this:

```xml
<radialMenu:SfRadialMenu CenterButtonText="Profiles">
    <radialMenu:SfRadialMenu.Items>
        <radialMenu:SfRadialMenuItem ItemHeight="60" ItemWidth="60" Text="John" Image="john.png" />
        <radialMenu:SfRadialMenuItem ItemHeight="60" ItemWidth="60" Text="Krish" Image="krish.png" />
        <radialMenu:SfRadialMenuItem ItemHeight="60" ItemWidth="60" Text="Ram" Image="ram.png" />
    </radialMenu:SfRadialMenu.Items>
</radialMenu:SfRadialMenu>
```

This approach helps create an attractive radial menu that is not only functional but also visually engaging. The images can be added to the `Resources/Images` folder of the MAUI project and referenced by filename without the file extension.

## Prerequisites

Before running this sample, make sure the following are available:

- Visual Studio 2022 with MAUI workloads installed
- .NET SDK supported by your MAUI project
- Syncfusion MAUI Radial Menu package referenced in the project
- Appropriate platform targets for Android, iOS, Windows, or Mac Catalyst

## Steps to Run the Sample

1. Open the solution file `ImageAndTextCombinations.slnx` in Visual Studio.
2. Restore NuGet packages.
3. Confirm that the image files such as `john.png`, `krish.png`, `ram.png`, and others are present in the project resources.
4. Set the target platform and run the application.
5. The radial menu will display on the page with each item showing both an image and a text label.

## Why This Pattern is Useful

Using image and text together in radial menu items improves usability across many modern app designs. Users can quickly recognize actions and identify options without reading detailed labels. It also creates a polished UI for profile-based navigation, contact selection, and service actions. Because the control is circular, the menu can save screen space while still presenting meaningful information.

## Notes

This sample can be customized further by changing:

- the item size and spacing
- the center button text
- the menu background and style
- the source images and names
- the number of items displayed

You can also extend this approach to other data-driven scenarios such as employee selection, product categories, or favorite actions in a dashboard.

## Summary

The combination of `Image` and `Text` in `SfRadialMenuItem` is a simple and effective way to create a more refined and user-friendly radial menu. This sample demonstrates the exact pattern needed to achieve that in a .NET MAUI app, and it can be adapted to many real-world business scenarios.

This demo is a helpful reference for developers who want to build a polished, informative radial menu without sacrificing space or readability.
