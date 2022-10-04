import java.util.*;
public class Password{
 public static void main(String[] args){
 int length=16;
 System.out.println(geek_password(length));
 }
 static char[]geek_password(int len){
 System.out.println("Generating Password random():");
 System.out.println("Your new password is:");
 String Capital_chars="ABCDEFGHIJKLMNOPQRSTUVWXYZ";
 String small_chars="abcdefghijklmnopqrstuvwxuyz";
 String numbers="1234567890";;
 String symbols="~!@#$%^&*()_+";
 String values=Capital_chars+small_chars+numbers+symbols;
 Random Rndm_methode=new Random();
 char[]password=new char[len];
  for(int i=0;i<len;i++){
  password[i]=values.charAt(Rndm_methode.nextInt(values.length()));  
  }
  return password;
 }
}
