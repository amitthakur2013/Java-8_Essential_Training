# Java-8_Essential_Training

# Number Format Class implementation and demo
// Your First Program
import java.text.NumberFormat;
import java.util.Locale;

class HelloWorld {
    public static void main(String[] args) {
       Locale locale = new Locale("da","DK");
       double val=1234569.89;
       System.out.println("Locale: " + locale.hashCode());  
       System.out.println(locale.getDisplayLanguage());
       System.out.println(locale.getDisplayCountry());
       NumberFormat numf= NumberFormat.getNumberInstance(locale);
       System.out.println("Money : "+numf.format(val));
       NumberFormat curf = NumberFormat.getCurrencyInstance(locale);
       System.out.println("Currency: "+curf.format(val));
       
       
    }
}
