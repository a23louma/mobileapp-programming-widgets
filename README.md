
# Rapport

Jag började med att lägga till en LinearLayout inuti den befintliga constraintlayout i
activity_main.xml. Jag valde att ändra "orientation" till horisontell. Jag ändrade även 
bakgrundsfärgen. Se koden nedan.
```
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="horizontal"
        android:background="#a1d4e2">

    </LinearLayout>
```
Därefter lade jag till EditText med placeholder "Skriv här" i activity_main.xml. Jag valde att använda
layout_margin för att ändra placeringen. Se koden nedan.
```
        <EditText
            android:id="@+id/myEdtText"
            android:hint="Skriv här"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:inputType="text"
            android:autofillHints="text"
            android:layout_margin="20dp"/>
```
Jag skapade en Button med texten "Tryck här" i activity_main.xml. Jag ändrade färgen på knappen
och även här valde jag att använda layout_margin för placering av knappen. Se koden nedan.
```
        <Button
            android:id="@+id/myFirstBtn"
            android:text="Tryck här"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_margin="20dp"
            android:background="#2596be"/>
```      
Därefter lade jag till en png-fil i resource manager, lade till ImageView i activity_main.xml
och lade till bilden där. Se koden nedan.
```  
        <ImageView
            android:id="@+id/myImage"
            android:layout_width="200dp"
            android:layout_height="200dp"
            android:layout_margin="20dp"
            android:contentDescription="summer_img"
            app:srcCompat="@drawable/summerimg" />
```   
För att få tillgång till knappen och edittext i Java, använde jag findViewById() i MainActivity.java.
Jag behövde importera Button-klassen och EditText-klassen. Se koden nedan.
```
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button myFirstBtn = findViewById(R.id.myFirstBtn);
        EditText myEdtText = findViewById(R.id.myEdtText);
```

Bilder läggs i samma mapp som markdown-filen.

![](android.png)

