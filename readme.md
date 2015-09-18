# Ratio

Ratio is a small library that fits your image into an imageview without cropping or stretching the image while still maintaining the aspect ratio of the image. 

## How to use

To use this library simple declare a RatioLayout in your layout file like this:

```xml

    <com.fisheradelakin.material.RatioLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            app:ratio="1">

            <ImageView
                android:id="@+id/user_photo"
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:contentDescription="User photo"/>

        </com.fisheradelakin.material.RatioLayout>

```
and in your activity or fragment, you can gain access to the layout using: 

```java 

    RatioLayout rl = (RatioLayout) findViewById(R.id.ratio_layout);

```

Feel free to change the values to whatever you see fit. You can still access the imageview in the layout the same you regularly access ui elements from your activity or fragment.

You can also look at [this file]() in my bitdate project for a better understanding as to how it's used. 

That's pretty much all there is to Ratio and using Ratio. It's super small and might not have a lot of uses but I use it quite often and decided to open-source it incase people had uses for it.