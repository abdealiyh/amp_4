# amp_4


PRACTICAL 4
Aim : Programs related to different Layouts 
(Linear, Relative, Table, Grid) 
Steps :
1. Create new Project > Empty Layout > Enter the project name > Finish
2. In the activity_main.xml file, add the following components:
a. Linear Layout (vertical)
b. Buttons (4)
This would be the code in activity_main.xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout 
xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:tools="http://schemas.android.com/tools"
 android:layout_width="409dp"
 android:layout_height="729dp"
 android:orientation="vertical"
 tools:layout_editor_absoluteX="1dp"
 tools:layout_editor_absoluteY="1dp">
 <Button
 android:id="@+id/b1_linear"
 android:layout_width="140dp"
 android:layout_height="80dp"
 android:layout_gravity="center_horizontal"
 android:layout_marginTop="50dp"
 android:backgroundTint="@color/Spanish_Bistre"
 android:text="Linear" />
 <Button
 android:id="@+id/b2_relative"
 android:layout_width="140dp"
 android:layout_height="80dp"
 android:layout_gravity="center_horizontal"
 android:layout_marginTop="50dp"
 android:backgroundTint="@color/Russian_Green "
 android:text="Relative" />
 <Button
 android:id="@+id/b3_grid"
 android:layout_width="140dp"
 android:layout_height="80dp"
 android:layout_gravity="center_horizontal"
 android:layout_marginTop="50dp"
 android:backgroundTint="@color/Sage "
 android:text="Grid" />
 PRACTICAL 4
Aim : Programs related to different Layouts 
(Linear, Relative, Table, Grid) 
Steps :
1. Create new Project > Empty Layout > Enter the project name > Finish
2. In the activity_main.xml file, add the following components:
a. Linear Layout (vertical)
b. Buttons (4)
This would be the code in activity_main.xml


          <?xml version="1.0" encoding="utf-8"?>
          <LinearLayout 
          xmlns:android="http://schemas.android.com/apk/res/android"
          xmlns:tools="http://schemas.android.com/tools"
           android:layout_width="409dp"
           android:layout_height="729dp"
           android:orientation="vertical"
           tools:layout_editor_absoluteX="1dp"
           tools:layout_editor_absoluteY="1dp">
           <Button
           android:id="@+id/b1_linear"
           android:layout_width="140dp"
           android:layout_height="80dp"
           android:layout_gravity="center_horizontal"
           android:layout_marginTop="50dp"
           android:backgroundTint="@color/Spanish_Bistre"
           android:text="Linear" />
           <Button
           android:id="@+id/b2_relative"
           android:layout_width="140dp"
           android:layout_height="80dp"
           android:layout_gravity="center_horizontal"
           android:layout_marginTop="50dp"
           android:backgroundTint="@color/Russian_Green "
           android:text="Relative" />
           <Button
           android:id="@+id/b3_grid"
           android:layout_width="140dp"
           android:layout_height="80dp"
           android:layout_gravity="center_horizontal"
           android:layout_marginTop="50dp"
           android:backgroundTint="@color/Sage "
           android:text="Grid" />



Add other layout pages:
App > New > Activity > Empty Activity
similarly , create for relative, grid and table. The java and the xml files will be created.


Let’s first design all the pages [xml files]
Activity_linear.xml

            <?xml version="1.0" encoding="utf-8"?>
            <LinearLayout 
            xmlns:android="http://schemas.android.com/apk/res/android"
             xmlns:app="http://schemas.android.com/apk/res-auto"
             xmlns:tools="http://schemas.android.com/tools"
             android:layout_width="match_parent"
             android:layout_height="match_parent"
             android:backgroundTint="@color/Spanish_Bistre"
             android:foregroundTint="@color/design_default_color_error"
             android:orientation="vertical">
             <TextView
             android:id="@+id/textView"
             android:layout_width="match_parent"
             android:layout_height="wrap_content"
             android:backgroundTint="#6E3B3B"
             android:fontFamily="@font/akaya_telivigala"
             android:text="This is Linear Layout"

            android:textAppearance="@style/TextAppearance.AppCompat.Body2"
             android:textSize="32dp"
             android:typeface="normal" />
             <ImageView
             android:id="@+id/imageView"
             android:layout_width="match_parent"
             android:layout_height="259dp"
             app:srcCompat="@drawable/linear" />
             <TextView
             android:id="@+id/textView2"
             android:layout_width="match_parent"
             android:layout_height="wrap_content"
             android:fontFamily="casual"
             android:text="Android LinearLayout is a view group that 
            aligns all children in either vertically or horizontally."
             android:textSize="24sp"
             android:textStyle="bold"
             android:typeface="sans" />
            </LinearLayout>
            
