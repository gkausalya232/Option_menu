# Ex.No:10 To create a option menu to display menu items.


## AIM:

To create a option menu to display menu items using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as “optionmenu″ and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Design option layout in option.xml.

Step 7: Add and Display option menu in MainActivity file.

Step 8: Save and run the application.


## PROGRAM:
```
/*
Program to print the text “optionmenu”.
Developed by:Kausalya G
Registeration Number :212221040076
*/
```
## Activity_xml File:
```
Activity_xml File:
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">

<ImageView
    android:id="@+id/imageView"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:src="@drawable/amgus"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    tools:srcCompat="@tools:sample/avatars" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## OPTION XML CODE:
```
OPTION XML CODE:
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
<item android:title="PRIME 1" />
<item android:title="PRIME 2" />
<item android:title="PRIME 3" />
</menu>
```
## MainActivity.java:
```
MainActivity.java:
  package com.example.menuapp;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.Menu;
import android.view.MenuInflater;

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

![WhatsApp Image 2023-06-11 at 18 07 57](https://github.com/gkausalya232/Option_menu/assets/133086820/3ba8b5c6-b53a-446a-9236-007455ef803d)
![WhatsApp Image 2023-06-11 at 18 08 38](https://github.com/gkausalya232/Option_menu/assets/133086820/c9d73fa8-658e-429a-8fab-6e07270d0b8b)



## RESULT
Thus a Simple Android Application to create a option menu to display menu items using Android Studio is developed and executed successfully.

