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