Activity_relative.xml

            <?xml version="1.0" encoding="utf-8"?>
            <RelativeLayout 
            xmlns:android="http://schemas.android.com/apk/res/android"
             xmlns:app="http://schemas.android.com/apk/res-auto"
             xmlns:tools="http://schemas.android.com/tools"
             android:layout_width="match_parent"
             android:layout_height="match_parent"
             tools:context=".relative">
             <EditText
             android:id="@+id/e1"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_alignParentStart="true"
             android:layout_alignParentTop="true"
             android:layout_margin="10sp"
             android:layout_marginStart="10sp"
             android:layout_marginTop="10sp"
             android:layout_marginEnd="10sp"
             android:layout_marginBottom="10sp"
             android:ems="10"
             android:inputType="textPersonName"
             android:minHeight="48dp"
             android:text="Name" />
             <EditText
             android:id="@+id/e2"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_below="@id/e2"
             android:layout_alignParentStart="true"
             android:layout_alignParentTop="true"
             android:layout_marginStart="10sp"
             android:layout_marginTop="50sp"
             android:layout_marginEnd="10sp"
             android:layout_marginBottom="10sp"
             android:ems="10"
             android:inputType="textPersonName"
             android:minHeight="48dp"
             android:text="Password" />
             <Button
             android:id="@+id/button4"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_margin="10sp"
             android:backgroundTint="#84a59d"
             android:text="Login"
             android:layout_below="@id/e2"/>
             <Button
             android:id="@+id/button7"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_margin="10sp"
             android:backgroundTint="#f28482"
             android:text="Cancel"
             android:layout_below="@id/e2"
             android:layout_toRightOf="@id/button4"/>
             <TextView
             android:id="@+id/textView3"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_alignParentStart="true"
            android:layout_alignParentBottom="true"
             android:layout_marginStart="19dp"
             android:layout_marginBottom="295dp"
             android:fontFamily="@font/akaya_telivigala"
             android:text="This is Relative Layout"

            android:textAppearance="@style/TextAppearance.AppCompat.Large"
             android:textSize="24sp"
             android:textStyle="bold" />
             <TextView
             android:id="@+id/textView4"
             android:layout_width="362dp"
             android:layout_height="wrap_content"
             android:layout_alignParentStart="true"
             android:layout_alignParentBottom="true"
             android:layout_marginStart="20dp"
             android:layout_marginBottom="217dp"
             android:text="The position of each view can be specified as 
            relative to sibling elements or relative to the parent."
             android:textSize="20sp" />
            </RelativeLayout>
            
Activity_grid.xml

            <?xml version="1.0" encoding="utf-8"?>
            <GridLayout 
            xmlns:android="http://schemas.android.com/apk/res/android"
             xmlns:app="http://schemas.android.com/apk/res-auto"
             xmlns:tools="http://schemas.android.com/tools"
             android:layout_width="match_parent"
             android:layout_height="match_parent"
             tools:context=".grid"
             android:rowCount="3"
             android:columnCount="3"
             android:id="@+id/grid1">
             <Button
             android:id="@+id/button"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_row="0"
             android:layout_rowWeight="1"
             android:layout_column="0"
             android:layout_columnWeight="1"
             android:layout_gravity="fill"
             android:layout_margin="10sp"
             android:backgroundTint="@color/Russian_Green"
             android:text="Btn (1,1)" />
             <Button
             android:id="@+id/button2"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
            android:layout_row="0"
             android:layout_rowWeight="1"
             android:layout_column="1"
             android:layout_columnWeight="1"
             android:layout_gravity="fill"
             android:layout_margin="10sp"
             android:backgroundTint="#506F5C"
             android:text="Btn (1,2)" />
             <Button
             android:id="@+id/button3"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_row="0"
             android:layout_rowWeight="1"
             android:layout_column="2"
             android:layout_columnWeight="1"
             android:layout_gravity="fill"
             android:layout_margin="10sp"
             android:backgroundTint="#50ACA5"
             android:text="Btn (1,3)" />
             <Button
             android:id="@+id/button5"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_row="1"
             android:layout_rowWeight="1"
             android:layout_column="0"
             android:layout_columnWeight="1"
             android:layout_gravity="fill"
             android:layout_margin="10sp"
             android:backgroundTint="#31433F"
             android:text="Btn (2,1)" />
             <TextView
             android:id="@+id/textView"
             android:layout_width="0dp"
             android:layout_height="wrap_content"
             android:layout_row="1"
             android:layout_rowWeight="1"
             android:layout_column="1"
             android:layout_columnWeight="1"
             android:layout_margin="10sp"
             android:background="#A9E7BD"
             android:fontFamily="monospace"
             android:text="This is Grid Layout"
             android:textAlignment="center"
             android:textAllCaps="false"
             android:textSize="16sp"
             android:textStyle="bold"
             app:layout_constraintLeft_toLeftOf="@id/button5"
             app:layout_constraintRight_toLeftOf="@id/button6" />
            <!-- android:layout_gravity="fill"-->
            <!-- android:textAlignment="center"-->
             <Button
             android:id="@+id/button6"
             android:layout_width="wrap_content"
             android:layout_height="wrap_content"
             android:layout_row="1"
             android:layout_rowWeight="1"
             android:layout_column="2"
             android:layout_columnWeight="1"
             android:layout_gravity="fill"
             android:layout_margin="10sp"
             android:backgroundTint="@color/teal_700"
             android:text="Btn (2,3)" />
            </GridLayout>
            
