# Providing locally hosted content to WebViews explainer

## Authors:

- Niklas Merz, Apache Software Foundation

## Use-case / Challenge

[The Origin in a WebView for locally hosted content](https://webview-cg.github.io/usage-and-challenges/#the-origin-in-a-webview-for-locally-hosted-content)

## Introduction

WebViews are widely used for building apps on the dominating mobile and desktop platforms. Up to 30% of apps found in the app stores (Apple and Google) are built with frameworks like Apache Cordova and CapacitorJS. Those two frameworks use one big WebView for providing app developers a native wrapper and some plugins for their Web app. App developers build their Web application and put the HTML, CSS and JavaScript files in one folder. The framework then takes care of building a native app project and bundling the Web code as a native application ready to distribute via the app stores.

Using this approach the native app is responsible for "hosting" the content for the WebView. In the past this was often done by using the file protocol (`file:/path/to/content`) to load the Web content from the app bundle. Mondern web APIs and some frontend frameworks don't work with pages loaded from `file:`. This led WebView vendors to build APIs for app developers to load their content into the WebView. The existing APIs uses each their own different approaches and origins, which imposes challenges to developers.

## Goals [or Motivating Use Cases, or Scenarios]

[What is the **end-user need** which this project aims to address?]

- different origins
- different capabilities to modify/intercept requests & response

## Non-goals

[If there are "adjacent" goals which may appear to be in scope but aren't,
enumerate them here. This section may be fleshed out as your design progresses and you encounter necessary technical and other trade-offs.]

## [API 1]

[For each related element of the proposed solution - be it an additional WebView API, a new web platform API, a new concept etc., create a section which briefly describes it.]

```js
// Provide example code - not IDL - demonstrating the design of the feature.

// If this API can be used on its own to address a user need,
// link it back to one of the scenarios in the goals section.

// If you need to show how to get the feature set up
// (initialized, or using permissions, etc.), include that too.
```

[Where necessary, provide links to longer explanations of the relevant pre-existing concepts and API.
If there is no suitable external documentation, you might like to provide supplementary information as an appendix in this document, and provide an internal link where appropriate.]

[If this is already specced, link to the relevant section of the spec.]

[If spec work is in progress, link to the PR or draft of the spec.]

## [API 2]

[etc.]

## Key scenarios

[If there are a suite of interacting APIs, show how they work together to solve the key scenarios described.]

### Scenario 1

[Description of the end-user scenario]

```js
// Sample code demonstrating how to use these APIs to address that scenario.
```

### Scenario 2

[etc.]

## Detailed design discussion

### [Tricky design choice #1]

[Talk through the tradeoffs in coming to the specific design point you want to make.]

```js
// Illustrated with example code.
```

[This may be an open question,
in which case you should link to any active discussion threads.]

### [Tricky design choice 2]

[etc.]

## Considered alternatives

[This should include as many alternatives as you can,
from high level architectural decisions down to alternative naming choices.]

### [Alternative 1]

[Describe an alternative which was considered,
and why you decided against it.]

### [Alternative 2]

[etc.]

## References & acknowledgements

[Your design will change and be informed by many people; acknowledge them in an ongoing way! It helps build community and, as we only get by through the contributions of many, is only fair.]

[Unless you have a specific reason not to, these should be in alphabetical order.]

Many thanks for valuable feedback and advice from:

- [Person 1]
- [Person 2]
- [etc.]

