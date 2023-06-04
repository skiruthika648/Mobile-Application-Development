# Ex.No:3 Develop program to create a text field and a button “Navigate”. When you enter “www.google.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the google page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:
Step 1: Open Android Studio and then click on File -> New -> New project.

Step 2: Then type the Application name as Implicit Intent and click Next.

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.


## PROGRAM:
```
/*
Program to print the text “Implicitintent”.
Developed by:KIRUTHIKA S
Registeration Number :212221040085
*/
```
# ACTIVITY_MAIN.XML
```
    <?xml version="1.0" encoding="utf-8"?>
    <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
      xmlns:app="http://schemas.android.com/apk/res-auto"
      xmlns:tools="http://schemas.android.com/tools"
      android:layout_width="match_parent"
      android:layout_height="match_parent"
      android:background="@color/background"
      tools:context=".MainActivity">

      <TextView
          android:id="@+id/textView"
          android:layout_width="263dp"
          android:layout_height="59dp"
          android:layout_marginTop="144dp"
          android:background="@color/button_background"
          android:fontFamily="@font/roboto_black"
          android:paddingTop="25px"
          android:paddingBottom="25px"
          android:text="IMPLICIT INTENT"
          android:textAlignment="center"
          android:textColor="@color/white"
          android:textSize="75px"
          app:layout_constraintEnd_toEndOf="parent"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toTopOf="parent" />

      <EditText
          android:id="@+id/editTextText"
          android:layout_width="263dp"
          android:layout_height="49dp"
          android:layout_marginTop="56dp"
          android:background="@color/button_background"
          android:ems="10"
          android:fontFamily="@font/roboto_black"
          android:hint="Enter a Website"
          android:inputType="text"
          android:textAlignment="center"
          android:textColor="@color/white"
          android:textColorHint="@color/white"
          android:textSize="75px"
          app:layout_constraintEnd_toEndOf="parent"
          app:layout_constraintHorizontal_bias="0.493"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toBottomOf="@+id/textView" />

      <Button
          android:id="@+id/button"
          android:layout_width="wrap_content"
          android:layout_height="wrap_content"
          android:text="VISIT"
          android:textColor="@color/white"
          android:background="@color/button_background"
          app:cornerRadius="0px"
          app:layout_constraintBottom_toBottomOf="parent"
          app:layout_constraintEnd_toEndOf="parent"
          app:layout_constraintStart_toStartOf="parent"
          app:layout_constraintTop_toBottomOf="@+id/editTextText"
          app:layout_constraintVertical_bias="0.258" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
# MAIN ACTIVITY.JAVA
```
package com.example.workshop_03;
import androidx.appcompat.app.AppCompatActivity;
import android.content.Intent;
import android.net.Uri;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;

public class MainActivity extends AppCompatActivity 
{
   @Override
   protected void onCreate(Bundle savedInstanceState) 
   {
      super.onCreate(savedInstanceState);
      setContentView(R.layout.activity_main);
      EditText editText = (EditText) findViewById(R.id.editTextText);
      Button btn = (Button) findViewById(R.id.button);
      btn.setOnClickListener(new View.OnClickListener() 
      {
          @Override
          public void onClick(View view) 
          {
              String url = editText.getText().toString();
              Intent i = new Intent(Intent.ACTION_VIEW, Uri.parse(url));
              startActivity(i);
          }
      });
  }
}  
```
## OUTPUT
![iia](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/a6531b4c-e8c3-4fb0-9a60-57aea393289b)

![iim](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/04da10f8-9e9b-429b-84e3-aaca7eb107d0)

![implictintent](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/b2b14b65-c6e5-4997-a5a7-6af78d3b0c3a)

![ii(1)](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/44b2297f-5005-4940-99c6-392462a3d4b1)

![ii(2)](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/bec0de25-3c45-4ebc-9573-59e2b32b92a1)

![ii(3)](https://github.com/skiruthika648/Mobile-Application-Development/assets/128348968/eebf0200-526a-4034-8a86-33e5f8236540)





## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the google page using Android Studio is developed and executed successfully.


