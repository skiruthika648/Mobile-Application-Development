# Mobile-Application-Development
# Ex.No:1
To create a HelloWorld Activity using all lifecycles methods to display messages.
# AIM:
To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.
# EQUIPMENTS REQUIRED:
Latest Version Android Studio
# ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.
# PROGRAM:
Program to print the text “Hello World”.
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
# OUTPUT:
![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/5349f027-3bc0-425b-a692-3a44bbf5cf69)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/2592f230-2adc-482c-b7ce-ebe56e96d6ce)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/8fc3cdad-c5e3-4ee3-be80-e8903aef85e3)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/89a589ec-53ab-47c1-b97f-cd367f4df6d3)



![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/b7a591a0-ae42-4843-8d36-88ddbbe41780)


![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/c99fdb32-f28e-4f4c-b1af-70b17fab5482)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/512daad8-872b-4ec7-b7d4-cc6fcc1b66f8)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/86a787b4-aec5-472d-8931-ed830edee65b)

![image](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/5267d3ea-4e5b-40de-94b6-58e7bbb51ba9)

# RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.








