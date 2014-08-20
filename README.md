
# Naming Convention for Android Development

## Package Structure

> See this [Package by feature, not layer][1] 

<!--
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>` - contain Application class **only**
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.activity` - contain all activities
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.adapter` - contain all adapters
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.api` - contain all network related classes
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.fragment` - contain all fragments 
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.model` - contain all models 
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.provider` - contain all database related classes
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.receiver` - contain all broadcast receiver classes
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.service` - contain all services 
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.util` - contain all utility classes
 - `com.<COMPANY_NAME>.<PRODUCT_NAME>.widget`- contain all custom views
-->

## Naming Convention for Classes

 - `<PRODUCT_NAME>Application.java` - for Application class
 - `<NAME>Activity.java` - for activity class
 - `<NAME>Adapter.java` - for adapter class
 - `<NAME>Fragment.java` - for fragment class
 - `<NAME>.java` - for model class
 - `<NAME>Provider.java` - for content provider class
 - `<NAME>Service.java` - for service class
 - `<NAME>Receiver.java` - for broadcast receiver class
 - `<NAME>Utils.java` - for utility class
 - `<NAME>.java` - for custom view class

## Short Name of Android Widgets

> **Note**: You should use more meaningful names than these short names unless you have two or more same kind of views in the same place.

 - `aclock` - AnalogClock
 - `actv` - AutoCompleteTextView
 - `btn` - Button
 - `cal` - CalendarView
 - `chb` - CheckBox
 - `chtv` - CheckedTextView
 - `chron` - Chronometer
 - `dp` - DatePicker
 - `edt` - EditText
 - `explv` - ExpandableListView
 - `fl` - FrameLayout
 - `gl` - GridLayout
 - `grv` - GridView
 - `hsv` - HorizontalScrollView
 - `imb` - ImageButton
 - `ims` - ImageSwitcher
 - `imv` - ImageView
 - `ll` - LinearLayout
 - `lsv` - ListView
 - `ctlr` - MediaController
 - `mactv` - MultiAutoCompleteTextView
 - `np` - NumberPicker
 - `pm` - PopupMenu
 - `pw` - PopupWindow
 - `pgb` - ProgressBar
 - `rb` - RadioButton
 - `rg` - RadioGroup
 - `rtb` - RatingBar
 - `rl` - RelativeLayout
 - `rv` - RemoteViews
 - `scv` - ScrollView
 - `schv` - SearchView
 - `skb` - SeekBar
 - `sap` - ShareActionProvider
 - `space` - Space
 - `spn` - Spinner
 - `stv` - StackView
 - `sw` - Switch
 - `tabh` - TabHost
 - `tabc` - TabHost.TabSpec
 - `tl` - TableLayout
 - `tr` - TableRow
 - `twg` - TabWidget
 - `tclock` - TextClock
 - `tsw` - TextSwitcher
 - `txv` - TextView
 - `tp` - TimePicker
 - `toast` - Toast
 - `tgb` - ToggleButton
 - `vdv` - VideoView
 - `vf` - ViewFlipper
 - `vsw` - ViewSwitcher

