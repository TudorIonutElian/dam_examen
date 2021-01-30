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

### Shared Preferences
#### Creare si Salvare
```java

    public void salveazaSetariCaPreferinte(){
        SharedPreferences sharedPreferences = getSharedPreferences("shared_preferences", MODE_PRIVATE);
        SharedPreferences.Editor editor = sharedPreferences.edit();

        editor.putBoolean(SALVEAZA_KILOGRAME, salveazaNumarKilograme.isChecked());
        editor.put(SALVEAZA_SPORT, salveazaNumarOreSport.isChecked());
        editor.putBoolean(SALVEAZA_ODIHNA, salveazaNumarOreOdihna.isChecked());
        editor.putBoolean(SALVEAZA_CALORII, salveazaNumarCalorii.isChecked());

        editor.commit();
        this.finish();
        Toast.makeText(getApplicationContext(), getText(R.string.preferences_setari_salvate), Toast.LENGTH_LONG).show();
    }
```

#### Preluare Shared Preferences si Aplicare valori pe elemente

```java

   public void preluareSetariPreferinte(){
        SharedPreferences sharedPreferences = getSharedPreferences("shared_preferences", MODE_PRIVATE);
        // Setare Kilograme
        boolean setareKilograme = sharedPreferences.getBoolean(SALVEAZA_KILOGRAME, false);
        if(setareKilograme){
            salveazaNumarKilograme.setText(getText(R.string.set_mesaj_text_DA));
            salveazaNumarKilograme.setTextColor(getResources().getColor(R.color.colorGreen));
        }else {
            salveazaNumarKilograme.setText(getText(R.string.set_mesaj_text_NU));
            salveazaNumarKilograme.setTextColor(getResources().getColor(R.color.colorRed));
        }
        salveazaNumarKilograme.setChecked(setareKilograme);

        // Setare sport
        boolean setareSport = sharedPreferences.getBoolean(SALVEAZA_SPORT, false);
        if(setareSport){
            salveazaNumarOreSport.setText(getText(R.string.set_mesaj_text_DA));
            salveazaNumarOreSport.setTextColor(getResources().getColor(R.color.colorGreen));
        }else {
            salveazaNumarOreSport.setText(getText(R.string.set_mesaj_text_NU));
            salveazaNumarOreSport.setTextColor(getResources().getColor(R.color.colorRed));
        }
        salveazaNumarOreSport.setChecked(setareSport);

        // Setare odihna
        boolean setareOdihna = sharedPreferences.getBoolean(SALVEAZA_ODIHNA, false);
        if(setareOdihna){
            salveazaNumarOreOdihna.setText(getText(R.string.set_mesaj_text_DA));
            salveazaNumarOreOdihna.setTextColor(getResources().getColor(R.color.colorGreen));
        }else {
            salveazaNumarOreOdihna.setText(getText(R.string.set_mesaj_text_NU));
            salveazaNumarOreOdihna.setTextColor(getResources().getColor(R.color.colorRed));
        }
        salveazaNumarOreOdihna.setChecked(setareOdihna);

        // Setare calorii
        boolean setareCalorii = sharedPreferences.getBoolean(SALVEAZA_CALORII, false);
        if(setareCalorii){
            salveazaNumarCalorii.setText(getText(R.string.set_mesaj_text_DA));
            salveazaNumarCalorii.setTextColor(getResources().getColor(R.color.colorGreen));
        }else {
            salveazaNumarCalorii.setText(getText(R.string.set_mesaj_text_NU));
            salveazaNumarCalorii.setTextColor(getResources().getColor(R.color.colorRed));
        }
        salveazaNumarCalorii.setChecked(setareCalorii);
    }
```

