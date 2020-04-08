# Kandy Link Anonymous Android SDK

<p>
    <img alt="GitHub release" src="https://img.shields.io/github/v/release/kandy-io/kandy-anonymous-android-sdk">
</p>

## Installation
To integrate Kandy Link Anonymous Android SDK to your project add gradle dependencies as described below.

### Step 1
Add Kandy Link Anonymous Android SDK maven repository url to your root level `build.gradle` file.

```
allprojects {
  ...
  repositories {
    ...
    maven {
      url "https://raw.githubusercontent.com/Kandy-IO/kandy-anonymous-android-sdk/master/dist/"
    }
  }
}
```

### Step 2
Add dependency of Kandy Link Anonymous Android SDK to your app level `build.gradle` file.

```
implementation 'com.kandy.mobile:kandyanonymousmobilesdk:5.5.0'
```

That's all! You can use Kandy Link Anonymous Android SDK after you sync gradle.

## Installation for versions before 5.0.0
Versions before 5.0.0 will require manual installation. To download an older version, switch to tag of that specific version. Then download the MobileSDKAnonymous-4.x.x.zip file under "dist" directory.

## Compatibility
Compatible Android OS versions :

* Android 4.1+ - Android 10.0

Tested on :

* Nexus 5, Samsung Note 3, Samsung Note 5, Samsung S7, LG G2, LG G3, LG G5, LG G6, HTC Desire 626, HTC One A9, HTC 10, SONY XPERIA Z5, SONY XPERIA XZ, General Mobile GM 5+

Compatible KandyLink Server versions :

* Kandy Link 4.6.1

* Kandy Link 4.7.0 + Patch 4

## Reference

The information about tutorials and documents can be found in the links below

* `Documents`: [API Docs](https://kandy-io.github.io/kandy-anonymous-android-sdk/docs)

* `Tutorials`: Choose your configuration ( [Kandy-US](https://kandy-io.github.io/kandy-anonymous-android-sdk/tutorials/?SUBSCRIPTIONFQDN=spidr-ucc.genband.com&WEBSOCKETFQDN=spidr-ucc.genband.com&ICESERVER1=turn-ucc-1.genband.com&ICESERVER2=turn-ucc-2.genband.com) | [Kandy-EMEA](https://kandy-io.github.io/kandy-anonymous-android-sdk/tutorials/?SUBSCRIPTIONFQDN=spidr-em.genband.com&WEBSOCKETFQDN=spidr-em.genband.com&ICESERVER1=turn-em-1.genband.com&ICESERVER2=turn-em-2.genband.com) | [Kandy-UAE](https://kandy-io.github.io/kandy-anonymous-android-sdk/tutorials/?SUBSCRIPTIONFQDN=ct-webrtc.etisalat.ae&WEBSOCKETFQDN=ct-webrtc.etisalat.ae&ICESERVER1=ct-turn1.etisalat.ae&ICESERVER2=ct-turn2.etisalat.ae) )