## Naming Convention for Image Files
> See this [Android-Cheatsheet-For-Graphic-Designers#Naming Convention][2]
 
## XML Files (res/anim)

 - `<INTERPOLATOR_NAME>_interpolator.xml` - for custom interpolator
 - `<ANIMATION_NAME>.xml` - for custom animation

## XML Files (res/animator)

 - `<ANIMATOR_NAME>.xml`- for custom animator

## XML Files (res/color)

 - `selector_<COLOR_NAME>.xml` - for color state list

## XML Files (res/drawable)

 - `bmp_<BITMAP_NAME>.xml` - for bitmap file
 - `np_<NINE_PATCH_NAME>.xml` - for nine-patch XML file
 - `layer_<LAYER_LIST_NAME>.xml` - for layer list
 - `selector_<STATE_LIST_NAME>.xml` - for state list
 - `anim_<DRAWABLE_ANIMATION_NAME>.xml` - for drawable animation
 - `level_<LEVEL_LIST_NAME>.xml` - for level list
 - `trans_<TRANSITION_DRAWABLE_NAME>.xml` - for transition drawable
 - `inset_<INSET_DRAWABLE_NAME>.xml` - for inset drawable
 - `clip_<CLIP_DRAWABLE_NAME>.xml` - for clip drawable
 - `scale_<SCALE_DRAWABLE_NAME>.xml` - for scale drawable
 - `shape_<SHAPE_DRAWABLE_NAME>.xml` - for shape drawable

## XML Files (res/layout)

 - `activity_<ACTIVITY_NAME>.xml` - for activity
 - `dialog_<DIALOG_NAME>.xml` - for dialog
 - `list_item_<LIST_NAME>.xml` - for list item in ListView
 - `grid_item_<GRID_NAME>.xml` - for grid item in GridView
 - `fragment_<FRAGMENT_NAME>.xml` - for fragment
 - `layout_<LAYOUT_NAME>.xml` - for re-useable layout
 - `merge_<MERGE_NAME>.xml` - for `<merge>` Tag **only**
 - `widget_<WIDGET_NAME>.xml` - for custom view
 - `appwidget_<APPWIDGET_NAME>.xml` - for app widget

## XML Files (res/menu)

 - `<MENU_NAME>.xml` - for option menu
 - `contextual_<MENU_NAME>.xml` - for contextual menu
 - `popup_<MENU_NAME>.xml` - for popup menu

## XML Files (res/values)

 - values/colors.xml
 
    - `<color name="<THEME_NAME>_<COLOR_NAME>"><COLOR_VALUE></color>`
    
        For example: 
        ```
        <color name=”holo_blue_dark”>#ff0099cc</color> 
        <color name=”material_blue_500”>#5677fc</color>
        ```

    - If the color is not in the theme: 
      
      `<color name="<COLOR_NAME>"><COLOR_VALUE></color>`

 - values/strings.xml
    - `<string name="title_<TITLE_NAME>"><TITLE_VALUE></string>` - for ActionBar title
    - `<string name="action_<ACTION_BUTTON_TEXT>"><TEXT_VALUE></string>` - for ActionBar button text
    - `<string name="tab_<ACTION_TAB_TEXT>"><TEXT_VALUE></string>` - for ActionBar.Tab text
    - `<string name="btn_<BUTTON_TEXT>"><TEXT_VALUE></string>`- for button
    - `<string name="empty_<VIEW_NAME>"><EMPTY_VALUE></string>` - for empty view
    - `<string name="hint_<EDITTEXT_NAME>"><HINT_VALUE></string>`- for the hint of EditText/AutoCompleteTextView
    - `<string name="label_<TEXTVIEW_NAME>"><TEXT_VALUE></string>`- for static TextView
    - `<string name="toast_<TOAST_NAME>"><TOAST_VALUE></string>` - for toast
    - `<string name="dialog_title_<DIALOG_NAME>"><TITLE_VALUE></string>`- for dialog
    - `<string name="dialog_msg_<DIALOG_NAME>"><MSG_VALUE></string>` - for dialog
    - `<string name="dialog_action_<ACTION_NAME>"><ACTION_NAME></string>` - for dialog button
    - `<string name="msg_<MESSAGE_NAME>"><MSG_VALUE></string>` - for Log or some other stuff
    - `<string name="contextual_<MENU_ITEM_NAME>"><TEXT_VALUE></string>`- for contextual menu item
    - `<string name="popup_<MENU_ITEM_NAME>"><TEXT_VALUE></string>` - for popup menu item
    
 - values/string_arrays.xml

    `<string-array name="<ARRAY_NAME>_array">`

 - values/plurals.xml

    `<plurals name="<PLURALS_NAME>">`
    
<!-- values/attrs.xml values/dimens.xml values/styles.xml values/themes.xml values/ids.xml values/bools.xml -->

## XML Files (res/xml)

 - `appwidget_<APPWIDGET_NAME>` - for app widget provider

  [1]:http://www.javapractices.com/topic/TopicAction.do;jsessionid=0BF4844350780B6F55476E1137FF4893?Id=205
  [2]:http://petrnohejl.github.io/Android-Cheatsheet-For-Graphic-Designers/#naming-conventions
