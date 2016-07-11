# udnd-android-basic
Rapid review of the Udacity Android Basic Nanodegree

# Android Development For Beginners

## Resources

 * [Vocabulary Glossary](https://developers.google.com/android/for-all/vocab-words/)
 * [CheatSheet: Common Android Views](https://drive.google.com/file/d/0B5XIkMkayHgRMVljUVIyZzNmQUU/view)
 * [Android Developers Documentation](https://developer.android.com)



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
 * Reference the [documentatio](https://developer.android.com) for latest View elements and their attribute names, values.
 * Exercise: View TextView documentation
 * Exercise: Use new TextView attributes



## Lesson 1B: Building Layouts