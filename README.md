# trail-project


abc




Reverse a string 
class sstring{
    public String reverseWords(String s) {
        String ans="";
        int i=s.length()-1;
        int j;
        
        while(i>=0)
        {           
            while (i >=0 && s.charAt(i)==' ' ) /while loop
                i--;
             j=i;
            if(i<0) break;
            while(i>=0 && s.charAt(i)!=' ' ) /while loop
                i--;
           if(ans.isEmpty())
           {ans = ans .concat(s.substring(i+1,j+1));
           }
            else
            {
                ans = ans .concat(" " +s.substring(i+1,j+1));
            }
                
                
        }
       
        return ans;
        
    }
}
