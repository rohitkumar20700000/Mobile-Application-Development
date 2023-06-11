# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: Rohit kumar.M
Registeration Number :212221220045
*/
```
## Activity_main.xml:-
```
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">

<TextView
    android:id="@+id/head"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:fontFamily="@font/arbutus_slab"
    android:text="Mobile Application Development"
    android:textColor="@color/Maroon"
    android:textSize="20sp"
    app:layout_constraintBottom_toTopOf="@+id/body"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />

<TextView
    android:id="@+id/body"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:layout_marginBottom="356dp"
    android:fontFamily="@font/expletus_sans_medium"
    android:text="HELLO WORLD"
    android:textColor="@color/MediumTurquoise"
    android:textSize="20sp"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.498"
    app:layout_constraintStart_toStartOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## Main_Activity.java :
```

package com.example.My Application;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle; import android.widget.Toast;
public class MainActivity extends AppCompatActivity {

@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    Toast t = Toast.makeText(getApplicationContext(),"onCreate Called",Toast.LENGTH_LONG);
    t.show();
}

protected void onStart(){
    super.onStart();
    Toast t = Toast.makeText(getApplicationContext(),"onStart Called",Toast.LENGTH_LONG);
    t.show();
}

protected void onRestart(){
    super.onRestart();
    Toast t = Toast.makeText(getApplicationContext(),"onRestart Called",Toast.LENGTH_LONG);
    t.show();
}

protected void onPause(){
    super.onPause();
    Toast t = Toast.makeText(getApplicationContext(),"onPause Called",Toast.LENGTH_LONG);
    t.show();
}

protected void onResume(){
    super.onResume();
    Toast t = Toast.makeText(getApplicationContext(),"onResume Called",Toast.LENGTH_LONG);
    t.show();
}

protected void onStop(){
    super.onStop();
    Toast t = Toast.makeText(getApplicationContext(),"onStop Called",Toast.LENGTH_LONG);
    t.show();
}

protected void onDestroy(){
    super.onDestroy();
    Toast t = Toast.makeText(getApplicationContext(),"onDestroy Called",Toast.LENGTH_LONG);
    t.show();
}
}
```

## OUTPUT:

## onStart()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/3858cc64-15b0-4be2-8425-a178ddbb5fb4)

## onCreate()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/8431d341-58ea-4630-aaef-509be30ff2b1)

## onRestart()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/533a3bf4-7a74-437b-817f-f542b0f2b6cc)

## onPause()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/efedec58-6dd0-4c5f-8a0f-ad7a3f64c217)

## onResume()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/a18e8568-7622-4e23-8458-16889c617ab3)

## onDestroy()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/9171418f-4bcf-4e7a-b560-9c5b97b54d31)

## onStop()
![image](https://github.com/nithish143257/Mobile-Application-Development/assets/113762839/6b5bea50-1a8d-4666-b650-724ad9633c70)

## RESULT:
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
