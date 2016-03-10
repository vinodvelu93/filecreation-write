# filecreation-write
package com.serialisation;

import java.io.File;
import java.io.FileWriter;
import java.io.IOException;

public class File1 {
	
	public static void main(String[] args) throws IOException {
		File f1= new File("D:/A.txt");
		try{
			f1.createNewFile();
		}
		catch(Exception e){
			System.out.println(e);
		}
		FileWriter w= new FileWriter("D:/A.txt");
		try{
			w.write("hai");
		}
		catch(Exception e){
			System.out.println(e);
		}
		w.close();
		// TODO Auto-generated method stub

	}

}
