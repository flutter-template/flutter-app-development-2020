#All about of Flutter App Development 2020
===============================================


CONTENTS

-   [What is Flutter exactly?](#what-is-flutter-exactly)
-   [Pros of Flutter development](#pros-of-flutter-development)
    -   [+ Ready-made and custom widgets for fast UI
        coding](#ready-made-and-custom-widgets-for-fast-ui-coding)
    -   [+ The mildest learning curve and a growing
        community](#the-mildest-learning-curve-and-a-growing-community)
    -   [+ Dart – simple and effective language targeted at Java
        programmers](#dart---simple-and-effective-language-targeted-at-java-programmers)
    -   [+ Hot reload function for instantaneous
        updates](#hot-reload-function-for-instantaneous-updates)
    -   [+ Portability](#portability)
    -   [+ Internationalization and
        accessibility](#internationalization-and-accessibility)
    -   [+ High performance](#high-performance)
-   [Cons of Flutter development](#cons-of-flutter-development)
    -   [– Lack of third-party
        libraries](#--lack-of-third-party-libraries)
    -   [– Dart, again](#--dart-again)
    -   [– Large file size](#--large-file-size)
    -   [– Issues with iOS](#--issues-with-ios)
-   [How to get started with Flutter](#how-to-get-started-with-flutter)
-   [Will Flutter replace React Native and
    Xamarin?](#will-flutter-replace-react-native-and-xamarin)

Reading time: 11 minutes

Without knowing it, you’ve probably already used the apps made with
Flutter. Whether you shopped on Alibaba, ran an ad campaign on Google
Ads, or used a digital coupon, you’ve likely witnessed the results of
Flutter’s still short history.

The product has remained beta for a long time. Now, with its [Release
Preview
2](https://developers.googleblog.com/2018/09/flutter-release-preview-2-pixel-perfect.html)
version, it finally stepped on the finish line before the initial 1.0
release. We understand the hesitation and excitement of the new,
transformative technology for developers, so here’s our overview of the
best and the worst of  Flutter – and what you can do with it.

The first question about Flutter you might have is “How is it
different?” If you’re familiar with hybrid and cross-platform
development, it’s valid to question how Flutter can be better than Xamarin, React
Native, or Ionic, for that matter. What’s the point of switching? As we had no
intention of promoting Flutter over other technologies, we decided to
figure out why you should be excited about the product – and what to be
wary of.

What is Flutter exactly?
------------------------

Flutter is Google’s new open source technology for creating native
Android and iOS apps with a single codebase. Unlike other popular
solutions, Flutter is not a framework; it’s a complete SDK – software
development kit – which already contains everything you will need to
build cross-platform applications. This includes a rendering engine,
ready-made widgets, testing and integration APIs, and command-line
tools.

Similar technologies such as Xamarin, React Native, Ionic, or
NativeScript all try to achieve platform nativeness via different
approaches.
Now, let’s see what Flutter introduces to the game.

Flutter follows the **reactive development architecture**, but with a
twist. The main thing to know about reactive programming is that it
updates UI contents automatically when you update the variables in the
code. React Native also follows this principle, but it uses the
JavaScript bridge to access OEM widgets. But since the app has to pass
this bridge to access widgets each time, it causes performance issues.
Flutter, however, omits this bridge altogether and communicates with the
native platform using Dart.

**Dart** is Flutter’s object-oriented language that uses Ahead-of-Time
compilation techniques and compiles into native code without that
additional bridge. This noticeably speeds up the app startup time.
Besides, Flutter doesn’t have to call to OEM (original equipment
manufacturer) widgets, because it uses its own. As seen on the image
below, Flutter uses the OS as a canvas to build an interface on and
moves services such as gestures, rendering, and animations into the
framework itself, which gives developers complete control over the
system.

![Reactive web
frameworks](https://content.altexsoft.com/media/2018/11/reactive-frameworks.png)

![Reactive web
frameworks](https://content.altexsoft.com/media/2018/11/reactive-frameworks.png)

![Flutter
architecture](https://content.altexsoft.com/media/2018/11/flutter.png)

![Flutter
architecture](https://content.altexsoft.com/media/2018/11/flutter.png)

*Reactive frameworks vs Flutter\
**Source: [Wm Leler on
Medium](https://hackernoon.com/whats-revolutionary-about-flutter-946915b09514)*

**Debugging** in Flutter also happens thanks to Dart. Dart Analyzer and
Dart Observatory tools help find errors using specific commands. The
process is explained in detail in [Flutter debug
docs](https://flutter.io/docs/testing/debugging). Another method
includes using Flutter-supported IDEs and their specific debuggers.
Since Flutter doesn’t use WebView it can’t be debugged directly in a
browser like Ionic. React Native and NativeScript allow for testing via
Chrome Developer Tools. However, considering that these products often
prefer third-party solutions for debugging anyway, Flutter’s process
shouldn’t appear very different.

Since Flutter is a full-fledged SDK, it already offers an automated
testing toolset, specifically, for three types of tests: unit test,
widget test, and integration test. You can find Google’s tutorials for
those tests [at this link](https://flutter.io/docs/testing). Flutter
also supports the model via [fastlane](https://docs.fastlane.tools/), a free tool that
bridges Flutter with Travis, Jenkins, or Cirrus.

Pros of Flutter development
---------------------------

What’s innovative, different, and simply better executed about Flutter?
Let’s review the features that will make you consider abandoning React
Native for a new tool.

### + Ready-made and custom widgets for fast UI coding

Previously we mentioned that Flutter uses ready-made widgets. You could
even say that Flutter *is* widgets. One of the revolutionary things
about the product is how it helps create a user interface utilizing
these building blocks. Compare that to other approaches that use
different objects (layouts, views, controllers), when Flutter has a
consistent and unified object model.

Any object in Flutter is a widget, from a button to padding or a font.
Widgets can be combined to create layouts, and you can choose to use
widgets on any level of customization – from existing building blocks to
the lowest level when you create your own widgets with the same tools
the Flutter team did theirs.

Widgets in Flutter are organized in trees, which is handy for rendering,
but may result in an excessive complication of the whole structure.
Large applications may require up to 10 layers of code to create a basic
object, so you’ll have to plan the structure ahead.

![flutter
widget](https://content.altexsoft.com/media/2018/11/inspector_select_example-fb6507f3f20614013165f91a3e4fc18036af153e6136a98d46aee59c7ca06dbe.gif)

![flutter
widget](https://content.altexsoft.com/media/2018/11/inspector_select_example-fb6507f3f20614013165f91a3e4fc18036af153e6136a98d46aee59c7ca06dbe.gif)

*Flutter widget tree*

The fact that Flutter has its own widgets gives you one big advantage:
Flutter already provides widgets that perfectly follow [Material
Design](https://flutter.io/docs/reference/widgets/material) and Apple’s
[Cupertino](https://flutter.io/docs/reference/widgets/cupertino) looks.
The UI customization that usually takes the longest to finish in
cross-platform development takes a minimum amount of time with Flutter.

### + The mildest learning curve and a growing community

Given that getting used to Dart is not a massive problem to you,
learning the tool itself should be easy. The Flutter team notes that
they’ve seen people with very limited programming knowledge prototyping
and building apps, and also mentions that no mobile development
experience is required to start with Flutter.

Besides, Google is known for creating detailed and well-structured
documentation, something that React Native struggles
with.
Apart from classic [docs](https://flutter.io/docs), you can watch [video
lessons](https://www.youtube.com/playlist?list=PLOU2XLYxmsIJ7dsVN4iRuA7BT8XHzGtCr)
from the Google team, and go through practical exercises on
[Codelabs](https://codelabs.developers.google.com/?cat=Flutter). And
these are just the resources provided officially. You can find courses
on Udemy and Udacity, join Facebook communities, and even a [study group
on Slack](https://flutterstudygroup.slack.com/).

For such a young technology, Flutter is growing very fast. This graph
shows the interest in Flutter on StackOverflow prior to the Release
Preview 2 launch in comparison with other front-end frameworks. Despite
still being in beta stage, the tool is production-ready which has only
piqued the crowd’s interest. It’s available for commercial use and has
already been successfully implemented in enterprises, medium-sized
agencies, and startups.

![StackOverflow question
views](https://content.altexsoft.com/media/2018/11/pasted-image-0-13image4.png)

![StackOverflow question
views](https://content.altexsoft.com/media/2018/11/pasted-image-0-13image4.png)

*Number of StackOverflow question views\
**Source: [Google Developers
blog](https://developers.googleblog.com/2018/09/flutter-release-preview-2-pixel-perfect.html)*

### + Dart – simple and effective language targeted at Java programmers {#dart---simple-and-effective-language-targeted-at-java-programmers}

[Dart](https://www.dartlang.org/) is a modern object-oriented language
that will remind you of
Java or C++ with its syntax. It supports both [strong and weak typing
styles](https://www.wikiwand.com/en/Strong_and_weak_typing) making it
easy to pick up for beginners. Above, we mentioned that Dart is
responsible for some of the crucial things about Flutter. Let’s analyze
what about Dart’s nature makes Flutter… well, Flutter.

**Both AOT and JIT compilation types.** In development, engineers
usually have to opt for the compilation their programming language
provides. Programs compiled Ahead-of-Time usually run faster because
they’ve been compiled before. However, in this case, the development
itself slows a lot. Just-in-Time compilation results in faster
development cycles, but, predictably, affects the app startup speed
since the compiler does its analyzing before code execution. Flutter
takes the best of both worlds by using JIT compilation during
development and switching to AOT for app release.

**No need for XML files.** In Android development, the work is separated
into layout and code. The layout should be written in XML as Views that
are then referenced in the Java code. Dart takes care of that by keeping
layout and code in one place. Since everything in Flutter is a widget,
the layout is also created in Dart.

**Better performance without a JavaScript bridge.** As you already know,
the app on a user’s device will run smoothly because Dart compiles into
native code directly, without the bridge.

While we’re talking about Dart benefits, it’s worth mentioning that the
language isn’t limited to mobile development – it’s also used for
building web apps, and by Google no less. It’s commonly used in
combination with web frameworks,
[AngularDart](https://webdev.dartlang.org/angular) being Google’s own
choice for some of its services.

### + Hot reload function for instantaneous updates

This tool is already engraved into Flutter’s architecture and doesn’t
require any plugins to work. Hot reloading basically allows you to see
updates in real time. Imagine you’ve encountered an error while running
a program. In Flutter, you can fix it right away, continuing from where
you left off, without restarting the whole thing. Going back to regular
programming where deployment takes several minutes may be a struggle.
Hot reload elevates programmers’ productivity, helps with quick
iterations, and allows you to experiment without long delays. Xamarin
and React Native have the equivalents of this feature too, but some
reviews claim that it’s much faster in Flutter. We’ve yet to see
benchmarks for proof of that.

![](https://content.altexsoft.com/media/2018/11/UIChange.gif)

![](https://content.altexsoft.com/media/2018/11/UIChange.gif)

*Changing app UI with Hot Reload\
 Source: *[*BuildFlutter*](https://buildflutter.com/hot-reloading/)

### + Portability

Since Flutter is not just a framework but a complete SDK, it can run on
virtually any device with a screen. Third-party ports have been created
to build [Flutter apps for Mac OS, Windows, and
Linux](https://github.com/google/flutter-desktop-embedding). They
include embedding APIs, mouse and keyboard input functions, and
different plugins. Some people even [tried to build TV
applications](https://www.youtube.com/watch?v=crODae5bIew) using
Flutter. Considering the possibilities and Google’s fondness for IoT
devices, it’s fair to expect that this functionality will become
official in the future.

### + Internationalization and accessibility

Being an advocate for diversity and inclusivity, Google provides
built-in opportunities to make your apps accessible to a wider range of
users. Usually, when you want your app to run in different languages and
be used in different regions, you need to prepare your code so it’s
ready for localized content which is typically created later. This
process is called internationalization.

Flutter natively provides widgets based on the [Dart intl
package](https://pub.dartlang.org/packages/intl) that simplifies this
process. Today it supports 24 languages, but also currencies, units of
measure, dates, layout options (for languages written from right to
left), and more.

Flutter also ensures web accessibility
and supports these three components:

-   Large fonts – adjusts font sizes to the ones a user specified in OS
    settings
-   Screen readers – provides spoken feedback on UI elements
-   Sufficient contrast – makes text easier to read

While all this is automated, developers should also test their designs
for different settings. For instance, they can use the largest font
setting to see how it fits in a small mobile screen.

![font
settings](https://content.altexsoft.com/media/2018/11/Screenshot_1.png)

![font
settings](https://content.altexsoft.com/media/2018/11/Screenshot_1.png)

*Standard vs the largest possible font settings*

### + High performance

A lot of factors go into accessing an app’s performance: CPU usage,
number of requests per second, average response time, number of frames
per second, and more. The Flutter team promises a constant 60fps, which
is the rate at which modern screens display a smooth, clear picture.
Since any lag in such a frame rate will be immediately noticed by a
human eye,  developers try to maintain motion at this level.

To access how well Flutter pulls through, see [this
research](https://www.slideshare.net/KorhanBircan/crossplatform-app-development-with-flutter-xamarin-react-native)
comparing Flutter, Xamarin, and React Native performance. Spoiler alert:
Flutter came in first with 58fps and a 220-millisecond launch time.
Xamarin launched in 345 ms with 53fps and React Native came second with
57fps and 229 ms.

Just a few other practical comparisons have been made.
[Here](https://robots.thoughtbot.com/examining-performance-differences-between-native-flutter-and-react-native-mobile-development#conclusion),
Flutter almost matched native app CPU usage, but used 50 percent more
memory than React Native.

Cons of Flutter development
---------------------------

Whenever we review a young or less popular technology, we notice the
same set of drawbacks diminishing the product’s success. Even though
cross-platform development is a new programming practice, Flutter
sometimes loses in the battle with its slightly older competitors. What
are the drawbacks?

### – Lack of third-party libraries {#--lack-of-third-party-libraries}

Third-party libraries and packages play a big part in automating
software development for programmers and relieving the need to code
everything from scratch. These libraries are mostly open source, easily
available, and pre-tested – who wouldn’t want to try a tool that’s been
used and tested in different environments before?

For many older and more popular technologies, finding the needed package
is not a big problem. As mobile developer Aawaz Gyawali
[says](https://medium.com/@awazgyawali/flutter-are-there-plenty-of-third-party-libraries-bc138d7fc37a)
on Medium:

*Talking about React Native, oh boy it’s JS. We get 10+ npm modules for
everything. Just type “…….. npm module” on Google and you will get more
than 10 results. The main benefit of using RN is that the community of
the developers is so big that, if you file an issue on GitHub, you will
find someone who will create a module for you.*

Flutter, like any new technology, doesn’t share these numbers. Flutter’s
[official resource of free packages](https://pub.dartlang.org/flutter)
gets better every day with, its list of tools is still growing. At
least, Flutter takes care of your UI package needs with handy widgets,
but any long-term development will probably require some waiting before
the product abounds in contributed content.

### – Dart, again {#--dart-again}

You may have seen in our comparison of Flutter vs
Xamarin that we mentioned Dart both in positive and negative lights. That’s
because Dart is a great language by itself – its paradigm should be
familiar to most programmers, it’s fast and object-oriented. But it
often loses in comparison to other technologies, especially giants such
as JavaScript, C\#, or native Objective-Cand Java. Not many beginning developers will pick up Dart on their
journey and finding new people for your mobile team can also be a
challenge. This should be something to consider when you’re choosing a
cross-platform approach.

### – Large file size {#--large-file-size}

Developers go to great lengths to minimize the size of an app. Users
have limited storage on their phones, so it’s much more preferable to
release an app that won’t make them delete it in favor of precious
photos or a music library. To decrease the program size, programmers
tend to avoid animations, bring the number of libraries and packages to
a minimum, or compress images.

Flutter has greatly frustrated developers when the release file size of
the Hello world app reached 6.7MB. Even after dropping to 4.7MB, it
[remained much
bigger](https://android.jlelse.eu/comparing-apk-sizes-a0eb37bb36f) than
native Java (539KB) and Kotlin (550KB) apps – and that’s for the bare
minimum app. Although, to be fair, its competitors share the same
problem, and probably even more so – the release version in Xamarin will
take almost
[16MB](https://docs.microsoft.com/en-us/xamarin/android/deploy-test/app-package-size)
and 7MB in React Native.

### – Issues with iOS {#--issues-with-ios}

Since Flutter is developed by Google, developers are rightfully worried
about its implementation for iOS. There’s no doubt that building Android
apps on Flutter is fast and enjoyable since Google is directly
interested in fixing bugs in the shortest amount of time. But what about
Apple devices?

One of the biggest updates in Flutter’s Release Preview 2 included a
pixel-perfect iOS look. The team
[illustrated](https://3.bp.blogspot.com/-UF1Gy-3Ajzo/W6Aume35h7I/AAAAAAAAGCw/lTQwwiQu2PEWegrxQiG9cqsxvzg8CMctwCLcBGAs/s1600/transitionimage2.gif)
the possibilities of Cupertino widgets by recreating iPhone settings on
Flutter. However, until recently, design features weren’t up to date and
followed iOS 10 features while iOS 11 had already been live for months.
It’s unclear yet if updates will keep coming as fast as Android’s
version when the product will finally leave the beta phase.

How to get started with Flutter
-------------------------------

So, we’ve reviewed Flutter’s main features, dropped in some comparison
with other products, and hopefully helped you form your own opinion
about the technology. Now, how do you get started with Flutter?

**Check your system requirements.**Windows users must have Windows 7 SP1
or later (64-bit) with [Windows PowerShell
5.0](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-windows-powershell?view=powershell-7)
and [Git for Windows](https://git-scm.com/download/win) pre-installed.
Mac OS developers need a 64-bit version with [Xcode
9.0](https://developer.apple.com/xcode/) or newer installed while Linux
users don’t have to comply with any special requirements.

**Download Flutter SDK.** [Choose your
OS](https://flutter.io/docs/get-started/install) and follow the
instructions. All operating systems support development both for iOS and
Android, but you will also require a platform-specific editor. Dart
comes pre-installed with Flutter.

**Install an editor.** You can use any IDE with Flutter command lines,
but Google recommends using their plugins for officially supported
editors: [Android Studio](https://developer.android.com/studio/),
[IntelliJ](https://www.jetbrains.com/idea/download/#section=windows),
and [Visual Studio](https://code.visualstudio.com/).

Also, you may find following links useful:

[Material Design docs for Flutter](https://material.io/develop/flutter/)

[Check out the curated list of
resources](https://github.com/Solido/awesome-flutter)

[Explore Flutter apps in a showcase](https://flutter.io/showcase)

[Review the gallery of Flutter
widgets](https://play.google.com/store/apps/details?id=io.flutter.demo.gallery)

Will Flutter replace React Native and Xamarin?
----------------------------------------------

Short answer: Not yet.

Long answer: Should it? Considering the rate at which we’re improving
our programming habits, it’s fair to expect a new Flutter to appear on
the horizon in a few years. This doesn’t mean that any older
technologies become obsolete, it just gives us more options and opens
new possibilities.

In business, however, the decision whether to use a new tool when
there’s an old tried and tested one can cost a lot. How to know if you
should take this step? We always recommend considering these three
factors:

**Team.** If you have in-house developers, will they gladly learn Dart
and embark on creating apps differently than they did before? If you
want to hire an outsource team, is there one with Flutter experience? If
you’re looking to create your own development expertise, is there enough
Dart/Flutter talent on the market?

**Time limit.** Does your team have time in between their project tasks
to learn Dart/Flutter? How time-sensitive is your project?

**Scope.** How big a project do you have? Is it complex and long-term?
Or is it an MVP that will bring minimum losses in case of failure?

Hopefully, this article answered most of your Flutter questions. Let us
know what new technology you’d like to read about next in our series The
Good and the Bad.


