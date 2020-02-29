#   Screenshoot
```JAVA
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_2"); // Report
test.get().pass("Menampilkan Form Update Company", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_2.png").build());
```
            
#   Text
```JAVA
test.get().pass("Mengklik Company Code :" + linkno.getText());
```
