# NodeBB Kakao SSO

NodeBB Plugin that allows users to login/register via their Kakao account.

## Installation

    npm install nodebb-plugin-sso-kakao

## Configuration

1. Create a **New Application** via the [KAKAO Developers](https://developers.kakao.com/console/app)
1. From the "Credentials" page, create a new "OAuth Client ID".
    * The "Application Type" is "Web application"
    * "Authorized Javascript origins" can be left empty
    * The "Authorised Redirect URI" is your NodeBB's URL with `/auth/kakao/callback` appended to it.
        * When you enter this value into the text field, be sure to hit <code>Enter</code> to submit the URL before saving
1. You will be shown a screen containing your **Client ID** and **Client Secret**. Paste those two values into this plugin's configuration page.
1. Save, rebuild your NodeBB assets (<code>./nodebb build</code>), and restart your NodeBB.