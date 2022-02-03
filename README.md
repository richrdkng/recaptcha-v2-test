# Simple Google reCAPTCHA v2 Test

A simple website to test basic [reCAPTCHA v2][url-recaptcha] functionality with callbacks.

## :coffee: Usage

To handle possible [reCAPTCHA v2 events][url-recaptcha-tags], override one or more of the following in [index.html][url-index-html]:

```javascript
// fired, when the reCAPTCHA is loaded (onload URL parameter)
function onCaptchaLoad() {
    console.log('onCaptchaLoad')
}
```

```javascript
// fired, when the user submits a successful reCAPTCHA response (data-callback attribute)
function onCaptchaSuccess(token) {
    console.log('onCaptchaSuccess', token)
}
```

```javascript
// fired, when the reCAPTCHA response expires and the user needs to re-verify (data-expired-callback attribute)
function onCaptchaExpired() {
    console.log('onCaptchaExpired')
}
```

```javascript
// fired, when the reCAPTCHA encounters an error (data-error-callback attribute)
function onCaptchaError() {
    console.log('onCaptchaError')
}
```

## :beers: Contribution

Any contribution is **highly** appreciated. **Thank you in advance** and have fun!

## :copyright: License

[MIT][url-license] @ [Richard King][url-github]

<!--- URLs -------------------------------------------------------------------->
[url-recaptcha]:      https://developers.google.com/recaptcha/docs/display
[url-recaptcha-tags]: https://developers.google.com/recaptcha/docs/display#render_param
[url-index-html]:     https://github.com/richrdkng/recaptcha-test/blob/main/index.html
[url-github]:         https://github.com/richrdkng
[url-license]:        https://github.com/richrdkng/recaptcha-test/blob/master/README.md
