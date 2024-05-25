<p align="center">
<p align="center">
  <a href="https://github.com/i-rin-eam">
    <img src="https://avatars.githubusercontent.com/u/154800878?s=400&u=5d18880cc28646190a19a971bfcdbc54644eab07&v=4" alt="Logo" width="100" height="100">
  </a> 
<h1 align='center'>Practice Challenge 7 Soltuion</h1>
<h3 align='center'>
   Visit my youtube channel <a href="https://www.youtube.com/@LearnWithYeamin">Learn With Yeamin</a>
</h3>
</p>

## Step 1: Here is `activity_main.xml` code.
```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="horizontal"
    android:weightSum="1.8"
    tools:context=".MainActivity">

    <LinearLayout
        android:layout_width="0dp"
        android:layout_height="match_parent"
        android:layout_weight=".8"
        android:orientation="vertical">

        <ScrollView
            android:layout_width="match_parent"
            android:layout_height="match_parent">

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="match_parent"
                android:orientation="vertical"
                android:paddingHorizontal="5dp"
                android:paddingBottom="5dp">

                <ImageView
                    android:id="@+id/imgMohammadNaim"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:paddingTop="5dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_mohammad_naim" />

                <ImageView
                    android:id="@+id/imgLitonDas"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_liton_das" />

                <ImageView
                    android:id="@+id/imgShakibAlHasan"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_shakib_al_hasan" />

                <ImageView
                    android:id="@+id/imgMushfiqurRahim"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_mushfiqur_rahim" />

                <ImageView
                    android:id="@+id/imgMahmudullahRiyad"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_mahmudullah_riyad" />

                <ImageView
                    android:id="@+id/imgAfifHossain"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_afif_hossain" />

                <ImageView
                    android:id="@+id/imgNurulHasan"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_nurul_hasan" />

                <ImageView
                    android:id="@+id/imgMahediHasan"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_mahedi_hasan" />

                <ImageView
                    android:id="@+id/imgMohammadSaifuddin"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_mohammad_saifuddin" />

                <ImageView
                    android:id="@+id/imgMustafizurRahman"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_mustafizur_rahman" />

                <ImageView
                    android:id="@+id/imgNasumAhmed"
                    android:layout_width="match_parent"
                    android:layout_height="200dp"
                    android:scaleType="centerCrop"
                    android:src="@drawable/img_nasum_ahmed" />
            </LinearLayout>
        </ScrollView>

    </LinearLayout>

    <LinearLayout
        android:layout_width="0dp"
        android:layout_height="match_parent"
        android:layout_weight="1"
        android:orientation="vertical"
        android:padding="5dp">

        <ImageView
            android:id="@+id/playerImage"
            android:layout_width="match_parent"
            android:layout_height="250dp"
            android:scaleType="centerCrop"
            android:src="@drawable/img_shakib_al_hasan" />

        <TextView
            android:id="@+id/playerName"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Player Name"
            android:textSize="16sp"
            android:textStyle="bold" />

        <TextView
            android:id="@+id/playerType"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Player Type"
            android:textSize="14sp" />

        <TextView
            android:id="@+id/playerDescription"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Player Description"
            android:textSize="12sp" />
    </LinearLayout>

</LinearLayout>
```

## Step 2: Here is `MainActivity.java` code.
```java
package com.myeamin.practicechallenge7;

import android.os.Bundle;
import android.view.View;
import android.widget.ImageView;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    private ImageView playerImage;
    private TextView playerName, playerType, playerDescription;
    private ImageView imgMohammadNaim, imgLitonDas, imgShakibAlHasan, imgMushfiqurRahim, imgMahmudullahRiyad;
    private ImageView imgAfifHossain, imgNurulHasan, imgMahediHasan, imgMohammadSaifuddin, imgMustafizurRahman, imgNasumAhmed;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        playerImage = findViewById(R.id.playerImage);
        playerName = findViewById(R.id.playerName);
        playerType = findViewById(R.id.playerType);
        playerDescription = findViewById(R.id.playerDescription);

        imgMohammadNaim = findViewById(R.id.imgMohammadNaim);
        imgLitonDas = findViewById(R.id.imgLitonDas);
        imgShakibAlHasan = findViewById(R.id.imgShakibAlHasan);
        imgMushfiqurRahim = findViewById(R.id.imgMushfiqurRahim);
        imgMahmudullahRiyad = findViewById(R.id.imgMahmudullahRiyad);
        imgAfifHossain = findViewById(R.id.imgAfifHossain);
        imgNurulHasan = findViewById(R.id.imgNurulHasan);
        imgMahediHasan = findViewById(R.id.imgMahediHasan);
        imgMohammadSaifuddin = findViewById(R.id.imgMohammadSaifuddin);
        imgMustafizurRahman = findViewById(R.id.imgMustafizurRahman);
        imgNasumAhmed = findViewById(R.id.imgNasumAhmed);

        imgMohammadNaim.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_mohammad_naim);
                playerName.setText("Mohammad Naim");
                playerType.setText("Batsman");
                playerDescription.setText("An aggressive top-order batsman.");
            }
        });

        imgLitonDas.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_liton_das);
                playerName.setText("Liton Das");
                playerType.setText("Wicketkeeper-Batsman");
                playerDescription.setText("A talented wicketkeeper-batsman.");
            }
        });

        imgShakibAlHasan.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_shakib_al_hasan);
                playerName.setText("Shakib Al Hasan");
                playerType.setText("All-rounder");
                playerDescription.setText("One of the best all-rounders in the world.");
            }
        });

        imgMushfiqurRahim.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_mushfiqur_rahim);
                playerName.setText("Mushfiqur Rahim");
                playerType.setText("Wicketkeeper-Batsman");
                playerDescription.setText("A reliable middle-order batsman.");
            }
        });

        imgMahmudullahRiyad.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_mahmudullah_riyad);
                playerName.setText("Mahmudullah Riyad");
                playerType.setText("Batsman");
                playerDescription.setText("The captain and a dependable batsman.");
            }
        });

        imgAfifHossain.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_afif_hossain);
                playerName.setText("Afif Hossain");
                playerType.setText("All-rounder");
                playerDescription.setText("A versatile young all-rounder.");
            }
        });

        imgNurulHasan.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_nurul_hasan);
                playerName.setText("Nurul Hasan");
                playerType.setText("Wicketkeeper");
                playerDescription.setText("A skilled wicketkeeper.");
            }
        });

        imgMahediHasan.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_mahedi_hasan);
                playerName.setText("Mahedi Hasan");
                playerType.setText("Bowler");
                playerDescription.setText("A promising off-spinner.");
            }
        });

        imgMohammadSaifuddin.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_mohammad_saifuddin);
                playerName.setText("Mohammad Saifuddin");
                playerType.setText("All-rounder");
                playerDescription.setText("A talented all-rounder.");
            }
        });

        imgMustafizurRahman.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_mustafizur_rahman);
                playerName.setText("Mustafizur Rahman");
                playerType.setText("Bowler");
                playerDescription.setText("A left-arm fast bowler known for his cutters.");
            }
        });

        imgNasumAhmed.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                playerImage.setImageResource(R.drawable.img_nasum_ahmed);
                playerName.setText("Nasum Ahmed");
                playerType.setText("Bowler");
                playerDescription.setText("A talented left-arm spinner.");
            }
        });
    }
}
```
## Authors

**MD YEAMIN** - Android Software Developer <a href="https://www.youtube.com/@LearnWithYeamin">**(Learn With Yeamin)**</a> 

<h1 align="center">Thank You ❤️</h1>
