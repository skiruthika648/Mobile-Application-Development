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
Developed by:KIRUTHIKA S
Registeration Number :212221040085
*/
```
# Activity_main.xml:
```
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">

<TextView
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:textSize="40dp"
    android:text="Hello World!"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
# MainActivity.java:
```
package com.example.helloworld;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    private static final String TAG = "HelloWorldActivity";

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.d(TAG, "onCreate: ");
        Toast.makeText(this, "onCreate", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Log.d(TAG, "onStart: ");
        Toast.makeText(this, "onStart", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onResume() {
        super.onResume();
        Log.d(TAG, "onResume: ");
        Toast.makeText(this, "onResume", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onPause() {
        super.onPause();
        Log.d(TAG, "onPause: ");
        Toast.makeText(this, "onPause", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onStop() {
        super.onStop();
        Log.d(TAG, "onStop: ");
        Toast.makeText(this, "onStop", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onDestroy() {
        super.onDestroy();
        Log.d(TAG, "onDestroy: ");
        Toast.makeText(this, "onDestroy", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onRestart() {
        super.onRestart();
        Log.d(TAG, "onRestart: ");
        Toast.makeText(this, "onRestart", Toast.LENGTH_SHORT).show();
    }
}
```


## OUTPUT
![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/60a90179-f239-417a-9de7-6e2901345bec)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/439e7e21-8340-4c9c-88af-a92ac0ac5af8)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/47d57606-9bc6-431a-aa6f-c13d7bab1631)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/bc41b3b2-cb9c-48f3-9870-bd7e12275d47)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/aa2e679a-a7a9-4c80-a3f0-703533825ad5)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/d0d02727-f299-40f9-984c-3e243ff140ab)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/32c549d0-77f0-48d5-a13c-03bce7b6f03a)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/e0e84b59-99be-42f3-bb88-6a8d27f158d0)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/07ca70e4-b8bb-4b1a-b577-9f956f244beb)






## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
