# Curve View
This view used to draw custom backgrounds that support:

1. curved shapes
2. gradient colors
3. shadow of different colors


# Example
<img style="float: right;" src="whatever.jpg">
```XML
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:clipChildren="false">


    <com.haytham.coder.curveview.CurveView
        android:id="@+id/curvedView"
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_marginBottom="100dp"
        app:startColor="#FFA78B"
        app:startColorX="0.5"
        app:startColorY="-25"
        app:endColor="#DE9BE8"
        app:endColorX="0.5"
        app:endColorY="25"
        app:firstControlPointExtraY="60dp"
        app:firstControlPointX="0.4"
        app:secondControlPointExtraY="-60dp"
        app:secondControlPointX="0.6"
        app:curveShadowColor="#DE9BE8"
        app:curveShadowRadius="24dp"
        app:layout_constraintBottom_toTopOf="@+id/curvedView2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.0"
        app:layout_constraintVertical_chainStyle="spread_inside"
        />

    <com.haytham.coder.curveview.CurveView
        android:id="@+id/curvedView2"
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_marginBottom="16dp"
        android:elevation="8dp"
        app:startColor="#FFA78B"
        app:endColor="#FFA78B"
        app:firstControlPointExtraY="150dp"
        app:firstControlPointX="0.4"
        app:secondControlPointExtraY="150dp"
        app:secondControlPointX="0.6"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/curvedView"
        app:layout_constraintVertical_bias="0.496"
        />

</androidx.constraintlayout.widget.ConstraintLayout>
```
