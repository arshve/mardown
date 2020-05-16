Menu +[TASK](https://github.com/arshve/mardown/blob/master/Task.md)+ +[Repo Input](https://github.com/arshve/mardown/blob/master/Repo%20Input.md#Insert-Multiple-input-To-Right-Box)+ +[Repo Button](https://github.com/arshve/mardown/blob/master/Repo%20Button.md)+ +[Repo Documentation](https://github.com/arshve/mardown/blob/master/Repo%20Documentation.md)+ +[Repo Select By](https://github.com/arshve/mardown/blob/master/Repo%20Select%20By.md)+ +[Repo Select](https://github.com/arshve/mardown/blob/master/Repo%20Select.md)+ +[ModulSF List](https://github.com/arshve/mardown/blob/master/ModulSF6.md)+

## Screenshoot

```JAVA
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_2"); // Report
test.get().pass("Menampilkan Form Update Company", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_2.png").build());
```

## Text

```JAVA
test.get().pass("Mengklik Company Code :" + linkno.getText());
```

## Make a Array Report

```JAVA
Assert.assertEquals(inp_pos_flagval, "Yes");
String[][] data = {
        {"<small>[Radio Button]</small>"},
        {"<b>Position Flag</b>"},
        {inp_pos_flagval}
};
```
