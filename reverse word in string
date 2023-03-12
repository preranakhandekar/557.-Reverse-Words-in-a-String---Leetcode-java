class Solution {
    public char[] swap(char[] ch,int i,int j){
        while(i<j){
            char temp=ch[i];
            ch[i]=ch[j];
            ch[j]=temp;
            i++;
            j--;
        }
        return ch;
    }
    
    public String reverseWords(String s) {
        char[] ch=s.toCharArray();
        int j=0;
        for(int i=0;i<ch.length;i++){
            if(ch[i]==' '){ 
                ch=swap(ch,j,i-1); // swap from j to the blank space index-1
                j=i+1;
            }
            if(i==ch.length-1){ // use when i reach to the end of a char array
                ch=swap(ch,j,i);
            }
        }
        String newstring=new String(ch);
        return newstring;

    }
}
