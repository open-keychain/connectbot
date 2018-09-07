[![Build Status](https://travis-ci.org/connectbot/connectbot.svg?branch=master)](
https://travis-ci.org/connectbot/connectbot)

Special version of ConnectBot that supports the SSH Authentication API. In combination with OpenKeychain it can use OpenPGP keys.

This is primarily developed to support authentication subkeys on smart cards and other security tokens over NFC and USB.

[<img src="https://f-droid.org/badge/get-it-on.png"
      alt="Get it on F-Droid"
      height="80">](https://f-droid.org/packages/org.sufficientlysecure.termbot/)
[<img src="https://play.google.com/intl/en_us/badges/images/generic/en-play-badge.png"
      alt="Get it on Google Play"
      height="80">](https://play.google.com/store/apps/details?id=org.sufficientlysecure.termbot)

Screenshots
----------------
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/hostlist.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/select_pubkey_auth_via_agent.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/select_agent.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/allow_access.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/select_key.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/key_selection_successful.png" width="256">

<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/token_enter_pass.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/token_pin.png" width="256">
<img align=left src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/token_hold.png" width="256">
<img src="https://github.com/open-keychain/connectbot/blob/agent_support_plus/screenshots/token_done.png" width="256">


Translations
----------------

If you'd like to see ConnectBot/TermBot translated into your language and
you're willing to help, then head on over to
https://translations.launchpad.net/connectbot/trunk/+pots/fortune


Compiling
----------------

To compile TermBot using gradlew, you must first specify where your
Android SDK is via the ANDROID_SDK_HOME environment variable.

To run the Jenkins CI pipeline locally, you can use
`jenkinsfile-runner` which can be invoked like this:

```sh
docker run -it -v $(pwd):/workspace \
    -v jenkinsfile-runner-cache:/var/jenkinsfile-runner-cache \
    -v jenkinsfile-runner:/var/jenkinsfile-runner \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -v $(which docker):$(which docker) \
    jenkins/jenkinsfile-runner
```
