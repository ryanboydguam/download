# download
SimpleDownloadSystemForJava
Hello,
This is a simple download system for Java. 
In your main class just add this line 
new Thread(new Download(link,out)).start();

Make sure your link is a string to the file you want to download and the out is a out folder. For example (MAC USER INSTRUCTIONS)
This may or may not work on windows you just need to try it but if it dosent you just need to implement the output for an example c:\\location
String fileSaveLocation=System.getProperty("user.home");
this will get your user home directory. Then just do += to the location you want to create. If you have any other questions feel free to ask at ryan#8929 on discord

EXAMPLE OF MAIN FILE
String link = "https://www.dropbox.com/s/q0xuvxlsimd5dyz/sample.png?dl=1";
		String fileSaveLocation=System.getProperty("user.home");
		fileSaveLocation += "/Desktop/trash.png";
		File out = new File(fileSaveLocation);
		new Thread(new Download(link,out)).start();
    
    
