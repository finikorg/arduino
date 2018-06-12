WebUSB Zephyr demo
==================

Origins
-------

Originally forked from https://github.com/webusb/arduino

Example JavaScript code are available in the demos directory.

Zephyr sample provode following functionality:

 * The WebUSB landing page descriptor, providing a hint to the browser about
   what page the user should navigate to to interact with the device. In
   Google Chrome the presence of this descriptor causes the browser to display
   a notification when the device is connected. The user can click on this
   notification to navigate directly to the provided URL.
 * Microsoft OS 2.0 Descriptors which instruct the Windows operating system
   (8.1 and above) to automatically the `WinUSB.sys` driver so that the browser
   can connect to the device.

Compatible Hardware
-------------------

Tested with following hardware with Zephyr

 * Quark SE C1000 devboard

Getting Started
---------------

1. When Zephyr booted you should see a notification from Chrome: "Go to [https://finikorg.github.io/webusb-zephyr-demo/demos/](https://finikorg.github.io/webusb-zephyr-demo/demos/) to connect." Try it out!

  **Windows:** This notification is currently disabled in Chrome on Windows due to [Chromium issue 656702](https://crbug.com/656702). Implementation of new, more stable USB support for Windows is tracked on Chromium issues [422562](https://crbug.com/422562) and [637404](https://crbug.com/637404).
