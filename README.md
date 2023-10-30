# jarvis
This is a Kotlin/Android Studio Jarvis Assistant integration with GPT4 API and Porcupine service integration

CAPABILITIES: You should be able to activate the app by using your "Wake Word" from porcupine services

Critical Dependencies on your build.gradle file you need to make this work: All of the versions on these might change by the time you view this code.

implementation("androidx.core:core-ktx:1.12.0")
    implementation("androidx.appcompat:appcompat:1.6.1")
    implementation("com.google.android.material:material:1.10.0")
    implementation("androidx.constraintlayout:constraintlayout:2.1.4")
    testImplementation("junit:junit:4.13.2")
    androidTestImplementation("androidx.test.ext:junit:1.1.5")
    androidTestImplementation("androidx.test.espresso:espresso-core:3.5.1")

    implementation ("org.jetbrains.kotlinx:kotlinx-coroutines-core:1.6.4")
    implementation ("org.jetbrains.kotlinx:kotlinx-coroutines-android:1.6.4")

    implementation ("ai.picovoice:porcupine-android:3.0.0")
    implementation ("com.squareup.okhttp3:okhttp:4.9.1")
    implementation ("com.squareup.okhttp3:logging-interceptor:4.9.1")

    Make sure that you are using targetSDK: 33-34 but nothing lower
    Create a new Device that has the target API

    Make sure to limit the Tokens you'll be using.

    FOR ANDROID:
    Check your settings if the Default assitant is using Google Voice and the Native language should be english
