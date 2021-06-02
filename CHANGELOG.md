# Change Log

Kandy Link Anonymous Android SDK change log.

- This project adheres to [Semantic Versioning](http://semver.org/).
- This change log follows [keepachangelog.com](http://keepachangelog.com/) recommendations.

## 5.19.0 - 2021-06-01

## 5.18.0 - 2021-04-26

## 5.17.0 - 2021-03-26

## 5.16.0 - 2021-02-26

### Removed
- `registerToServer(final Constants.SubscribeServices[] serviceTypes, final int expirationTime, final OnCompletionListener listener)` was removed.

## 5.15.0 - 2021-02-04

### Deprecated
- `isRingingFeedbackEnabled` and `setRingingFeedbackEnabled` added to Configuration class methods are deprecated and will be removed in future releases. Instead `ringingFeedbackOptions` and `setRingingFeedbackOptions` should be used. 

## 5.14.0 - 2020-12-30

### Deprecated
- `DTLS`, `securedWSProtocol`, `requestProtocolHttp`, `kandyVersion`, `kandyToken`, `deviceId`, `deviceNativeId`, `sendKandyTokenInRestHeader`, `connectionType`, `auditEnable`, `supportedCallFeautes`, `notificationType` parameters removed from Configuration class. `KAE-869`

### Added
- `isRingingFeedbackEnabled` and `setRingingFeedbackEnabled` added to Configuration class in order to set and/or check ringing feedback feature.

### Renamed
- `replaceCodecSet` parameter renamed as `codecPayloadTypeSet` in Configuration class. `KAE-869`

## 5.13.0 - 2020-12-02

### Fixed
- Crash when the application native dial pad is used is fixed. `KAE-865`

## 5.12.0 - 2020-11-04

## 5.11.0 - 2020-10-05

### Changed
- Return type of `CallInterface.getRTPStatistics` was changed as `NSString`

## 5.10.0 - 2020-08-28

## 5.9.0 - 2020-07-22

## 5.8.0 - 2020-07-03

## 5.7.0 - 2020-06-12

## 5.6.0 - 2020-05-04

### Fixed
- After Session Complete notification the end call DELETE request must be sent. `KAE-669`

## 5.5.0 - 2020-03-30

## 5.4.0 - 2020-03-02

### Added
- Adding configuration property for control TCP keep alive `KAE-571`

## 5.3.0 - 2020-01-09

### Fixed
- Fixed internal error handling issue during anonymous (un)subscription  `KAE-574`


## 5.2.0 - 2019-12-02

### Added
- WebRTC stack upgraded to version M78 `KAE-507`
- Custom Kandy Agent HTTP Header is implemented `KAE-524`
- Anonymous SDK APIs are separeted from Regular SDK API module. Features that are not used in Anonymous SDK (like call transfer) will not be included in Anonymous API stack. `KAE-504`

### Deprecated
- `CallService.createOutgoingCall(String, CallApplicationListener, OutgoingCallCreateInterface)`, `CallService.createOutgoingCall(String, String, String, CallApplicationListener, OutgoingCallCreateInterface)` and `CallService.createOutgoingCall(String, String, String, String, CallApplicationListener, OutgoingCallCreateInterface)` methods are deprecated and will be removed in future releases, since `CallApplicationListener` can already be set to CallService via a setter method. Instead `CallService.createOutgoingCall(String, OutgoingCallCreationCallback)`, `CallService.createOutgoingCall(String, String, String, OutgoingCallCreationCallback)` and `CallService.createOutgoingCall(String, String, String, String, OutgoingCallCreateInterface)` should be used.


## 5.1.0 - 2019-11-04

### Fixed
- Single m-line audio call issue is fixed `KAE-527`
- Default value for codec preferrence is set to reflect WebRTC default codec behavior `KAE-538`


## 5.0.0 - 2019-10-03

### Added
- Unified Plan Support `KAE-200`
- Mobile SDK Distribution on Maven `KAE-425`
- Support Custom SIP headers in Incoming Call `KAE-447`
- Callee Name api added to CallInterface `KAE-475`


## 4.6.2 - 2019-09-02

### Fixed
- Media problem when switching between two calls on Music-on-Hold is fixed `KAE-410`


## 4.6.1.1 - 2019-08-05


## 4.6.1 - 2019-07-05

### Added
- Bandwidth limitation feature implemented `KAE-63`

### Fixed
- A fix provided for race condition case during WebRTC audio module creation when a second call session is being initiated. `KAE-435`


## 4.6.0 - 2019-06-01

### Fixed
- HTTP 4xx and 5xx responses are coded with a new error code and reported with MobileError. `KAE-288`


## 4.5.9.1 - 2019-05-06

### Fixed
- Hardware support of "Acoustic Echo Canceler" and "Noise Suppressor" configuration is fixed `KAE-369`


## 4.5.9 - 2019-05-02

### Added
- Time-Limited Token Based Anonymous Call feature implemented `KAE-284`

### Changed
- Package name for VideoView is changed to "com.genband.mobile.core.webrtc.view". `KAE-368`
