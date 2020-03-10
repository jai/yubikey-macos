**TODO: Test with multiple YubiKeys**

## Instructions on forcing YubiKey login for macOS

Note that after you complete these instructions, you will not be able to use your password to log in to your user account on macOS!

### Pair YubiKey as a smart card with your macOS login

- Enable PIV on YubiKey using YubiKey Manager: [https://developers.yubico.com/PIV/Guides/Device_setup.html](https://developers.yubico.com/PIV/Guides/Device_setup.html)
- Pair the YubiKey with the desired macOS user account by removing and re-inserting the YubiKey.

### Test smart card login

Test to ensure that smart card login works (log out, and try to log in with YubiKey + PIN). Your regular password should still work (remove YubiKey to log in with your password).

### Disable password (enforce smart card-only login)

Configure macOS for smartcard-only authentication: [https://support.apple.com/en-us/HT208372](https://support.apple.com/en-us/HT208372) by installing this the latest version of the profile from this repository: [https://github.com/jai/yubikey-macos](https://github.com/jai/yubikey-macos)