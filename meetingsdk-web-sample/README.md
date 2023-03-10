# Zoom Meeting SDK Sample App - Web

Use of this sample app is subject to our [Terms of Use](https://zoom.us/docs/en-us/zoom_api_license_and_tou.html).

The [Zoom Meeting SDK](https://marketplace.zoom.us/docs/sdk/native-sdks/web) embeds the Zoom Meeting and Webinar experience in a website through a highly optimized WebAssembly module.

![Zoom Meeting SDK Client View](https://marketplace.zoom.us/docs/static/msdk-web-client-view-6276487add553e9849f39a7cec9ac7c7.gif)

## Installation

To get started, clone the repo:

`$ git clone https://github.com/zoom/sample-app-web.git`

## Setup

1. Once cloned, navigate to the `sample-app-web/CDN` directory for the Client View CDN sample, or `sample-app-web/Local` for the Client View NPM sample, or `sample-app-web/Components` for the Component View NPM sample:

   `$ cd sample-app-web/CDN` or `$ cd sample-app-web/Local` or `$ cd sample-app-web/Components`

1. Then install the dependencies:

   `$ npm install`

1. Open the directory in your code editor.

1. Open the `sample-app-web/CDN/js/index.js` or `sample-app-web/Local/js/index.js` or `sample-app-web/Components/tools/nav.js` file respectively, and enter required values for the variables:

   | Key                   | Value Description |
   | -----------------------|-------------|
   | `CLIENT_ID`     | Your Client ID or SDK Key. Required. |
   | `CLIENT_SECRET`  | Your Client Secret or SDK Secret. Required. |

   Example:

   ```js
   var CLIENT_ID = "YOUR_CLIENT_ID_OR_SDK_KEY"
   var CLIENT_SECRET = "YOUR_CLIENT_SECRET_OR_SDK_SECRET"
   ```

   > Reminder to not publish this sample app as is. Replace the frontend signature generator with a [backend signature generator](https://marketplace.zoom.us/docs/sdk/native-sdks/auth#generate-the-sdk-jwt) to keep your SDK Secret safe.

1. Save `index.js` or `nav.js` respectively.

1. Run the app:

   `$ npm start`

## Usage

1. Navigate to http://localhost:9999 for the `CDN` or
`Local` sample, or http://localhost:3000 for the `Components` sample. Then, enter in a Meeting or Webinar number and passcode, choose host or attendee (participant), and, click "join".

   ### Client View
   
   ![Zoom Meeting SDK Client View](https://marketplace.zoom.us/docs/static/msdk-web-client-view-6276487add553e9849f39a7cec9ac7c7.gif)

   > The Client View provides the option to display the Meeting SDK as a full page. This allows for a familiar Zoom Meeting experience because the Client View is the same as the [Zoom Web Client](https://support.zoom.us/hc/en-us/articles/214629443-Zoom-Web-Client), except it lives inside your own web page.

   ### Component View

   ![Zoom Meeting SDK Component View](https://marketplace.zoom.us/docs/static/msdk-web-component-view-64311bbbf32eaddfc2f3fac6e89928df.gif)

   > The Component View provides the option to display the Meeting SDK in components on your page. This allows for a more flexible design.

> Learn more about [Gallery View requirements](https://marketplace.zoom.us/docs/sdk/overview/improve-performance) and [see more product screenshots](https://marketplace.zoom.us/docs/sdk/overview/websdk-gallery-view/#how-views-look-with-and-without-sharedarraybuffer).

For the full list of features and event listeners, as well as additional guides, see our [Meeting SDK docs](https://marketplace.zoom.us/docs/sdk/native-sdks/web).

## Need help?

If you're looking for help, try [Developer Support](https://devsupport.zoom.us) or our [Developer Forum](https://devforum.zoom.us). Priority support is also available with [Premier Developer Support](https://zoom.us/docs/en-us/developer-support-plans.html) plans.
