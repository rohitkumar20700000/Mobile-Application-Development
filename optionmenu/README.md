# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as OptionMenu and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Create a option.xml file to create options in your menu.

Step 7: Display options in MainActivity file.

Step 8: Save and run the application.


## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by: Rohit kumar.M
Registeration Number : 212221220045
*/
```
activtity_main.xml:

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"/>
```
option.xml:

```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
    <item android:title="@string/item_1" />
    <item android:title="@string/item_2" />
    <item android:title="@string/item_3" />
</menu>
```

MainActivity.java:

```
package com.example.optionmenu;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

import com.example.optionmenu.R;

public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }
    @Override
    public boolean onCreateOptionsMenu(Menu menu) {
        MenuInflater m = getMenuInflater();
        m.inflate(R.menu.option,menu);
        return true;
    }
}
```
## OUTPUT

![image](https://github.com/kannan0071/MAD-Ex.No-10/assets/119641638/31b526e6-c0b8-4db3-b190-3258743d7f1e)

![image](https://github.com/kannan0071/MAD-Ex.No-10/assets/119641638/5b0ad7a8-b92f-489b-b221-88bce95e51cf)

![image](https://github.com/kannan0071/MAD-Ex.No-10/assets/119641638/3c21ac8e-18a0-43c0-b79c-1356b42f7e49)

![WhatsApp Image 2023-05-25 at 14 13 27](https://github.com/kannan0071/MAD-Ex.No-10/assets/119641638/7d90553e-3990-4621-b5cc-553d19640297)

![WhatsApp Image 2023-05-25 at 14 13 27](https://github.com/kannan0071/MAD-Ex.No-10/assets/119641638/3c257b09-4978-4d41-baff-6214a68e01c8)

## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.