### Clasa Java pentru implementare SQLite
```java
public class DatabaseHelper extends SQLiteOpenHelper {
    public static final String DATABASE_NAME = "map.db";
    public static final String MAP_TABLE_NAME = "map_data";
    public static final String MAP_TABLE_NAME_WORKING = "map_data_WORKING";
    public static final String MAP_COLUMN_ID = "id";
    public static final String MAP_COLUMN_DATE = "data";
    public static final String MAP_COLUMN_KG = "kg";

    public static final String MAP_COLUMN_SPORT = "sport";
    public static final String MAP_COLUMN_ODIHNA = "odihna";
    public static final String MAP_COLUMN_CALORII = "calorii";
    public static final String MAP_COLUMN_COEFCIENT = "coeficient";


    private HashMap hp;

    public DatabaseHelper(Context context) {
        super(context, DATABASE_NAME , null, 1);
    }

    public DatabaseHelper(@Nullable Context context, @Nullable String name, @Nullable SQLiteDatabase.CursorFactory factory, int version) {
        super(context, name, factory, version);
        SQLiteDatabase db = this.getWritableDatabase();
    }

    @Override
    public void onCreate(SQLiteDatabase db) {
        // TODO Auto-generated method stub
        db.execSQL(
                "create table " + MAP_TABLE_NAME +
                        " (" +
                        MAP_COLUMN_ID + " integer primary key, " +
                        MAP_COLUMN_DATE + " String, " +
                        MAP_COLUMN_KG + " integer, " +
                        MAP_COLUMN_SPORT + " integer, " +
                        MAP_COLUMN_ODIHNA + " integer, " +
                        MAP_COLUMN_CALORII + " integer, " +
                        MAP_COLUMN_COEFCIENT + " decimal(2,2)" +")"
        );
    }

    @Override
    public void onUpgrade(SQLiteDatabase db, int oldVersion, int newVersion) {
        // TODO Auto-generated method stub
        db.execSQL("DROP TABLE IF EXISTS " + MAP_TABLE_NAME );
        onCreate(db);
    }

    // Preluare Toate inregistrarile
    public Cursor getData() {
        SQLiteDatabase db = this.getReadableDatabase();
        Cursor res =  db.rawQuery("SELECT * FROM " + MAP_TABLE_NAME, null);
        return res;
    }

    // Get numar inregistrari
    public int numberOfRows(){
        SQLiteDatabase db = this.getReadableDatabase();
        int numRows = (int) DatabaseUtils.queryNumEntries(db, MAP_TABLE_NAME);
        return numRows;
    }

    // Preluare Date activitate personala by ID
    public Cursor getActivitateById(int id_editare){
        SQLiteDatabase db = this.getReadableDatabase();
        Cursor res =  db.rawQuery("SELECT * FROM " + MAP_TABLE_NAME + " WHERE " + MAP_COLUMN_ID + " = " + id_editare,
                null);
        return res;
    }

    // Inserare activitate noua
    public boolean inserareActivitate(ActivitatePersonala activitatePersonala){
        SQLiteDatabase db = this.getWritableDatabase();
        ContentValues contentActivitate = new ContentValues();

        contentActivitate.put(MAP_COLUMN_DATE, activitatePersonala.getData_adaugarii());
        contentActivitate.put(MAP_COLUMN_KG, activitatePersonala.getNumar_kilograme());
        contentActivitate.put(MAP_COLUMN_SPORT, activitatePersonala.getNumar_ore_sport());
        contentActivitate.put(MAP_COLUMN_ODIHNA, activitatePersonala.getNumar_ore_odihna());
        contentActivitate.put(MAP_COLUMN_CALORII, activitatePersonala.getNumar_calorii_consumate());
        contentActivitate.put(MAP_COLUMN_COEFCIENT, activitatePersonala.getValoare_coeficient());
        long rezultat = 0;
        try{
           rezultat = db.insert(MAP_TABLE_NAME, null, contentActivitate);
        }catch (Exception ex){
            Log.d("Excep", ex.getMessage());
        }
        if(rezultat == 0){
            return true;
        }else{
            return false;
        }

    }
    // Stergere activitate by ID
    public boolean stergereActivitate(int idStergere){
        SQLiteDatabase db = this.getWritableDatabase();
        db.execSQL("DELETE FROM " + MAP_TABLE_NAME + " WHERE " + MAP_COLUMN_ID + " = "+ idStergere +"");
        db.close();
        return true;
    }

    // Update actualizare
    public boolean updateActivitate(int id_editare, ActivitatePersonala activitatePersonala){
        SQLiteDatabase db = this.getWritableDatabase();
        ContentValues dataUpdate = new ContentValues();

        dataUpdate.put(MAP_COLUMN_DATE, activitatePersonala.getData_adaugarii());
        dataUpdate.put(MAP_COLUMN_KG, activitatePersonala.getNumar_kilograme());
        dataUpdate.put(MAP_COLUMN_SPORT, activitatePersonala.getNumar_ore_sport());
        dataUpdate.put(MAP_COLUMN_ODIHNA, activitatePersonala.getNumar_ore_odihna());
        dataUpdate.put(MAP_COLUMN_CALORII, activitatePersonala.getNumar_calorii_consumate());
        dataUpdate.put(MAP_COLUMN_COEFCIENT, activitatePersonala.getValoare_coeficient());
        db.update(MAP_TABLE_NAME, dataUpdate, MAP_COLUMN_ID + "= ?", new String[]{String.valueOf(id_editare)});

        db.close();
        return true;
    }
}

```