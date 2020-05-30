~~~~~~
public class problem3 {
   static int[][] graph;
   public static void main(String args[]) {
      int total_sp = 121;
      int[][] skills = {{1,2},{1,3},{3,6},{3,4},{3,5}};
      int[] answer = {};
      int[] list = new int[100000];
      int[] parent = new int[100000];
      int[] child = new int[100000];
      int max = skills.length+1;
      int sum = 0;
      
      for(int i=0; i<max-1; i++) {
         int x = skills[i][0];
         int y = skills[i][1];
         parent[y]=x;
         child[x]++;
      }
      
      for(int i=1; i<=max; i++) {
         if(parent[i]>0) {
            if(child[i]==0){
               list[i]=1;
               int x = i;
               while(parent[x] != 0) {
                  list[parent[x]]++;
                  x = parent[x];      
               }
            }
         }
      }
      
      for(int i=1; i<=max; i++) {
         sum+=list[i];
      }
      
      sum = total_sp /sum;
      
      answer = new int[max];
      
      for(int i=0; i<max; i++) {
         answer[i] = list[i+1]*sum;
      }
   }
}
~~~~~~
