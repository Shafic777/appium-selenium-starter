<h1 align="center">
  Appium Selenium Starter 
</h1>
<p align="center" style="font-size: 1.2rem;">Simple and easy to use boilerplate for writing tests for mobile or web.</p>

<hr />

[![Build Status][build-badge]](build)
[![downloads][downloads-badge]](downloads)
[![MIT License][license-badge]](license)

[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors)
[![PRs Welcome][prs-badge]](prs) 
[![Code of Conduct][coc-badge]](coc)
[![Watch on GitHub][github-watch-badge]](github-watch)
[![Star on GitHub][github-star-badge]](github-star)
[![Tweet][twitter-badge]](twitter)

## Requirements

1. PHP >= 7.0

## Installation

You can install this `appium-codeception-boilerplate` using the following methods:

### Cloning the repo

Run the following command to configure the boilerplate on your machine:

```bash
git clone git@github.com:me-io/appium-codeception-starter.git
```

### Via composer create-project

Alternatively, you may also install `appium-codeception-starter` by issuing the Composer create-project command in your 
terminal:

```bash
composer create-project --prefer-dist me-io/appium-codeception-starter
```

## Running Example Tests

You can find the android and ios example tests inside `_example_tests` directory. We also put some example android
and ios apps inside `_example_tests/_data/test-apps` directory.

### Android Tests

You need to configure your enviorment for android testing. Just run the following command inside your terminal 
it will configure your enviorment.

```bash
./vendor/bin/appium.sh configure
```

For running android emulator we are using genymotion. Follow this [guide](https://shankargarg.wordpress.com/2016/02/25/setup-genymotion-android-emulators-on-mac-os/) 
if you don't know how to install and run android emulator.After setting up android emulator now you need to 
update the `deviceName` inside `_example_tests/android.suite.yml` file.

![Imgur](https://i.imgur.com/znQkuLq.png)

### Staring Appium Server

Now inside your terminal run the following command:

```bash
./vendor/bin/appium.sh start
```

### Running Tests

To run the android tests run the following codecept command inside your terminal:

```bash
./vendor/bin/codecept -c _example_tests_codeception.yml run android --steps
```

![Android](https://i.imgur.com/PdqDRFa.gif)

> **Note:** Make sure appium server is running before running the android tests.

### iOS Tests

Just like we did earlier first we need to configure our machine before running iOS tests. To configure your 
machine just run the following command inside your terminal and you are ready to go:

```bash
./vendor/bin/appium.sh configure
```

### Staring Appium Server

Now inside your terminal run the following command:

```bash
./vendor/bin/appium.sh start
```

### Running Tests

To run the ios tests run the following codecept command inside your terminal:

```bash
./vendor/bin/codecept -c _example_tests_codeception.yml run ios --steps
```

![iOS](https://i.imgur.com/Au45fXv.gif)

## Contributors

A huge thanks to all of our contributors:

| [<img src="https://avatars0.githubusercontent.com/u/45731?v=3" width="100px;"/><br /><sub><b>Mohamed Meabed</b></sub>](https://github.com/Meabed)<br />[💬](#question-meabed "Answering Questions") [📖](#documentation-meabed "Documentation") [👀](#review-meabed "Reviewed Pull Requests") [📢](#talk-meabed "Talks") | [<img src="https://avatars2.githubusercontent.com/u/16267321?" width="100px;"/><br /><sub><b>Zeeshan Ahmad</b></sub>](https://github.com/zeeshanu)<br />[💻](#code-zeeshan "Code") [📖](#documentation-zeeshan "Documentation") |
|:---: | :---: |
## License

The code is available under the [MIT license](LICENSE.md).

[build-badge]: https://img.shields.io/travis/me-io/appium-selenium-starter.svg?style=flat-square
[downloads-badge]: https://img.shields.io/packagist/dm/me-io/appium-selenium-starter.svg?style=flat-square
[license-badge]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[prs]: http://makeapullrequest.com
[coc-badge]: https://img.shields.io/badge/code%20of-conduct-ff69b4.svg?style=flat-square
[github-watch-badge]: https://img.shields.io/github/watchers/me-io/appium-selenium-starter.svg?style=social
[github-watch]: https://github.com/me-io/appium-selenium-starter/watchers
[github-star-badge]: https://img.shields.io/github/stars/me-io/appium-selenium-starter.svg?style=social
[github-star]: https://github.com/me-io/appium-selenium-starter/stargazers
[twitter]: https://twitter.com/intent/tweet?text=Check%20out%20appium-selenium-starter!%20https://github.com/me-io/appium-selenium-starter%20%F0%9F%91%8D
[twitter-badge]: https://img.shields.io/twitter/url/https/github.com/me-io/appium-selenium-starter.svg?style=social