**Take a ten minutes walk**

```
public class TenMinWalk {
  public static boolean isValid(char[] walk) {
    int countns = 0;
    int countew = 0;
    char n = 'n';
    char s = 's';
    char e = 'e';
    char w = 'w';
    boolean comprobacion = false;
    
    if (walk.length > 2 && walk.length < 11) {
        for (int i = 0; i < walk.length; i++){
          if (walk[i]==n){
            countns++;
          }
          if (walk[i]==s){
            countns--;
          }
          if (walk[i]==e){
            countew++;
          }
          if (walk[i]==w){
            countew--;
          }
        }
      if (countns == 0 && countew == 0){
        comprobacion = true;
      }
    }
    
    return comprobacion;
  }
}

```