Activity_table.xml

              <?xml version="1.0" encoding="utf-8"?>
              <TableLayout
               xmlns:android="http://schemas.android.com/apk/res/android"
               xmlns:app="http://schemas.android.com/apk/res-auto"
               xmlns:tools="http://schemas.android.com/tools"
               android:layout_width="409dp"
               android:layout_height="601dp"
               android:orientation="horizontal"
               tools:layout_editor_absoluteX="1dp"
               tools:layout_editor_absoluteY="1dp"
               tools:context=".table"
               android:padding="20dp"
               android:stretchColumns="0">
               <TableRow>
               <TextView
               android:id="@+id/textView5"
               android:layout_width="wrap_content"
               android:layout_height="wrap_content"
               android:text="This is Table View"
               android:textSize="16sp"
               android:textStyle="bold" />
               <TextView
               android:id="@+id/textView6"
               android:layout_width="wrap_content"
               android:layout_height="wrap_content"
               android:text="row 1"
               android:textSize="16sp"
               android:textStyle="bold" />
               </TableRow>
               <TableRow>
               <Button
               android:id="@+id/button9"
              android:layout_width="wrap_content"
               android:layout_height="wrap_content"
               android:backgroundTint="#C9ADA1"
               android:text="Button 1"
               app:cornerRadius="10dp" />
               <Button
               android:id="@+id/button8"
               android:layout_width="wrap_content"
               android:layout_height="wrap_content"
               android:text="Button 2"
               android:backgroundTint="#4D6A6D"
               app:cornerRadius="30dp"/>
               </TableRow>
               <TableRow>
               <Button
               android:id="@+id/button10"
               android:layout_width="wrap_content"
               android:layout_height="wrap_content"
               android:text="Button 3"
               android:layout_span="2"
               android:backgroundTint="#0E6BA8"
               app:cornerRadius="80dp"/>
               </TableRow>
              </TableLayout>
              
              
Adding code to MainActivity.java:

              package com.example.prac4_2;
              import androidx.appcompat.app.AppCompatActivity;
              import android.content.Intent;
              import android.os.Bundle;
              import android.view.View;
              import android.widget.Button;
              public class MainActivity extends AppCompatActivity {
               Button linear, relative, grid, table;
               @Override
               protected void onCreate(Bundle savedInstanceState) {
               super.onCreate(savedInstanceState);
               setContentView(R.layout.activity_main);
               // hooks
               linear = findViewById(R.id.b1_linear);
               relative = findViewById(R.id.b2_relative);
               grid = findViewById(R.id.b3_grid);
               table = findViewById(R.id.b4_table);
               // listeners
               linear.setOnClickListener(new View.OnClickListener(){
               @Override
               public void onClick(View view) {
               Intent intent = new Intent(getApplicationContext(), 
              linear.class);
               startActivity(intent);
              }
               });
               relative.setOnClickListener(new View.OnClickListener(){
               @Override
               public void onClick(View view) {
               Intent intent = new Intent(getApplicationContext(), 
              relative.class);
               startActivity(intent);
               }
               });
               grid.setOnClickListener(new View.OnClickListener(){
               @Override
               public void onClick(View view) {
               Intent intent = new Intent(getApplicationContext(), 
              grid.class);
               startActivity(intent);
               }
               });
               table.setOnClickListener(new View.OnClickListener(){
               @Override
               public void onClick(View view) {
               Intent intent = new Intent(getApplicationContext(), 
              table.class);
               startActivity(intent);
               }
               });
               }
              }
              
              
colors.xml

          <?xml version="1.0" encoding="utf-8"?>
          <resources>
           <color name="purple_200">#FFBB86FC</color>
           <color name="purple_500">#FF6200EE</color>
           <color name="teal_700">#FF018786</color>
           <color name="black">#FF000000</color>
           <color name="purple_700">#FF3700B3</color>
           <color name="teal_200">#068D80</color>
           <color name="white">#FFFFFFFF</color>
           <!-- Button Colors -->
           <color name="Spanish_Bistre">#7C6A0A</color>
           <color name="Old_Lavender">#6A5D7B</color>
           <color name="Russian_Green">#749C75</color>
           <color name="Sage">#8B9043</color>
          </resources>
          
          



