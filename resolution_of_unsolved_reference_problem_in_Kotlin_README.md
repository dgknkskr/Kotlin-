# Kotlin-
//Hi, if you have also like such a problem in Android Studio, Your problem will solve by adding kotlin as follow

// Problem example in below


    class MainActivity : AppCompatActivity() {

        override fun onCreate(savedInstanceState: Bundle?) {

            super.onCreate(savedInstanceState)

            setContentView(R.layout.activity_main)
        }
        fun plus_button(view: View){

        var num1 = editText.text  // editText shown as red
                                  // I created editText in Design-Side(Android Studio) however Console is showing " editText is unresolved reference".And then I can // not use this textbox in my codes.
    }
}

// Solution:

// open the " build.gradle " file in app file(on the left side in android studio, under the test file) You're just adding 2 blocks of code.

// 1- Write two codes i gave below in build.gradle(app)

// 2- go to Terminal and write " grandle idea " and click enter

// 3- Then click to " sync now " in notification shown 


//FOR KOTLİN

    plugins {

        id 'com.android.application'

        id 'kotlin-android'

        id 'kotlin-android-extensions'  // add this here***
        }

    android {
    ...
    }

    dependencies {
    ...
    
    }

    apply plugin: 'idea'    // add this here***


// Come to editText(example) and click on it and click " import this "

// Problem solved.

------------------------------------------------------------------------


//FOR JAVA 

    apply plugin: 'com.android.application'

    apply plugin: 'kotlin-android' 
    
    apply plugin: 'kotlin-android-extensions' // add this here***

    android {
    ...
    }

    dependencies {
    ...
    }
    apply plugin: 'idea' // add this here***

// Come to editText(example) and click on it and click " import this "

// Problem solved.




