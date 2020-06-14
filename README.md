# How to Design an app for Android TV
**The current explanation is based on the Design Propopal written by me for Building [STEM DIVERSE TV](https://github.com/NitishGadangi/stem-diverse-android-tv) of [AnitaB .org](https://github.com/anitab-org)**

**Refer to the [Github Repo Files](https://github.com/NitishGadangi/Android-TV-Prototpe) to get Raw version of all the Design Templates used in this proposal**

**All MockUps are Designed using [AdobeXD](https://www.adobe.com/in/products/xd.html)**

# Building for Android TV
TV celebrates content by making it front and center. Whether you’re looking for movies, games, or TV, it’s about finding and enjoying content with the least amount of friction.

We have an entire living room or other rooms dedicated and focused around the TV. TV is colorful, guided by ambient movement, with immediate access to content. These qualities define the experience of TV and form the foundation of Android TV’s design.

## What Users Expect ?

As a potential user of TV Apps myself, I prefer to have these following features which I think has already been satisfied based on the App Design explained above.

-   People often use TV in a relaxed mindset. Casual consumption is the primary use case of Android TV.
    
-   While searching for content, every part of the experience should be simple. New content should be easy to discover.
    
-   The default action should be one click away.
    
-   Minimize the number of navigation steps required to perform actions. Build apps with the fewest screens possible between app entry and content immersion.
    
-   Avoid making users enter text whenever possible, and use voice interfaces when you require text input.
    
-   Because anyone in a trusted household might have access to it, app content should be appropriate for mixed audiences.This makes a TV an inherently shared device.
    
-   Place controls, like the search action, in locations that don’t overlap with other clickable elements.
    
-   Categories can be traversed on the vertical axis, and items within each category can be browsed on the horizontal axis.
    

Every point of the above mentioned user stories are considered while building the APP UI and correspondingly REST API is designed. And I think you will witness them while going through the proposal.

Users come for content and stay for the app. Hence it really matters how user friendly and intuitive you build the app. According to me the main focus of building a TV app revolves around these three building blocks.

![](https://lh6.googleusercontent.com/Scv9Q5GtHibhb6OuHO8F0P8IEyk2JS3hJnKsuAmFd1Yf9Q0Za89LXLsIuKCEW8m8LrJigGbV8GDXUfb9wdXPHDph-tsj9tiv4K9raBLwUkQsMYdAkbvejUPInt0PUD-8ifEr72tq)

Now let’s dive into the technical discussions of the App design.

# App Design
You can view all the Mockups mentioned below [here at highest quality possible.](https://drive.google.com/open?id=1n0w_uteuTSFm4Wa9-akaQZqM-hUokkJa)

## Designing Principles
As TV is quite different from Mobile there are several design principles which are quite different and they must be considered while building the app for TV. For example we should make an app so that we can navigate the application only using ↑↓→← direction keys, instead of touchpad navigation. Because the user uses a remote controller, and cannot use the “touch screen” function with TV.

Navigation: TV should provide the shortest possible path to content. Place the fewest screens possible between the viewer and content. When screens are necessary, they are consistent and simple to operate with an input device.

Information density: Due to the viewing distance of the TV, users may not be able to process as much information on TV as they would on a computer or mobile device. Limit the amount of text and reading on TV screens.

Hence my App mockups follow all these principles in order to make UI as User Friendly as possible.

## Colors

Colors on TV can look very different from colors on computer or mobile devices, and some color combinations may not work on both.

Using colors two to three levels darker than those used a mobile device is recommended. Alternatively, we can use colors from the 700-900 range of the material color palette.

I have opted to go with Darker UI as it will reduce the Eye Strain and Makes users stay for the content for a longer duration.

TV WHITE: Pure white (#FFFFFF) can be very harsh on a bright TV screen. Light gray (#EEEEEE) is recommended as the default text color on dark backgrounds.

And so does the remaining colors and each color has its own significance.

Here is the Colour Pallete I had used for the whole Design.

![](https://lh6.googleusercontent.com/d4TAq4098vknQEdkxoSLzq1i3HWqu20cktVwAvFB0hEeEWQ0f3CHl2aZWHv44aw2pDpkFgLQWvh2ZYffYV5vhhLGE493UE7-R-Po2TgppVUTcRVOlgBS5KjNHP3JswVU7kUiidQ0)

## Typography

![](https://lh3.googleusercontent.com/ARBmOqyENKE1zbBN5HPH4nYbts-9fOUanBjgSNNDipj9M11cukHehmdnUNU_axW4fKEZfFnJKgVU-muiQIyTgAefW2TwJ_iq9GZNxfTBMhXKCnM0jlPYPL1-eJv20WKbcxfUAcIS)

## UI States

This explains how the user interacts with each of the UI elements and how they respond to each element.

![](https://lh6.googleusercontent.com/m_XZPywTnf4De2Kk69TLVM8Fde4ueITd6WAX3gLJJBTFjq4A0FQmpPuZ3oBB43-BtL3tkoo1TWPfiBYPjfTCj_0iHLkAKuGf_pBkrfiWbP0QxS5JcEedKWJi0x74s6PPkgbCN_dH)

## App Structure

The MVP will contain the following features explained below with mocks and backend.

Here is a basic overview of the flow of the app. Basically shows all the screens and interlinks between them in brief.

The Structure of the App is basically divided into three segments

1.  BrowseView: where the user browses for the content.
    
2.  InAppSearch: where users search for the content.
    
3.  ConsumptionView (Player): where user watches(consumes) the content.
    

[Go Here](https://drive.google.com/open?id=1UA7rYkcXcMgP-XXHQZeysVtNqxVsQDQ4) to view it at higher resolution.

*The mentioned figures are available below in the further discussion,(Use figure numbers)

[![](https://lh4.googleusercontent.com/-MjxP3JHTMPBmG4Z1b2X0uXLYU9QzO2e6x5BPpPvF1G2ZeXMBDkvb8SGWP8M7bPWl36qnf3DjW3Ui0q03DBw7CPkrv1yQlLkteDlYOJHBmH3RvsMYRQHVDb43v8PULLV1Vpd_ZxV)](https://drive.google.com/open?id=1UA7rYkcXcMgP-XXHQZeysVtNqxVsQDQ4)

## Splash

Splash screen presented as soon as the app launches. It basically enables us to load the background content in the meantime. So that the user will be presented with the homepage with at least partially loaded content.

*The Logo used is provided by Anna and however it can be changed in future if necessary.

[Figure 1.0] SplashScreen

![](https://lh5.googleusercontent.com/SRon9VDSyF7l2XDbWuxLt7tvDjDcuvEaXRCOFSB-QwemTlPGoYFNKj2CT4w4psiLTMaYk12S4RPribpAeq1nTKX9erEIHzAzeAEZ_d2CyArlHFn9eUvtNvpMqKKT_JoNoTYmH5mH)

## Home

This is the place where users land up for the content.

HomePage can be structurally divided into three parts.

1.  TitleRow: up top where Titles of the each page can be displayed in a row
    
2.  BrowseRow: Browse Row organizes content into categories. These categories are displayed in the form of horizontal lists, which are stacked vertically on top of one another. By default, only one row scrolls horizontally at a time.
    
3.  SideLane/BrowseLane: where major controls for Activity shifting lies.
    

[Figure 2.1] Home with TittleRow and BrowseRow

![](https://lh4.googleusercontent.com/pv6FMKvblMiDyWY4v--uU8UQJcB3jZVOFAUt2cekudBBbWCBAQH2lInl17ZvTyKdxPFt6OVyPJd6C3XB-cTuoQ_N1bjY3Mn_a8OfwnI58Hc94HSnGFriEeXCQHodKdfzCMm-nKiL)

On hitting the left button the D-Pad user can navigate into the SideLane which looks like this.

[Figure 2.5] BrowseLane/SideLane

![](https://lh4.googleusercontent.com/ODNwF5WxRKTXfjaVCMWuTGBlaM7C3fpaXPkTeLM6HwHfAKc-iq4pZ8AlXUAFvASzm2N8zymsBhOlm54SQl8O6PgisuunfQzn7Sv-D4ptQuIOQr-ZtkI6GFiy-wQuENQUGPbkRC6w)

## GridView

The BrowseRow will be containing only few number of videos of the content, so after reaching at the end of the each row there will be an option to SEE ALL from that content

[Figure 2.3] SEE ALL

![](https://lh6.googleusercontent.com/_u6D1s6ze6L-2MkqTn-ec9R8rEoUGOVsmbQT51B6854P7q04XTrI_c_68B_BtWzicBacVQWTemmHtaM2t64QHeKmqV7KLsg1o6nmfDlljEbGbX1LppNz7WZCq7KR1K4JU-q0_rHl)

Later on clicking on SEE ALL , a new page opens displaying all the content related to the corresponding topic/category. I like to call it GridView.

[Figure 2.4] GridView

![](https://lh3.googleusercontent.com/oUNOgig0daWMFAwxVJeQZxPIuRav4VFPW8YKGHl7va_ElLfJzfmS3fwamo-j0W4Oer-ueRyAb5vIoeeFMDzSxUoMyivdAujug308cKWqmaUQ2HCIJw-Pc52AV5cTcy_yEBbouNQn)

## In-app Search

In-app search provides a consistent search experience for all participating Android TV apps. Users may quickly search across apps that contain large amounts of information.

Invoking in-app search is simple. Press the microphone button on your controller or select the on-screen search button from the SideLane.

[Figure 3.1] Search

![](https://lh3.googleusercontent.com/AK_45t96uYwIKV0_sI6pnmBRqCPmp9DNPHfQ1b1W7KZ7znuW7p-vskog1nHcVmxDWJyQ64EsoEjxF1I3UYS4v7dM2KW8JMBtFeZlE4zW8x841jyCIBsr7BPb-6l36L-Or40r87VM)

On making a Search, the search results will be stacked as a row in the bottom, so that users quickly select one to watch. Also, enabling auto search will help to uplift the user experience.

[Figure 3.2] Search Results

![](https://lh4.googleusercontent.com/5S7mSd110D0CqSa_a34TDn42W-UAyVEnE21DmVRM51ty66B-Rg4weptO7m-hfFLVkYS8Re92qXch-gOPrLM13csFx_NriAojBsqOftpD-FEyEoryFSJF5cryL5O-Pqfzh5_K8Q2t)

There is also a provision to integrate Google Assistant with the search which makes it more user intuitive. However it might not be possible for the version1 of MVP.

![](https://lh4.googleusercontent.com/uEGCOaAJZLX1fZuH6zFlfFwtShFI4DXRf0bWSOw8x9L-D8JBnGWEYdvba572_CzSP3Afwv2fkYpbF9tLTFv7ydKYzm94BDaK40X1Cis0ADg0iLyzETydpghNV-c2JsEntGogj2Ki)

## Continue Watching

Because there are many reasons users pause content, provide multiple avenues for users to quickly pick up from where they left off. Continue watching Row will help us to achieve this.

[Figure 2.2] Continue Watching ![](https://lh5.googleusercontent.com/o9OPJnSUKIWKNRufhWpIOWsNfxAfpQpfBpE1vQkjjzAETaP32Bl0Gj5zA358D-FLQj410bxqvCmJsAeyjBoTg_FcKoUYlNxbLIQx-tmxrme4t3rRsFqAWeURB07OPqWp8XNSkSpc)

## ConsumptionView (Player)

The Consumption View is where the user will engage with or watch content. Users will spend most of their time in this immersive experience.

### Transport Controls

Transport Controls give users control of the content currently playing.

1.  The controls are displayed by pressing any navigational button on an Android TV controller.
    
2.  The center action is focused by default, so it should be the most commonly used action. In most cases, this action is Play/Pause.
    
3.  To Keep the number of available actions to a minimum, I have added quick shortcuts to go to next and previous content.
    

[Figure 4.0] ConsumptionView (Player)![](https://lh3.googleusercontent.com/l-Jjw5f391Kpudk123mhqOGbitMyqA9DU-gNtJR5tadBV-D2qlQ9GJm4dYQbWALMCtkzhVvlj6fWyX6UvM7AsACKCzFVPp54c_qn9VpG7uEdgzYgdniQy24UWuMMcYsdgOiNFcXy)

# Techstack

Here is a list of libraries and programming practices that I would like to propose and would follow while building the Android App.

## Leanback

The leanback library provides a templated UI so developers can focus on the important parts of their app.

When using leanback, content is shown in rows. Leanback supplies a rectangular card view, ImageCardView, to easily display content. The card size scales when selected and has shadows to accent the content. This is great for content such as movie posters and album art.

API Reference:

[androidx.leanback.app](https://developer.android.com/reference/androidx/leanback/app/package-summary)

[androidx.leanback.database](https://developer.android.com/reference/androidx/leanback/database/package-summary)

[androidx.leanback.graphics](https://developer.android.com/reference/androidx/leanback/graphics/package-summary)

[androidx.leanback.media](https://developer.android.com/reference/androidx/leanback/media/package-summary)

[androidx.leanback.preference](https://developer.android.com/reference/androidx/leanback/preference/package-summary)

[androidx.leanback.system](https://developer.android.com/reference/androidx/leanback/system/package-summary)

[androidx.leanback.widget](https://developer.android.com/reference/androidx/leanback/widget/package-summary)

[androidx.leanback.widget.picker](https://developer.android.com/reference/androidx/leanback/widget/picker/package-summary)

Refer [Leanback](https://developer.android.com/jetpack/androidx/releases/leanback), for a complete description about the library.

## Exoplayer
Player Constitutes the major section of the app. Because, it is where the user will engage with or watch content. Users will spend most of their time in this immersive experience. It's better to have an inbuilt player instead of opening another app to play videos.

[ExoPlayer](http://google.github.io/ExoPlayer/) is an open source project that is not part of the Android framework and is distributed separately from the Android SDK. ExoPlayer’s standard audio and video components are built on Android’s MediaCodec API, which was released in Android 4.1 (API level 16). Because ExoPlayer is a library, you can easily take advantage of new features as they become available by updating your app.

ExoPlayer supports features like Dynamic adaptive streaming over HTTP (DASH), SmoothStreaming and Common Encryption, which are not supported by [MediaPlayer](https://developer.android.com/reference/android/media/MediaPlayer). It's designed to be easy to customize and extend.

Here is small snippet which explains the initialisation procedure for Exoplayer

[![](https://lh5.googleusercontent.com/1pIbE9-gMLbKmj0G_ZXFA7DfOf_pgs8nBZpMnZD2XQ3qzLAVeeOeX4SZ5Dvh12aIun_uSTnSuMDCQOAOeQCvUGVhkVWSHAsNH100wet96r0Ng-pv4fI8ecIkJHnSjz5zzlC-ZbnC)](https://carbon.now.sh/?bg=rgba(255%2C255%2C255%2C1)&t=seti&wt=none&l=text%2Fx-java&ds=false&dsyoff=20px&dsblur=68px&wc=true&wa=true&pv=0px&ph=0px&ln=false&fl=1&fm=Fira%20Code&fs=18px&lh=155%25&si=false&es=2x&wm=false&code=%252F%252FCreating%2520the%2520player%250ASimpleExoPlayer%2520player%2520%253D%2520new%2520SimpleExoPlayer.Builder(context).build()%253B%250A%252F%252F%2520Bind%2520the%2520player%2520to%2520the%2520view.%250AplayerView.setPlayer(player)%253B%250A%252F%252F%2520Produces%2520DataSource%2520instances%2520through%2520which%2520media%2520data%2520is%2520loaded.%250ADataSource.Factory%2520dataSourceFactory%2520%253D%2520new%2520DefaultDataSourceFactory(context%252C%250A%2520%2520%2520%2520Util.getUserAgent(context%252C%2520%2522yourApplicationName%2522))%253B%250A%252F%252F%2520This%2520is%2520the%2520MediaSource%2520representing%2520the%2520media%2520to%2520be%2520played.%250AMediaSource%2520videoSource%2520%253D%250A%2520%2520%2520%2520new%2520ProgressiveMediaSource.Factory(dataSourceFactory)%250A%2520%2520%2520%2520%2520%2520%2520%2520.createMediaSource(mp4VideoUri)%253B%250A%252F%252F%2520Prepare%2520the%2520player%2520with%2520the%2520source.%250Aplayer.prepare(videoSource)%253B)

## Supported Media formats
In version 1 of the MVP, mostly we might be added content from the youtube directly. Basically embedding sources from youtube into the Exoplayer.

Here is how we can extract the source link from youtube and play them in exoplayer.

![](https://lh3.googleusercontent.com/RasOcIsEVP8uuTNyemGfAQ3hhMvYwyQrH_RO2NiuKUfbDKlSCr1eJRaZER3gEsd6q-d25gC0_sHuX8taoofnQA7459Z5Co0XYrIwshisqtwDo6hSg0g5754onVHSUXAaDWOtT9B7)

However, in ExoPlayer every piece of media is represented by MediaSource. The ExoPlayer library provides MediaSource implementations for several stream types:

-   DashMediaSource for [DASH](https://exoplayer.dev/dash.html).
    
-   SsMediaSource for [SmoothStreaming](https://exoplayer.dev/smoothstreaming.html).
    
-   HlsMediaSource for [HLS](https://exoplayer.dev/hls.html).
    
-   ProgressiveMediaSource for [regular media files](https://exoplayer.dev/progressive.html).
    

## Glide
Images form the major part of the App and hence we need to make sure loading images into Imageviews goes frictionless.

[Glide](https://github.com/bumptech/glide) is a fast and efficient open source media management and image loading framework for Android that wraps media decoding, memory and disk caching, and resource pooling into a simple and easy to use interface.

[![](https://lh5.googleusercontent.com/RaKnnbehqTp0Dftv50G4HkUKTCieXXxaKvG_li7jc27qfjDvzf9dYmoMILbztkBgLu1MZ1d3WTMkWLHLPIEGoDxrXpPe-kltNNtY86BhPfrObjDjGDPXkL4cWe4bXtvtf0WmldVB)](https://carbon.now.sh/?bg=rgba(255%2C255%2C255%2C1)&t=seti&wt=none&l=text%2Fx-java&ds=false&dsyoff=20px&dsblur=68px&wc=true&wa=true&pv=0px&ph=0px&ln=false&fl=1&fm=Fira%20Code&fs=18px&lh=155%25&si=false&es=2x&wm=false&code=Glide.with(myFragment).load(url).centerCrop()%250A%2520%2520.placeholder(R.drawable.loading_spinner)%250A%2520%2520%2520%2520.into(myImageView)%253B)

## Retrofit
[Retrofit](https://square.github.io/retrofit/) is a REST Client library (Helper Library) used in Android and Java to create an HTTP request and also to process the HTTP response from a REST API.

REST Client in our case is the Retrofit library that is used on the client side (Android) to make HTTP requests to the REST API.

Here is small snippet as proposed in the [Retrofit documentation](https://square.github.io/retrofit/)

[![](https://lh4.googleusercontent.com/7DUiRaiZnNsDExgF-VAa8D4KAAGU1FJhJPAPADQLb6XTw34TKVoUotfJC8Ju2if4WC2dJQ_MQ19O1UXAKVtfLg82nmfe8MpqKc2AjnAugK4s0wl4BX0XicuYnWckCZJdvXWLkdst)](https://carbon.now.sh/?bg=rgba(255%2C255%2C255%2C1)&t=seti&wt=none&l=text%2Fx-java&ds=false&dsyoff=20px&dsblur=68px&wc=true&wa=true&pv=0px&ph=0px&ln=false&fl=1&fm=Fira%20Code&fs=18px&lh=155%25&si=false&es=2x&wm=false&code=%252F%252FThe%2520Retrofit%2520class%2520generates%2520an%2520implementation%2520of%2520the%2520GitHubService%2520interface.%250ARetrofit%2520retrofit%2520%253D%2520new%2520Retrofit.Builder()%250A%2520%2520%2520%2520.baseUrl(%2522https%253A%252F%252Fapi.github.com%252F%2522)%250A%2520%2520%2520%2520.build()%253B%250A%250AGitHubService%2520service%2520%253D%2520retrofit.create(GitHubService.class)%253B)

## RxJava

[RxJava](https://github.com/ReactiveX/RxJava) provides an opportunity for making parallel network calls efficiently and easily.

RxJava is a Java VM implementation of Reactive Extensions: a library for composing asynchronous and event-based programs by using observable sequences.

## Kotlin and MVVM
Of course, Kotlin being the android-first language it's obvious that it will be beneficial for future sustainment of the project. Basically, less code, more robustness, better safety, and a strong community.

As everyone knows about the perks of shifting towards Kotlin, I would like to stop the Kotlin discussion here and move towards dependency injection.

Coming to MVVM, MVVM combines the advantages of separation of concerns provided by MVP, while leveraging the advantages of data bindings. The result is a pattern where the model drives as many of the operations as possible, minimizing the logic in the view. MVVM being itself a suggested architecture by Google Developers, it's quite obvious to have such advantages

  

## Dependency Injection
Usage of dependency injection frameworks gives you various benefits that improve the app performance and allowing the app features to stay decoupled, helps us in testing components individually. And there are several more advantages that make up my whole proposal if I continued explaining… Hence, Keeping the advantages aside let me explain which framework I am going to opt for.

There are two major types of Dependency Injection frameworks available right now.

1.  Dagger2
    
2.  Koin
    

Out of Dagger and Koin, would prefer to go with Koin, and Koin has its own reasons and perks for opting it over Dagger. I will list them briefly below.

**However, I am quite experienced in working with Dagger2 also. Hence it's ok for me to work on any of them. So we can discuss this further in the community bonding period and proceed further based on discussions.

### Why Koin
Since Koin isn't a dependency injector but a service locator with a clever reified trick that you can use to manually perform dependency injection, the boilerplate will scale disproportionally.

This below stats might give a small idea.

![](https://lh3.googleusercontent.com/C2KiO0kpkSEr7dV3yCF-bCvdXierch6yB_-AQ1GP8j4rCm0hboqRA_OcfKRbXBwIOJmhwsyXMRkjplXDgSoxwGsGfSGn-lIb8D3QEu13kkD558DYp98f2nMxQXhFwcPnCu4_eyrJ)

To make the situation clearer, let me give more details on the Koin framework.

-   Koin DSL allows you to declare your components graph, through functions and constructor dependency injection.
    
-   Koin is a real DI container which manages all components instances and definitions. We don't use any introspection or proxy mechanism. It's all about pure function resolution.
    
-   Service Locator is only needed in Activity/Fragment classes, to inject your components (lazily or not) due to the fact we can’t inject them by a constructor.
    

![](https://lh4.googleusercontent.com/cM48lHsneNN0WkUTULt5_lmv3Hvu2NxWKC2WarKfPnQeSsy9aajdxT8IESUwzzL_qXXcw52SWKgALtg5XCxh20tfHFF8g2Qv6n06CXT1N3Nv7n-NPGf855yHX33e93rzzGPM8lHj)

The thing is that frameworks like Koin reduce the 90% boilerplate thanks to the reified trick, making it very interesting.

That summed with the problems that annotation processing brings, increasing compile times and making it harder to do an incremental compilation in modules makes me want to re-evaluate if Dagger is worth it.

I mean having to add one line per each class that I want to add to the service locator is way better than having to re-compile all the graphs every time I do a clean build…

## Testing
Testing is the most important step of the development life cycle as it will help us to verify the functionality of all the features of the app. Here is a list of libraries which I will be using for testing.

-   Functional tests with [Espresso](http://google.github.io/android-testing-support-library/docs/espresso)
    
-   Unit tests with [Mockito](http://mockito.org/)
    
-   [Checkstyle](http://checkstyle.sourceforge.net/), [FindBugs](http://findbugs.sourceforge.net/) and [PMD](https://pmd.github.io/)
    

## DevOps
In order to make it dev-ops friendly firstly I would like to use a Trunk based approach during the development of the app.

Here, We only have one main branch. Then, we would branch off master when doing any features and anything that gets merged into master should be ready to ship to users. The image given can explain it in a better way.

  

![](https://lh5.googleusercontent.com/uQ4JADxFZlSYjEN61Go2N110YQ1MBAzHEgMvQ0znkxRXLZgohAhTJ58vv_GzsDcMgbPUX3Po-R-RdVmGu3BQs7Bk7Dws-p-xjQL_1r5hB6bIMSnhjj0PNrT9HI6qgcQBk8Xqq6_T)

### Fastlane (optional)

I made this optional, as it might not be possible to implement it for the first version of MVP.

[Fastlane](https://fastlane.tools/) is a great tool that developers can use to automate their release process & significantly reduce their release cycle times. The 4 major features offered by Fastlane are:

-   [AUTOMATE SCREENSHOTS](https://docs.fastlane.tools/getting-started/android/screenshots/): Automatically generate localized screenshots for the app store.
    
-   [BETA DEPLOYMENT](https://docs.fastlane.tools/getting-started/android/beta-deployment/): Easily distribute beta builds to testers.
    
-   [APP STORE DEPLOYMENT](https://docs.fastlane.tools/getting-started/android/release-deployment/): Publish a new release to the app store in seconds.
    
-   [CODE SIGNING](https://docs.fastlane.tools/codesigning/getting-started/): Reliably and consistently code sign your app–no more headaches.
    

Since Fastlane allows plugins, there is no restriction on the capabilities.

  

## What about Amazon FireTV
Most apps that work on Android will also work on Fire TV because Fire TV is built on Android. The only difference is with services — for Fire TV, you'll want to use Amazon services instead of Google services (see [How Fire TV Development Differs from Android TV Development](https://developer.amazon.com/docs/fire-tv/differences-from-android-tv-development.html)).
Hence building an Android App based on Android 5.1 / Android 7.1 will work on FireOs5 / FireOs6 seamlessly.


## Whats Next
Ultimately this is the basic approach and you must relate it to your requirements.

I hope my explanation gives you a basic idea upon the various design guidelines that one must follow while building for TV.

Thats the End for now.

I will try to add more about the Backend in the upcomming days. Untill then Keep Exploring.


**Designed with ❤ by [Nitish Gadangi](https://nitishgadangi.github.io/)**
