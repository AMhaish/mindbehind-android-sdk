# MindBehind

This repo contains the built version for the Android SDK and instruction on how to use it.

The structure for the repo is as follows:

| Filename        | Description                                               |
|-----------------|-----------------------------------------------------------|
| build           | Contains the ready to distribute binaries                 |
| build/docs      | API reference documentation in javadoc.jar format         |
| README          | This guide                                                |

# Using the pre-built aar

To use the pre-built aar in your own application, follow the steps below to add it as a dependency in your Android app.

1. Import `core-1.0.0.aar` and `ui-1.0.0.aar` from the `build` directory into your Android Studio project by going to `File -> New -> New Module -> Import .JAR/.AAR`.
1. In your project's `build.gradle` file add the following lines:
    ```gradle
    implementation project(':core-1.0.0')

    implementation 'com.google.firebase:firebase-messaging:18.0.0'
    implementation 'com.google.code.gson:gson:2.8.6'
    implementation 'com.squareup.okhttp3:okhttp:3.12.6'
    implementation 'com.squareup.retrofit2:retrofit:2.6.2'
    implementation 'com.squareup.retrofit2:converter-gson:2.6.2'
    implementation 'com.google.dagger:dagger:2.25.2'
    implementation 'com.android.support:support-annotations:28.0.0'

    annotationProcessor 'com.google.dagger:dagger-compiler:2.25.2'

    implementation project(':ui-1.0.0')

    implementation 'com.github.bumptech.glide:glide:4.9.0'
    implementation 'com.android.support:support-v4:28.0.0'
    implementation 'com.android.support:appcompat-v7:28.0.0'
    implementation 'com.android.support:exifinterface:28.0.0'
    implementation 'com.android.support:recyclerview-v7:28.0.0'
    implementation 'com.android.support:support-media-compat:28.0.0'
    implementation 'com.google.android.gms:play-services-location:16.0.0'
    implementation 'com.davemorrissey.labs:subsampling-scale-image-view:3.10.0'
    ```

You should now be able to import the libraries (`import com.mindbehind.core`, `import com.mindbehind.ui`) and start using them in your code.

# Version

This is version 1.0.0 of MindBehind.
