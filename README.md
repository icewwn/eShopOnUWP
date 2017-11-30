# Introduction 
This repo contains a UWP sample application for Windows 10 Fall Creators Update. It is focused on Line of Business scenarios, showing how to use the latest Windows capabilities in Desktop applications.

Some of the features showcased by this application include:

- The MVVM Design Pattern
- Use of Fluent Design System
- Multiple Data Providers
- Common CRUD operations
- .NET Standard 2.0
- REST API requests
- Windows Hello
- Telerik controls

**CI Build**
[![Build status](https://ci.appveyor.com/api/projects/status/wqn7or9m95xjurjy?svg=true)](https://ci.appveyor.com/project/rido-min/eshoponuwp)

**CD Build**
[![Build status](https://rido.visualstudio.com/_apis/public/build/definitions/989ddbdd-c86a-4fa8-8d80-89eb785d8056/83/badge)](https://aka.ms/eshopuwp)

# Prerequisites

## System requirements:
- Windows 10 Fall Creators Update. To run the application you should be running Windows version 10.0.16299 or above.
	- You can get it as described [here](https://blogs.windows.com/windowsexperience/2017/10/17/get-windows-10-fall-creators-update)
- Visual Studio 15.4 -> [Download](http://visualstudio.com/)
	- Including the Windows 10 FCU SDK 10.0.16299

# Getting Started

You can install a working version of the app from
[https://aka.ms/eshopuwp](https://aka.ms/eshopuwp)

If you want to execute the app from Visual Studio 2017, follow these steps:
- Clone or download a Zip copy of the entire solution
- Open the eShop.UWP.sln solution in Visual Studio 2017
- Ensure eShop.UWP is the startup project
- Start the project

> Note: In Visual Studio 2017, the platform target defaults to ARM, so be sure to change that to x64 or x86 if you want to test on a non-ARM device

# Features

## Windows Hello
There are two ways to log-in, either with user/password or using Windows Hello. The first time the application is run, the user/password log in option will appear by default. After log-in you will be prompted to enable Windows Hello for that user.

Once you have logged-in using Windows Hello, your user will be saved and the next time you open the application Windows Hello authentication will appear as default. Depending on how your Windows Hello settings are (Settings/Accounts/Sign-in options), you will be able to authenticate by using:

- Pin
- Face recognition
- Fingerprint
- Etc.

![Windows Hello](/docs/Login.gif)

## Data Providers
From the Settings page, you can select one of the following Data Providers, each supporting CRUD operations and demonstrating different data access technologies:
- Local (json file)
- REST API
- SQL Server

![Settings](/docs/Settings.jpg)

## Fluent Design

### Acrylic material
[Acrylic material](https://docs.microsoft.com/windows/uwp/design/style/acrylic) is a type of Brush that creates a partially transparent texture.

![Acrylic material](/docs/AcrylicFluent.png)

### Connected animations
[Connected animations](https://docs.microsoft.com/windows/uwp/style/connected-animation) let you create a dynamic and compelling navigation experience by animating the transition of an element between two different views.

![Connected animations](/docs/ConnectedAnimation.gif)

### Reveal
[Reveal](https://docs.microsoft.com/windows/uwp/style/reveal) is a lighting effect that helps bring depth and focus to your app's interactive elements.

![Reveal](/docs/RevealFluent.gif)

### ShyHeader
[ShyHeader](https://github.com/Microsoft/WindowsUIDevLabs/tree/master/SampleGallery/Samples/SDK%2014393/ShyHeader) demonstrates how to use ExpressionAnimations Tookit with a ScrollViewer to create a shinking header tied to scroll position.

![ShyHeader](/docs/ShyHeaderToolkit.gif)

