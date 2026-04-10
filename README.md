# Pascal

Table of Contents
- [Motivation and Background](#motivation-and-background)
- [Features](#features)
- [Screenshots](#screenshots)
- [Technical Implementation](#technical-implementation)
  - [Sensor Integration](#sensor-integration)
  - [Physics Engine](#physics-engine)
  - [UI](#ui)
  - [Accessibility](#accessibility)
- [How to run](#how-to-run)
- [Future Steps](#future-steps)

Pascal is an iOS app playground that allows users to boil eggs perfectly by automatically accounting for local atmospheric pressure and altitude. The main feature of the app is its hardware-driven cooking calculator. Users simply start the app, and it uses the device's barometric sensors to run a heat-transfer simulation, calculating the exact cooking time needed for a perfect boil based on their current environment.

## Motivation and Background

I built this project as my submission for the Swift Student Challenge. Boiling an egg seems like a simple everyday task, but the boiling point of water drops significantly at higher altitudes, which ruins standard cooking times. Since I have a strong foundation in core sciences (Physics and Mathematics), I wanted to solve this real-world problem by bridging the gap between hardware sensors and mathematical modeling. 

I decided to utilize the power of the iPhone's internal sensors combined with Newton's Law of Cooling. All you need to do is open the app, and it does the complex physics calculations for you. I tried to make the app as easy and beautiful as possible, creating a very friendly glassmorphic UI, so users don't spend time on complex features but just get perfectly cooked eggs.

## Features

**Smart Time Calculation**
- Automatically reads real-time local atmospheric pressure.
- Adjusts water boiling point dynamically based on altitude.
- Calculates perfect cooking times using a heat-transfer simulation based on Newton's Law of Cooling.

**Modern User Experience**
- Clean, modern glassmorphic UI built entirely in SwiftUI.
- Beautiful, intuitive timer interface.

**Accessibility**
- Integrated haptic feedback to ensure users are notified when their egg is ready, even without sound.
- Documented scientific inspiration and technical implementation for educational purposes.

## Screenshots

[Watch Demo Version](link_to_your_video)

![Image 1](link_to_image) ![Image 2](link_to_image) ![Image 3](link_to_image)

## Technical Implementation

In this section, I describe what frameworks I used and some interesting moments that I encountered during development.

### Sensor Integration
To make the app accurate, I had to tap into the device's actual hardware. I utilized Apple's frameworks to access the barometric altimeter. Reading this raw data and converting it into a usable atmospheric pressure metric was crucial for the app's core logic. 

### Physics Engine
My application relies heavily on mathematical modeling. I wrote custom Swift logic to implement Newton's Law of Cooling. This simulates the heat transfer into the egg, adjusting the required time dynamically based on the pressure variables retrieved from the device's sensors. 

### UI
I used native Apple Frameworks for the interface. All code was written in Swift using the SwiftUI framework, heavily focusing on a glassmorphic aesthetic to make the app feel modern and deeply integrated into the iOS ecosystem.

### Accessibility
One of the most important parts for me was making the app accessible. I implemented haptic feedback so the application doesn't rely purely on visual or auditory cues, ensuring an inclusive experience for all users.

## How to run

Clone the repository:
```bash
git clone git@github.com:Paarth2006/Pascal.git
