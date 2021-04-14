
# Rapport Assignment 3: Widgets



I stared by changing the existing layout to linearlayout, Because i wanted all the
element to be places vertically after each other.
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:app="http://schemas.android.com/apk/res-auto"
```

I added a ImageView and made a map called drawable-hdpi inside the res map in my project files.
I could then use the picture inside my ImageView by using the " android:src="@drawable/""
code line and just add the mane of the picture
I also styled the picture to be in the center.
```
 <ImageView
        android:id="@+id/picture"
        android:layout_width="match_parent"
        android:layout_height="300dp"
        android:src="@drawable/pillar"
        android:layout_centerInParent="true"
        android:contentDescription="a picture" />
```

After that I added a TextView and styled it to be a tittle for the information i was going to put in after.
i med the text, bold, change the font size, typeface and i also change background color and made the text centered.

```
 <TextView
        android:id="@+id/title_Window"
        android:text="Pillar 2: BODY"
        android:textStyle="bold"
        android:layout_margin="15dp"
        android:textColor="#FFFFFF"
        android:background="#36393F"
        android:textSize="25sp"
        android:typeface="serif"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:gravity="center" />
```

As the last thing i wanted to ad a scrollable text with information.
It was tricky to get the scrollview active and working.
I realized in the end that i didn't have a ending tag for the scrollview,
this because i didn't drag and drop the pallet, and i was sure we learn that we don't need a ending tag
when working with styling in android. Inside the scrollview i added another text view and style it so
that the text would be padding in a bit on the sides. To be able to have a lot of text i also put the text information
inside the string.xml file simply by making a string tag added a name and pasted in the text and
just called the information from the file using the code line "android:text="@string/message".

```
  <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent">

        <TextView
            android:id="@+id/message_Window"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:layout_gravity="center"
            android:layout_marginTop="20dp"
            android:paddingLeft="10dp"
            android:paddingRight="10dp"
            android:text="@string/message"
            android:textColor="#FFFFFF" />

    </ScrollView>
```

```
 <string name="message">
         the problem however is that processed food manufacturies know this and have muddied...\n\n
    </string>
```

![bild.png]

