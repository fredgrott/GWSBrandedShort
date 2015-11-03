GWSBrandedShort
===============

A library that you can use to do launch screens for your android java application.


Usage
=====

I use jitpack to upload my libraries so you put this in your root buildscript:

```groovy
allprojects {
        repositories {
            jcenter()
            maven { url "https://jitpack.io" }
        }
   }
```
Than in the module buildscript:


```groovy
compile 'com.github.shareme:GWSBrandedShort:{latest-release-number}@aar'
```

Create an drawable-xhdpi res folder and place banded png image there and name it branded.png.

In your Android Manifest:

```xml
<application
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:theme="@style/AppTheme" >
        <activity
            android:name=".MainActivity"
            android:label="@string/app_name"
            android:theme="@style/AppTheme.BrandedLaunch">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

```

and your layout activity can be something like:

```xml
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"
             xmlns:tools="http://schemas.android.com/tools"
             android:layout_width="match_parent"
             android:layout_height="match_parent"
             android:paddingBottom="@dimen/activity_vertical_margin"
             android:paddingLeft="@dimen/activity_horizontal_margin"
             android:paddingRight="@dimen/activity_horizontal_margin"
             android:paddingTop="@dimen/activity_vertical_margin"
             tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:text="@string/hello_world"
        android:textAllCaps="true"
        android:textAppearance="@style/TextAppearance.AppCompat.Display1"/>

</FrameLayout>

```

Remember that you want the style AppTheme from the library to be applied. Depending upon how complex
your application maybe and your res merge rules that you set up you might have to delete the
default AppTheme in the res/values/styles.xml file in your application res.

Target Android API Range
========================

Api 16 to api 23.


Credits
========

Fred Grott(aka shareme  GrottWorkShop)
[MyGithubProfile](https://github.com/shareme/MyGithubProfile)

Former JavaME and JavaEE developer that made the transition to Android Native java Application Development.
Multi-computer-language polyglot that can jump into anything and I do not play follow-the-leader but
often follow my own unique way.(No recruiters, please for any reason)

[Github profile](https://github.com/shareme)
[Bitbucket profile](https://bitbucket.org/fredgrott)
[G+ profile](https://plus.google.com/u/0/+FredGrott/about)
[Twitter profile](https://twitter.com/fredgrott)
[Facebook profile](http://www.facebook.com/fredgrott)
[DeviantArt profile](http://shareme.deviantart.com)
[BeHance profile](https://www.behance.net/gwsfredgrott)
[Dribbble profile](https://dribbble.com/FredGrott)
[AngelList profile](https://angel.co/fred-grott)
[BuiltINChicago profile](http://www.builtinchicago.org/member/fred-grott)
[HackerNews profile](https://news.ycombinator.com/user?id=fredgrott)
[Geeklist profile](https://geekli.st/fredgrott)
[Medium profile](https://medium.com/@fredgrott)
[StackOverflow profile](http://stackoverflow.com/users/237740/fred-grott)
[Blogger blog](http://grottworkshop.blogspot.com)
[Reddit profile](http://www.reddit.com./user/fredgrott/)
[Quora profile](http://www.quora.com/Fred-Grott)
[YouTube channel](https://www.youtube.com/c/FredGrott?gvnc=1)
[AboutMe profile](https://about.me/fredgrott)
[LinkedIN profile](http://www.linkedin.com/in/shareme/en)
[Xing profile](https://www.xing.com/profile/Fred_Grott?sc_o=mxb_p)
[SlideShare profile](http://www.slideshare.net/shareme)
[SpeakerDeck profile](https://speakerdeck.com/fredgrott)
[Android Hacker Tumbler](https://www.tumblr.com/blog/androidhacker)
[Ustream](https://www.ustream.tv/manage-show/12940149)
[AboutMe](https://about.me/fredgrott)



License
=======

[Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.txt)

Resources
=========

[Google Android Developer Site](http://developer.android.com)

[Google Android Developer Tool Site](http://tools.android.com)

[Google Android Developer Blog](http://android-developers.blogspot.com/)


[StackOverflow Android Questions](http://stackoverflow.com/questions/tagged/android)

[Gradle](http://gradle.org)

[Reddit-androidev](http://reddit.com/r/androdev/)

[AndroidChat at Slack](https://androidchat.slack.com/messages/development/)

[Amazon Android Dev Site](https://developer.amazon.com/public)

[JavaRanch Android Forum](http://www.coderanch.com/forums/f-93/Android)

[Android Development Tools G+ community](https://plus.google.com/communities/114791428968349268860)

[Android Development G+ Community](https://plus.google.com/communities/105153134372062985968)

[Android Developers G+ Community](https://plus.google.com/+AndroidDevelopers/posts)

[Android Design G+ Community](https://plus.google.com/communities/113499773637471211070)

[UX Design for Developers](https://plus.google.com/communities/103651070366324568638)

[Android MVP G+ Community](https://plus.google.com/communities/114285790907815804707)
