# DEBA-HTML
&nbsp;
Simple and fast way to create android button with icon, radius, background 



&nbsp;
### Features!
- Drawable Resource - position, padding
- Font Awesome Icon - color, position, padding
- Radius, Background and Focus color
- Border - color and width
- Text - normal color, disable color,  size, style, AllCaps 

&nbsp;
### Screenshot
![Styles Button Screenshot](https://raw.githubusercontent.com/debashissabar7/Styles-Button-/052529ce536f6192cfa001ce3eddda6441bb5dac/debashissabar7-Styles-Button.png)

&nbsp;
### Install

&nbsp;
#### Gradle 
```java
allprojects {
   repositories{
	  ...
	  maven { url 'https://jitpack.io' }
  }
}
```

```java
dependencies {
        compile 'com.github.debashissabar7:Styles-Button-:1.0.0' // AndroidX dependencies
}
```

&nbsp;
#### Maven

```xml
<dependency>
   <groupId>com.github.debashissabar7</groupId>
   <artifactId>Styles-Button-</artifactId>
   <version>1.0.0</version>
</dependency>
```

&nbsp;
### Use

&nbsp;
#### XML
Include namespace to the root View/Layout :
```xml
xmlns:app="http://schemas.android.com/apk/res-auto"
```
StylesButton with custom params

```xml
<com.debashis.styles.button.StylesButton		
  android:layout_width="150dp"
  android:layout_height="45dp"
  android:padding="10dp"
  app:debashis_text="Follow Me"
  app:debashis_borderColor="#FFFFFF"
  app:debashis_borderWidth="0dp"
  app:debashis_gravity="center"
  app:debashis_backgroundColor="#00C853"
  app:debashis_focusColor="#EEEEEE"
  app:debashis_textColor="#FFF"
  app:debashis_radius="23dp"
  android:layout_marginTop="10dp"
  app:debashis_fontIcon="&#xf023;"/>
<!--- app:debashis_fontIcon="&#x fontcode input; -->
```

&nbsp;
#### JAVA

```java
StylesButton button = new StylesButton(this);
button.setText("Submit");
button.setTextColor(Color.RED);
button.setAllCaps(true);
button.setFontIcon("\uf138");
button.setIconPosition(NoboButton.POSITION_LEFT);
button.setBackgroundColor(Color.WHITE);
button.setFocusColor(Color.GRAY);
button.setBorderColor(Color.RED);
button.setBorderWidth(2);
button.setRadius(10);
```

&nbsp;
#### Font Awesome Icon

Cheatsheet http://fontawesome.io/cheatsheet/

Note: before use **font awesome** please see their license http://fontawesome.io/license/

&nbsp;
#### Attributes
| Description (Data type) | XML Attribute | Java Attribute | 
|-------------------------------|-------------|-------------|
| Text (String) | app:text="Button Text" | setText("Submit") |
| Text color (color) |  app:textColor="#FFF" | setTextColor(Color.WHITE) |
| Text size (dimension) |  app:textSize="18sp" | setTextSize(18) |
| UPPER Text (boolean) |  app:textAllCaps="true" | setAllCaps(true) |
| Text Style (int); supported style: NORMAL, BOLD, ITALIC  |  app:textStyle="bold" | setTextStyle(NoboButton.TEXT_STYLE_BOLD) |
| border color (int) | app:borderColor="#FFF" | setBorderColor(Color.WHITE); |
| border width (dimension) | app:borderWidth="2dp" | setBorderWidth(2) |
| background color (int) | app:backgroundColor="#FF0000" | setBackgroundColor(Color.RED) |
| focus/pressed color (int) | app:focusColor="#FF4081" | setFocusColor(Color.GRAY) |
| radius of button (dimension) | app:radius="10dp" | setRadius(10) |
| disabled text color | app:disabledTextColor="#DDD" | setDisabledColor(Color.GRAY) |
| Awesome font unicode (String) | app:fontIcon="&#xf291;" | setFontIcon("\uf007"); |
| Icon drawable resource (int) | app:drawableResource="@drawable/ic_camera" | setDrawableResource(R.drawable.ic_camera) |
| Icon color (int) | app:iconColor="#FFF" | setIconColor(Color.WHITE) |
| Icon position (int); Supported position, LEFT, TOP, RIGHT, BOTTOM | app:iconPosition="left" | setIconPosition(NoboButton.POSITION_LEFT) |
| Space between icon & text (dimension) | app:iconPadding="10dp" | setIconPadding(10) |


&nbsp;
&nbsp;
## License
    Copyright 2023 Debashis Sabar
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and limitations under the License.
    
