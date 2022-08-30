# Instagram Clone with Parse Server on AWS

Coursework from [The Complete Android Oreo Developer Course - Build 23 Apps!](https://www.udemy.com/course/the-complete-android-oreo-developer-course/) at Udemy.

An Instagram Clone that works with the [Parse Server](https://parseplatform.org/) on [Amazon EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html).

## General

- **Version**: 1.0
- **Compatibility**: Android 6.0

## Demo

![demo](demo/demo.gif)

## Features

- Advanced keyboard management
- Show the user list
- Users can upload photos from the camera and view other users' feeds
- Admins can manage data via [Parse Dashboard](https://github.com/parse-community/parse-dashboard)

## Setup

If you want to run this project on your own server, you must:

1. Launch a [Parse Server instance on AWS](https://aws.amazon.com/marketplace/pp/prodview-gu6judefvlbxg?sr=0-1&ref_=beagle&applicationId=AWSMPContessa#pdp-overview).
2. [Set up AWS EC2 Parse Server](https://foystor.github.io/2022/03/15/set-up-aws/).
3. Initialize the Parser Server in the ```StarterApplication.java``` file:

```
// Add your initialization code here
Parse.initialize(new Parse.Configuration.Builder(getApplicationContext())
        .applicationId("")      // appId
        .clientKey("")          // masterKey
        .server("")             // serverURL
        .build()
);
```

## License

[MIT License](LICENSE)