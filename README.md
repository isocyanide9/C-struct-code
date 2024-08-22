#include<stdio.h>
struct rect
{
     float length;
    float breadth;
};
int main()
{
    struct rect arr[100];
    int n;
    float area=0,index=0;
    printf("How many rectangle : ");
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    {
        printf("Enter the length of %d rectangle : ",i+1);
        scanf("%f",&arr[i].length);
        printf("Enter the breadth of %d rectangle : ",i+1);
        scanf("%f",&arr[i].breadth);
    }
    for(int i=0;i<n;i++)
    {
        if(arr[i].length*arr[i].breadth>=0)
        {
            area=arr[i].length*arr[i].breadth;
            index+=1;
        }
    }

    printf("Largest rectangle area is %f with rectangle no. %f : ",area,index);
    return 0;


    

}
