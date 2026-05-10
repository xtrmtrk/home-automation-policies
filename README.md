# home-automation-policies

Policies and SMS consent registration page for the private Hubitat home automation notification system.

## Live pages

- Home: https://xtrmtrk.github.io/home-automation-policies/
- Registration: https://xtrmtrk.github.io/home-automation-policies/SignUp.html
- Privacy Policy: https://xtrmtrk.github.io/home-automation-policies/privacy.html
- Terms and Conditions: https://xtrmtrk.github.io/home-automation-policies/terms.html

## Google Apps Script setup

Create a Google Sheet named `Home Automation SMS Registrations` with a tab named `Registrations` and these headers:

```text
Timestamp, Name, Phone, Email, Consent, Consent Text, Page URL, Client Timestamp
```

Paste `SignUp.js` into Extensions -> Apps Script, deploy it as a Web App, then replace the placeholder `REGISTRATION_ENDPOINT` value in `SignUp.html` with the deployed Web App URL.
