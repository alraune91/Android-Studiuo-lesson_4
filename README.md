package com.example.as_project_4;

import androidx.appcompat.app.AppCompatActivity;
import androidx.core.content.ContextCompat;

import android.content.Context;
import android.os.Bundle;
import android.view.View;
import android.widget.LinearLayout;
import android.widget.TextView;



public class MainActivity extends AppCompatActivity {
    private LinearLayout mLL;
    private TextView mTV;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        mLL = findViewById(R.id.linearLayout);
        mTV = findViewById(R.id.textView);
    }
    public void onClick(View v) {
        int id = v.getId();
        if (id == R.id.buttonRed) {
            mTV.setText(R.string.red);
            mLL.setBackgroundColor(ContextCompat.getColor(this, R.color.red));
        } else if (id == R.id.buttonYellow) {
            mTV.setText(R.string.yellow);
            mLL.setBackgroundColor(ContextCompat.getColor(this, R.color.yellow));
        } else if (id == R.id.buttonGreen) {
            mTV.setText(R.string.green);
            mLL.setBackgroundColor(ContextCompat.getColor(this, R.color.green));
        }
    }
}# Android-Studiuo-lesson_4
