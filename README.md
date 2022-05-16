# Secret Server Postman Collections

This repository host a Postman collection for latest versions of Secret Server. An environment file is also included that the collections are configured to utilize.

This repository will only host the last 3 major versions of Secret Server, previous versions can be found by looking at the Git history through GitHub if needed.

## Visualize

Each collection includes a JavaScript that will **attempt to** parse the `records` object (if the endpoint returns one) and build a formatted table to view the data:

<img src="https://user-images.githubusercontent.com/11204251/104269730-99dc2d00-545c-11eb-97f5-3026be12e662.png" width="633" height="260">

## Setup

1. Clone or download this repository to your device.
1. Open [Postman](https://www.getpostman.com/) on your device.
1. Click **File | Import ...**.
1. Click the Upload Files button.
1. Hold `CTRL` key and click on environment file and the desired collections.
1. Click **Import** button.

You can view a recording of the above steps [here](secretserver_postman_setup.mp4).

> Newer versions of Postman starting with version 8 allow you to import the full repository into Postman. You will need to fork this repository to your GitHub account for that to work.

## Troubleshooting Postman

If you are using this collection against your internal or local Secret Server lab you may see an initial error like this when you try to retrieve an access token:

<img src="https://user-images.githubusercontent.com/11204251/104262762-dce2d400-544d-11eb-8a1d-eb7f339b6e29.png" width="521" height="308">

If you show the Postman console (`ATL + CTRL + C` or _View | Show Postman Console_) you will see this message to indicate the SSL certificate for your web service cannot be validated:

<img src="https://user-images.githubusercontent.com/11204251/104262838-03087400-544e-11eb-80da-c5769aa11a0c.png" width="687" height="182">

To fix this you need to go into your settings for Postman (`CTRL + comma` or _File | Settings_) and toggle off the setting **SSL certificate verification**.

<img src="https://user-images.githubusercontent.com/11204251/104262900-26332380-544e-11eb-9c16-64c6678c1497.png" width="618" height="457">

# Disclaimer

The content (scripts, documentation, examples) included in this repository is not supported under any Thycotic standard support program, agreement, or service. The code is provided AS IS without warranty of any kind. Thycotic further disclaims all implied warranties, including, without limitation, any implied warranties of merchantability or fitness for a particular purpose. The entire risk arising out of the code and content's use or performance remains with you. In no event shall Thycotic, its authors, or anyone else involved in the creation, production, or delivery of the content be liable for any damages whatsoever (including, without limitation, damages for loss of business profits, business interruption, loss of business information, or other pecuniary loss) arising out of the use of or inability to use the code or content, even if Thycotic has been advised of the possibility of such damages.
