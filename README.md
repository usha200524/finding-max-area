class Main {
    public static void main(String[] args) {
        int[] heights={1,8,6,2,5,4,8,3,7};
        int ma=0;
        int n=heights.length;
        for(int i=0;i<n-1;i++){
            for(int j=i+1;j<n;j++){
                int h=Math.min(heights[i],heights[j]);
                int b=j-1;
                int a=h*b;
                if(a>ma){
                    ma=a;
                }
            }
        }
        System.out.println("max area is " + ma);
        
        }
}
