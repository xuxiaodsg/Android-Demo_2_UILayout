# 实验2_Android界面布局



## Android布局实验——线性布局

利用线性布局实现如下界面：

![image-20210927155949930](https://user-images.githubusercontent.com/81363852/134870738-d81e9996-c5e8-4c79-b8c5-f6630d2c8214.png)


代码:

```java
<LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">

        <Button
            android:id="@+id/button3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button18"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button19"
            android:layout_width="129dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button20"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal"
        >

        <Button
            android:id="@+id/button21"
            android:layout_width="126dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button22"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button23"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button24"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">

        <Button
            android:id="@+id/button25"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button31"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button32"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button33"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="50dp"
        android:orientation="horizontal">

        <Button
            android:id="@+id/button34"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button35"
            android:layout_width="117dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button36"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />

        <Button
            android:id="@+id/button37"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="Button" />
    </LinearLayout>
```

结果:

![image-20210927161008180](https://user-images.githubusercontent.com/81363852/134870768-e1cd0934-ca1b-4c59-b786-241436d12d4e.png)





## Android布局实验——约束布局

• 利用ConstraintLayout实现如下界面：

![image-20210927161128928](https://user-images.githubusercontent.com/81363852/134870791-579d031b-6d14-4d7d-9227-b77cd57379f1.png)


代码:

```java
<Button
        android:id="@+id/button17"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="."
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button15"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button13" />

    <Button
        android:id="@+id/button14"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="-"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button16"
        app:layout_constraintTop_toBottomOf="@+id/button10" />

    <Button
        android:id="@+id/button15"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="0"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button16"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button17"
        app:layout_constraintTop_toBottomOf="@+id/button11" />

    <Button
        android:id="@+id/button16"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="="
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/button14"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button15"
        app:layout_constraintTop_toBottomOf="@+id/button12" />

    <Button
        android:id="@+id/button13"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="1"
        app:layout_constraintBottom_toTopOf="@+id/button17"
        app:layout_constraintEnd_toStartOf="@+id/button11"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button9" />

    <Button
        android:id="@+id/button10"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="+"
        app:layout_constraintBottom_toTopOf="@+id/button14"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button12"
        app:layout_constraintTop_toBottomOf="@+id/button6" />

    <Button
        android:id="@+id/button11"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="2"
        app:layout_constraintBottom_toTopOf="@+id/button15"
        app:layout_constraintEnd_toStartOf="@+id/button12"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button13"
        app:layout_constraintTop_toBottomOf="@+id/button7" />

    <Button
        android:id="@+id/button12"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="3"
        app:layout_constraintBottom_toTopOf="@+id/button16"
        app:layout_constraintEnd_toStartOf="@+id/button10"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button11"
        app:layout_constraintTop_toBottomOf="@+id/button8" />

    <Button
        android:id="@+id/button9"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="4"
        app:layout_constraintBottom_toTopOf="@+id/button13"
        app:layout_constraintEnd_toStartOf="@+id/button7"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button2" />

    <Button
        android:id="@+id/button6"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="*"
        app:layout_constraintBottom_toTopOf="@+id/button10"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button8"
        app:layout_constraintTop_toBottomOf="@+id/button4" />

    <Button
        android:id="@+id/button7"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="5"
        app:layout_constraintBottom_toTopOf="@+id/button11"
        app:layout_constraintEnd_toStartOf="@+id/button8"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button9"
        app:layout_constraintTop_toBottomOf="@+id/button5" />

    <Button
        android:id="@+id/button8"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="6"
        app:layout_constraintBottom_toTopOf="@+id/button12"
        app:layout_constraintEnd_toStartOf="@+id/button6"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button7"
        app:layout_constraintTop_toBottomOf="@+id/button" />

    <Button
        android:id="@+id/button2"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="7"
        app:layout_constraintBottom_toTopOf="@+id/button9"
        app:layout_constraintEnd_toStartOf="@+id/button5"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/editTextTextPersonName3" />

    <Button
        android:id="@+id/button4"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="/"
        app:layout_constraintBottom_toTopOf="@+id/button6"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button"
        app:layout_constraintTop_toBottomOf="@+id/editTextTextPersonName3" />

    <Button
        android:id="@+id/button5"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="8"
        app:layout_constraintBottom_toTopOf="@+id/button7"
        app:layout_constraintEnd_toStartOf="@+id/button"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button2"
        app:layout_constraintTop_toBottomOf="@+id/editTextTextPersonName3" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="121dp"
        android:layout_height="41dp"
        android:layout_marginStart="20dp"
        android:layout_marginTop="16dp"
        android:text="Input"
        android:textSize="24sp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <EditText
        android:id="@+id/editTextTextPersonName3"
        android:layout_width="368dp"
        android:layout_height="52dp"
        android:layout_marginTop="44dp"
        android:ems="10"
        android:gravity="right|bottom"
        android:inputType="textPersonName"
        android:text="0.0"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView" />

    <Button
        android:id="@+id/button"
        android:layout_width="58dp"
        android:layout_height="wrap_content"
        android:text="9"
        app:layout_constraintBottom_toTopOf="@+id/button8"
        app:layout_constraintEnd_toStartOf="@+id/button4"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/button5"
        app:layout_constraintTop_toBottomOf="@+id/editTextTextPersonName3" />
        			          
```

结果:

![image-20210927161257245](https://user-images.githubusercontent.com/81363852/134870806-78259d66-6ce4-45fb-8d51-d3f3c42d0425.png)



## Android布局实验——表格布局

• 利用表格布局实现如下界面：

![image-20210927161318136](https://user-images.githubusercontent.com/81363852/134870827-665ba9cd-d7aa-4225-bb14-ebbacc7d1999.png)


代码:

```java
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="10dp">
        <TextView
            android:id="@+id/textView"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text="Open..."
            android:textSize="24sp" />
        <TextView
            android:id="@+id/textView2"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text=""
            android:textSize="24sp" />

        <TextView
            android:id="@+id/textView3"
            android:layout_width="168dp"
            android:layout_height="41dp"
            android:text="Ctrl+O"
            android:gravity="right"
            android:textSize="24sp" />
    </TableRow>
    <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="10dp">
        <TextView
            android:id="@+id/textView4"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text="Save..."
            android:textSize="24sp" />
        <TextView
            android:id="@+id/textView5"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text=""
            android:textSize="24sp" />

        <TextView
            android:id="@+id/textView6"
            android:layout_width="168dp"
            android:layout_height="41dp"
            android:text="Ctrl+S"
            android:gravity="right"
            android:textSize="24sp" />
    </TableRow>
    <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="10dp">
        <TextView
            android:id="@+id/textView7"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text="Save as..."
            android:textSize="24sp" />
        <TextView
            android:id="@+id/textView8"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text=""
            android:textSize="24sp" />

        <TextView
            android:id="@+id/textView9"
            android:layout_width="168dp"
            android:layout_height="41dp"
            android:text="Ctrl+Shift+S"
            android:gravity="right"
            android:textSize="24sp" />
    </TableRow>
    <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="10dp">
        <TextView
            android:id="@+id/textView11"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text="X Import..."
            android:textSize="24sp" />

    </TableRow>
    <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="10dp">
        <TextView
            android:id="@+id/textView12"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text="X Export..."
            android:textSize="24sp" />
        <TextView
            android:id="@+id/textView18"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text=""
            android:textSize="24sp" />

        <TextView
            android:id="@+id/textView19"
            android:layout_width="168dp"
            android:layout_height="41dp"
            android:text="Ctrl+E    "
            android:gravity="right"
            android:textSize="24sp" />

    </TableRow>
    <TableRow
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="10dp">
        <TextView
            android:id="@+id/textView111"
            android:layout_width="121dp"
            android:layout_height="41dp"
            android:text="Quit"
            android:textSize="24sp" />

    </TableRow>

</TableLayout>
```

结果:

![image-20210927161405563](https://user-images.githubusercontent.com/81363852/134870846-fb74c786-3eab-45ce-9ede-b4cb40d0d401.png)

