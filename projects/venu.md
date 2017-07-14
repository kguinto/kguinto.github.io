layout: page
title: Venü
---

Ven&#252; is an iOS app developed for the [AT&T Hackathon](https://www.eventbrite.com/e/att-hackathon-hawaii-tickets-31100289804) that occurred in March 2017 in Honolulu, Hawaii. It was conceptualized, designed, and coded over a 24-hour period by myself and four other students from UH Manoa.

The premise of the idea was an app for event venues to provide information for attendees, such as locations for bathrooms, emergency exit routes, schedules, or general announcements. An organizer would submit information through a website, and attendees could access the event information by scanning a QR code or with a [BLE](https://en.wikipedia.org/wiki/Bluetooth_Low_Energy) connection.

The app was developed for iOS using Xcode, and the backend was implemented through [Amazon Web Services' DynamoDB](https://aws.amazon.com/dynamodb/).

Ultimately, the project was... <i>a learning experience</i>. Difficulties arose with time and resource management, lack of experience with the environments used, and group organization. As a group, we got stuck on the more technical features-- namely, trying to set up a Raspberry Pi 2 as an [iBeacon](https://developer.apple.com/ibeacon/), and trying to implement multi-layered maps to display different routes on a map. We also had trouble managing the coding between five people, two Macbooks, and two macOS VM.

What we did accomplish was having an app that successfully pulled data from the AWS database, using the makeshift iBeacon. I personally learned a lot of technical things regarding iOS, Amazon Web Services and BLE technology, but moreso learned a lot about managing a team, prioritizing tasks, and properly managing time and resources.
