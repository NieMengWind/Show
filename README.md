# Show
public class test
{
  public static void main(String[] args)
  {
    String s1 = "ab";
    String s2 = "a"+"b";
    final String s3 = "a";
    String s4 = s3 + "b";
    String s5 = "a";
    String s6 = s5 + "b";
    String s7 = new String("ab");
    String s8 = s7.intern();
    System.out.pringln(s1 == s2); //true
    System.out.pringln(s1 == s4); //true
    System.out.pringln(s1 == s6); //false
    System.out.pringln(s1 == s7); //false
    System.out.pringln(s1 == s8); //true
  }
}
