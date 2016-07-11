# udnd-android-basic
Rapid review of the Udacity Android Basic Nanodegree

# Android Development For Beginners

## Resources

 * [Vocabulary Glossary](https://developers.google.com/android/for-all/vocab-words/)
 * [CheatSheet: Common Android Views](https://drive.google.com/file/d/0B5XIkMkayHgRMVljUVIyZzNmQUU/view)
 * [Android Developers Documentation](https://developer.android.com)
 * [BLOG: Styling Android](https://blog.stylingandroid.com/)
 * [BLOG: Chris Banes](https://chris.banes.me/)
 * [PODCAST: Fragmented Podcast](http://fragmentedpodcast.com/)



## Lesson 1A: Building Layouts

Vocabulary used in this lesson
 * Layout
 * User Interface
 * TextView
 * ImageView
 * Button
 * Camel Case


Introducing Views
 * Rectangle on the screen
 * Different kinds of views (TextView, ImageView, Button)
 * View = basic building block for layouts
 * View components defined in camelcase
 * Exercise: identify views in various UI


Programming
 * Code = Sequence of instructions
 * IDE = Integrated Development Environment
 * Android IDE = Android Studio
 * XML = Extensible Markup Language


XML Syntax
 * TextView in XML => Make observations on [example](https://classroom.udacity.com/nanodegrees/nd803/parts/8031345401/modules/677455098475460/lessons/4027328704/concepts/42472686090923)
 * Syntax = rules that define valid language
 * XML Element Name
 * XML Attributes
 * XML Brackets for Opening/Closing "Tags"
 * Elements can be nested
 * Brackets must match for valid XML


XML for Layouts/Views
 * Attributes define characteristics of view
 * Attributes have default values
 * You can leave out attributes if default value is okay
 * Element Names are in camelcast
 * Exercise: Identify element name, attributes in [example](https://classroom.udacity.com/nanodegrees/nd803/parts/8031345401/modules/677455098475460/lessons/4027328704/concepts/42555185990923)


XMLV = [XML Visualizer](http://labs.udacity.com/android-visualizer/?_ga=1.7577202.1373577476.1468202837#/android/text-view) (Udacity only)
 * DP = Density Independent Pixels
 * Medium, High and Extra-High Resolution devices
 * DP = same physical size on all devices
 * Make [touch target size](https://material.google.com/layout/metrics-keylines.html#metrics-keylines-touch-target-size) at least 48dp on all devices
 * Exercise: Change View (text, size)
 * Exercise: Create an error, then undo it.


Debugging
  * Getting past errors is important
  * It's a trial-and-error method
  * Strategy: read error msg, see working code, undo, stack overflow or ask for help


Wrap Content (Views)
 * Setting absolute width/height is bad practice
 * Set "wrap_content" adjusts to "fit" content
 * Set "fill_parent" adjusts to "fill" container

Text Size (TextView)
 * "android:textSize" is the attribute name
 * "sp" is scale-independent pixels (used only for font)
 * scales with user's Font preference on devices
 * Best Practices: [Material Design Typography](http://www.google.com/design/spec/style/typography.html#typography-styles)
 * [ProTip](https://plus.google.com/+AndroidDevelopers/posts/gQuBtnuk6iG): use "android:textAppearance" instead of "android:textSize" and set its value to a predefined constant (e.g., textAppearanceSmall) within that theme. This allows you to have a consistent/limited set of centrally-defined values for textsizes across your app screens


Color
 * Use "android:background" for component background
 * Use "android:textColor" for text color
 * Values can be set to standard/theme-defined values (@android:color/white) or to hex value ("#ffffff")
 * Best Practices: See [Material Design Color Palette](https://material.google.com/style/color.html#color-color-palette)


Simple ImageView
 * ElementName: <ImageView>
 * Drawables = resource type for images
 * Attribute "android:src" values set to drawable reference
 * Attribute "android:scaleType" scales that source image to make it show appropriately within the container - see [values here](https://developer.android.com/reference/android/widget/ImageView.ScaleType.html) notably *CENTER* and *CENTER_CROP*

Documentation
 * Reference the [documentation](https://developer.android.com) for latest View elements and their attribute names, values.
 * Exercise: View TextView documentation
 * Exercise: Use new TextView attributes


## Lesson 1B: Building Layouts



## Practice Set 1

Hello World
 * [View the video](https://classroom.udacity.com/nanodegrees/nd803/parts/8031345401/modules/677455098475460/lessons/4034888704/concepts/43534185610923#)
 * [Read the instructions](https://classroom.udacity.com/courses/ud837/lessons/4034888704/concepts/41804293660923)

Concepts
 * Android Studio Version (now: 2.1.2 )
 * Package Name
 * Minimun SDK (use API 15 +)
 * API Level (Version Distribution Dashboard)
 * Use "Empty Activity" (leave defaults)

[Android Studio Tour](https://classroom.udacity.com/nanodegrees/nd803/parts/8031345401/modules/677455098475460/lessons/4034888704/concepts/43534185620923)
 * Android mode = shows logical grouping of files
 * Project mode = shows actual files in directory
 * Use "Android" mode
 * app/java = source, app/res = resources (XML)
 * Layout file = Design/Text views
 * Design view = drag-and-drop views into layout
 * Text view = easier to read/edit for attributes

Running on Device
 * Set phone into "Developer" mode
 * Install driver on development device (PC) if needed
 * Connect phone and PC with USB cable
 * "Run" your app, select device (should be auto-detected)
 * Installs app and starts it (verify this happened)

Running on Emulator
 * AVD = Android Virtual Device
 * Select existing AVD for quick start
 * Create custom AVD for advanced usage
 * "Run" your all, select AVD => will be slow to start
 * Note: If "N Preview" causes render issues, select different device from drop-down.
 * [Troubleshooting the Emulator](https://docs.google.com/document/d/1w1Xn_hnSAODAAtdRDp7haYPBtEwX_l7Htpf8Wpgbu6w/pub)

Create the Birthday Card:
 * Select Views
 * Position Views (Relative Layouts allow overlapping)
 * Style the Views


Step 1: Drawable
 * Download image, move to drawable folder, add TextView, add ImageView with this source.

Step 2: Positioning
 * Use RelativeLayout positioning attributes (alignParentRight etc.) to move one TextView to bottom of screen

Step 3: Styling
 * Make text larger (36 sp for both)
 * Set the font (fontFamily: "san-serif-light")
 * Set text color (@android:color/white)
 * Image Expanded to fit entire screen (scaleType: "centerCrop")
 * Text should have spacing around it (margin: 20dp)

