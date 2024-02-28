---------------
28 February 2024
---------------
Hotfix Release with following fixes:
- Fixed Scrolling Lags
- Fixed sms/otp issue that has been bugging us since longgg

---------------
27 February 2024
---------------
- Based on HyperOS firmware
- Added 90Hz support
- Added double tap to fingerprint feature
- Ships with Evenstar Kernel non-ksu variant
- Dropped support for 32 bit apps for now
- Added overlay for Turbo Power Charging
- Optimized Dex flags (faster boot)
- Removed Force triple frame buffers (Reduces app lags & improves UI performance)
- Tweaked surface flinger flags (Improves QS animation, app opening & app switching)
- Added props to Optimize Touch and Improve animations
- Nuked Per-app Refresh Rate for now (Buggy after update to Hyperos Blobs)
- Set Brightness slider curve Implementation (Enjoy higher brightness at lower slider positions; U can set brightness slider to 10% if u were previously setting it to 40% and still enjoy same>
- Moved Fuse Passthrough prop to product.prop from system.prop as per latest android change
- Fixed Battery Drain due to statsd
- Updated BCR app to latest 1.6
- Updated ViperFX to latest 6.1
