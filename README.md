# ruanjiangongcheng
package softwareengineering;

public class BubbleSort {
    public static void main(String[] args) {
        
        int[] num=new int[]{1,5,8,2,3,9,4};
        int i,j;
        for(i=0;i<num.length-1;i++){
        	
            for(j=0;j<num.length-1-i;j++){
            	
                if(num[j]>num[j+1]){
                	
                    int temp=num[j];
                    num[j]=num[j+1];
                    num[j+1]=temp;
                }
            }
        }
        System.out.println("从小到大排序后的结果是:");
        for(i=0;i<num.length;i++)
            System.out.print(num[i]+" ");
    }
}
