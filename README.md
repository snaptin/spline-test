# Spline Tests

This repo includes the tests used in [our article](https://webdesign.tutsplus.com) published on Tuts+ Web Design, which discusses how to improve the web performance of Spline scenes.

You can [sign up for a Spline account here](https://app.spline.design/signin) for free. Or, you can [check out their homepage here](https://spline.design/).

## The Base Folders

The `zip/` and `zip-web` folders include our test code as it was exported from Spline:
- `zip` is an ECMAScript app – you can test it on [this web page](https://snaptin.github.io/spline-test/zip/).
- `zip-web` is a website –you can test it on [this web page](https://snaptin.github.io/spline-test/zip-web/).

Both folders includes the same design — only in a different format. The object you can see on the screen is an interactive 3D scene created with Spline that you can move around using the cursor. Visually speaking, it's a 3D candy letter.

## The Experiments

The `experiments/` folder implements some experiments on the `zip-web` folder.

### Experiment 1

Experiment 1 removes the Spine logo to demonstrate that the `<canvas>` element is not included in LCP.

You can test it [here](https://snaptin.github.io/spline-test/experiments/1/).

### Experiment 2

Experiment 2 adds extra text to the page and removes `overflow: hidden;` from the `<body>` element to see how web performance metrics (mainly INP and CLS) change when there's other content on the page.

You can test it [here](https://snaptin.github.io/spline-test/experiments/2/).

### Experiment 3

Experiment 3 puts the `<canvas>` element into a `<div>` and adds inline `width` and `height` rules to it to see if it improves web performance results (mainly INP and CLS).

You can test it [here](https://snaptin.github.io/spline-test/experiments/3/).

## Recommended Testing Tools
- [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview) for local lab tests in the Chrome browser
- [DebugBear](https://www.debugbear.com/test/website-speed) for remote lab tests and RUM (real user monitoring)
