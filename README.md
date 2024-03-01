int peakElement(int arr[], int n)
    {
       // Your code here
       if(n==1) return 0 ;
       int mid=low+(high-low)/2 ;
       while(low<high){
           if(arr[mid] <arr[mid+1]){
              low=mid+1 ;
           }
           else{
               high=mid ;
           }
           mid=low+(high-low)/2 ;
       }
       return low ;
    }
