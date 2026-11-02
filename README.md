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
Developed by:IYYAPPAN S
Registeration Number : 212225230108
*/
```
MainActivity.java
```
package com.example.exp_1;

import android.os.Bundle;

import androidx.appcompat.app.AppCompatActivity;

import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onResume() {
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();
    }

    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```
activity_main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#DB0505"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="serif"
        android:text="hello world"
        android:textColor="#B60FC8"
        android:textSize="24sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```


## OUTPUT

<img width="1920" height="1080" alt="690291322-5829184d-deb2-4147-b317-62b1d51531be" src="https://github.com/user-attachments/assets/c31f5637-1730-423e-8062-650582313165" />
<img width="1920" height="1080" alt="690291850-3932f15b-fb28-4a65-8973-3e006c6d5a29" src="https://github.com/user-attachments/assets/e2779e6d-2176-46e3-be66-4c15ae1b5c60" />
<img width="1920" height="1080" alt="690292136-467b21c2-59df-4ede-926f-6d84975de0c0" src="https://github.com/user-attachments/assets/398e680f-7d1d-470f-9b30-26d74a3243e9" />
<img width="1920" height="1080" alt="690292634-cc212efc-a968-4e42-8a24-5099d17c4a51" src="https://github.com/user-attachments/assets/4c506846-43bc-4d50-b04c-82624178ef8c" />
<img width="1920" height="1080" alt="690293422-408531f3-277b-46fc-b1ac-b140a1507e6a" src="https://github.com/user-attachments/assets/a82dae1a-1b05-4791-9350-8b6d9baed4a8" />



## RESULT
Thus a Simple Android Application create a **HelloWorld** Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
