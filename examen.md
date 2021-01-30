# Examen Dispozitive si Aplicatii Mobile <br>

## Cerinta 1
> Se va defini o clasa cu minim cinci atribute relevante, din domeniul dat, pentru care se vor implementa/genera constructori, metoda  *toString()* si functii accesor(metode get(), set()) **(1p)**.

```java
public class ClasaExamen {
    private int proprietate_int_1;
    private int proprietate_int_2;
    private String proprietate_string;
    private Date proprietate_date;
    private TipProprietate proprietate_tip;

    public ClasaExamen(int proprietate_int_1, int proprietate_int_2, String proprietate_string, Date proprietate_date, TipProprietate proprietate_tip) {
        this.proprietate_int_1 = proprietate_int_1;
        this.proprietate_int_2 = proprietate_int_2;
        this.proprietate_string = proprietate_string;
        this.proprietate_date = proprietate_date;
        this.proprietate_tip = proprietate_tip;
    }

    public int getProprietate_int_1() {
        return proprietate_int_1;
    }

    public void setProprietate_int_1(int proprietate_int_1) {
        this.proprietate_int_1 = proprietate_int_1;
    }

    public int getProprietate_int_2() {
        return proprietate_int_2;
    }

    public void setProprietate_int_2(int proprietate_int_2) {
        this.proprietate_int_2 = proprietate_int_2;
    }

    public String getProprietate_string() {
        return proprietate_string;
    }

    public void setProprietate_string(String proprietate_string) {
        this.proprietate_string = proprietate_string;
    }

    public Date getProprietate_date() {
        return proprietate_date;
    }

    public void setProprietate_date(Date proprietate_date) {
        this.proprietate_date = proprietate_date;
    }

    public TipProprietate getProprietate_tip() {
        return proprietate_tip;
    }

    public void setProprietate_tip(TipProprietate proprietate_tip) {
        this.proprietate_tip = proprietate_tip;
    }

    @Override
    public String toString() {
        return "ClasaExamen{" +
                "proprietate_int_1=" + proprietate_int_1 +
                ", proprietate_int_2=" + proprietate_int_2 +
                ", proprietate_string='" + proprietate_string + '\'' +
                ", proprietate_date=" + proprietate_date +
                ", proprietate_tip=" + proprietate_tip +
                '}';
    }
}
```

## Cerinta 2
> Se va crea o activitate de preluare a datelor care va include obligatoriu controalele alocate, pe langa alte controale adecvate **(1p)**.

### TextView
```xml

<TextView
        android:id="@+id/idTextViewNou"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="32dp"
        android:gravity="center_horizontal|center_vertical"
        android:text="Text de Salvat in Strings"
        app:layout_constraintEnd_toStartOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="parent" />

```

### Switch

```xml
<Switch
        android:id="@+id/idSwitchNou"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="84dp"
        android:text="Text de Salvat in Strings"
        android:textColor="@android:color/holo_orange_dark"
        app:layout_constraintHorizontal_bias="0.509"
        app:layout_constraintEnd_toStartOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="parent" />
```


### Button

```xml
<Button
        android:id="@+id/idButtonNou"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginTop="164dp"
        android:background="@color/colorRed"
        android:text="@string/reseteaza_setari"
        android:textColor="@android:color/background_light"
        android:textStyle="bold"
        app:layout_constraintEnd_toStartOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="parent" />
```

### Vertical Guideline

```xml
    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/idGuidelineNou"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintGuide_percent="0.6" />
```


### TextView

```xml
 <TextView
        android:id="@+id/idTextViewNou"
        android:layout_width="220dp"
        android:layout_height="49dp"
        android:layout_marginTop="12dp"
        android:gravity="center_horizontal|center_vertical"
        android:text="@string/coeficient_date"
        android:textColor="@android:color/holo_red_dark"
        app:layout_constraintEnd_toStartOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="parent" />
```

### EditText

```xml
<EditText
        android:id="@+id/idEditTextNou"
        android:layout_width="0dp"
        android:layout_height="50dp"
        android:layout_marginStart="15dp"
        android:layout_marginLeft="15dp"
        android:layout_marginTop="20dp"
        android:layout_marginEnd="15dp"
        android:layout_marginRight="15dp"
        android:contentDescription="@string/nr_kg"
        android:ems="10"
        android:importantForAutofill="no"
        android:inputType="number"
        app:layout_constraintEnd_toStartOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="parent" />
```

### ImageView

```xml
    <ImageView
        android:id="@+id/idImageViewNou"
        android:layout_width="86dp"
        android:layout_height="42dp"
        android:layout_marginStart="8dp"
        android:layout_marginLeft="8dp"
        android:layout_marginTop="196dp"
        android:contentDescription="@string/vizualizare_map"
        app:layout_constraintStart_toStartOf="@+id/leftGuide"
        app:layout_constraintTop_toTopOf="parent"
        app:srcCompat="@drawable/vizualizare" />
```


### TextInputLayout

```xml
    <com.google.android.material.textfield.TextInputLayout
        android:id="@+id/idEditTextNou"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_marginTop="32dp"
        android:layout_marginStart="50dp"
        android:layout_marginEnd="50dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/btnImagineMAP">

        <com.google.android.material.textfield.TextInputEditText
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:hint="hint" />
    </com.google.android.material.textfield.TextInputLayout>
```

### String Array

```xml
    <string-array name="dropdown_items">
        <item name="optiune-1">Optiune 1</item>
        <item name="optiune-2">Optiune 2</item>
        <item name="optiune-3">Optiune 3</item>
        <item name="optiune-4">Optiune 4</item>
        <item name="optiune-5">Optiune 5</item>
        <item name="optiune-6">Optiune 6</item>
    </string-array>

```